# configure subprojects for monorepo

Make sure the netlifyCMS configurations point to the correct folders.

Fix paths in all [subproject]/src/admin/config.yml

``` yaml
media_folder: "[subproject]/src/static/img"
```

# create a netlify website

Team overview > New site from git
build command: npm run build
publish directory: \_site_

after creation

Site settings > Build settings > Base directory: site2

https://docs.netlify.com/configure-builds/get-started/#basic-build-settings

Enable netlify Identity
Identity > Enable Identity
https://docs.netlify.com/visitor-access/identity/#enable-identity-in-the-ui

Enable git gateway
Site settings > Identity > Services > Git Gateway, and select Enable Git Gateway
https://docs.netlify.com/visitor-access/git-gateway/

