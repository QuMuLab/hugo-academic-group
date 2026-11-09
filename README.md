# hugo-academic-group

An academic group website theme for Hugo.


## Installation

 1. Install [Hugo](https://gohugo.io/) and create a new website:

 ```
    hugo new site website_name
    cd website_name
 ```

 2. Clone (or download) the theme to `themes/hugo-academic-group folder`:

 ```
    git clone git@github.com:biaslab/hugo-academic-group.git themes/hugo-academic-group
 ```

 3. Copy all the contents of the `exampleSite` folder to the root of your website, overwriting if necessary:

 ```
    cp -av themes/hugo-academic-group/exampleSite/* .
 ```

 4. Run Hugo server from the root of your website:

 ```
    hugo server --watch
 ```

 Open [localhost:1313](localhost:1313) and your website should appear.


## Citations

The theme includes `cite` and `bibliography` shortcodes for CSL-JSON
references (e.g., a `bib.json` file in a page bundle):

 ```
    Some claim {{< cite "key" >}}.

    {{< bibliography cited >}}
 ```

These are vendored from [hugo-cite](https://github.com/loup-brun/hugo-cite)
(WTFPL, see `layouts/partials/bibliography/LICENSE-hugo-cite`) and updated to
work with current versions of Hugo, so hugo-cite does not need to be installed
separately.
