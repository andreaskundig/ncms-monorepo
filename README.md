# modify project for monorepo

Copy root to site1 and site2.

Fix paths in siteX/src/admin/config.yml

``` yaml

# media_folder: "src/static/img"
media_folder: "site1/src/static/img"
```

# configure netlify
Site settings > Build settings > Base directory: site1

Create another site and change github project

Site settings > Build settings > Repository: link to a different repository
