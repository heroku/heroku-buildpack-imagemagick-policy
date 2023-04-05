**Please note:** This buildpack is a stopgap and not officially supported.

# heroku-buildpack-imagemagick-policy

A tiny buildpack to set a good default policy for ImageMagick coders, disabling the following coders: `EPHEMERAL`, `HTTPS`, `MVG`, `MSL`, and `PDF`.

This is intended to be used in conjunction with other Heroku buildpacks, and may conflict with other buildpacks that vendor ImageMagick and associated policy files.

## Usage

```shell
$ heroku buildpacks:add https://github.com/heroku/heroku-buildpack-imagemagick-policy --index 1 --app <your app>
```
