# xbps-builder

This is an XBPS builder, inspired by the
[xbps-mini-builder](https://github.com/the-maldridge/xbps-mini-builder).

Use this script to create a repository of selected packages and automatically
update them when they're outdated. This is useful for restricted packages which
are not contained in the offical repository.

Unlike xbps-mini-builder, it uses `xbps-checkvers(1)` to check for outdated
packages in your local repository. Additionally it can build packages for
multiple architectures which is not supported by xbps-mini-builder.

## Instructions

Copy the `conf.example` file to `conf` and modify it to your liking.

xbps-builder won't create the `void-packages` repository for you.
Clone it from https://github.com/void-linux/void-packages.git and specify the
path in the `distdir` variable in the `conf` configuration file.

Execute `./xbps-builder`.
