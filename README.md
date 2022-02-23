# xbps-builder

This is an XBPS builder, inspired by the
[xbps-mini-builder](https://github.com/the-maldridge/xbps-mini-builder).

Use this script to create a repository of selected packages and automatically
update them when they're outdated. This is useful for restricted packages which
are not contained in the offical repository.

## Instructions

Copy the `conf.example` file to `conf` and modify it to your liking.

xbps-builder won't create the `void-packages` repository for you.
Clone it from https://github.com/void-linux/void-packages.git and specify the
path in the `distdir` variable in the `conf` configuration file.

Execute `./xbps-builder`.
