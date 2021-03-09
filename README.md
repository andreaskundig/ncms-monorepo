# configure subprojects for monorepo

Make sure the netlifyCMS configurations point to the correct folders.

Fix paths in all [subproject]/src/admin/config.yml

``` yaml
media_folder: "[subproject]/src/static/img"
```

# create a netlify website

**Team overview > New site from git**
build command: npm run build
publish directory: \_site_

After the creation, go the new site's configuration

## Set the base directory

**Site settings > Build settings > Base directory: dating-privacy**

https://docs.netlify.com/configure-builds/get-started/#basic-build-settings

## Enable netlify Identity
**Identity > Enable Identity**
https://docs.netlify.com/visitor-access/identity/#enable-identity-in-the-ui

Set Registration to invite only
**Site settings > Identity > Registration > Registration preferences > Edit Settings**

Invite a user by adding her email address.
**Identity > Invite users**

## Enable git gateway
**Site settings > Identity > Services > Git Gateway > Enable Git Gateway**
https://docs.netlify.com/visitor-access/git-gateway/

