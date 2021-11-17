# Jekyll-Github-Pages-Documentation
Documentation on how to fix the vendor css file problems with SASS and bootstrap with github pages


#Step 1 - Edit the config.yml

Add url and base url to your .config
```
baseurl: "/repository-name"
url" "https://example.github.io"
```

Add a remote theme
```
remote_theme: jekyll-theme-cayman
```

Add the sass plugin and paths
```
sass:
  load_paths:
      - _sass
      - _css
```

##Step 2 - Edit the .gitignore
the default .gitignore with jekyll includes a vendor path that bootstrap relies on, remove the line that says vendor
```
_site
.sass-cache
.jekyll-cache
.jekyll-metadata
-vendor * DELETE *
```
