# Learning `dpkg`
## [Link](http://www.hackgnar.com/2016/01/simple-deb-package-creation.html)

### Hacking
#### Before

```
$ ls build
my-awesome-package
```

#### Setup

- **macOS**: Run `brew bundle`
- Run `bin/build`

#### After

```
$ ls build
my-awesome-package     my-awesome-package.deb
```

Then you can...
```
dpkg -i my-awesome-package.deb
```
...wherever you want!

## To be continued...

I feel pretty good about this setup currently. For simple scripts, this should work great, and it doesn't seem like too much to ask that a developer have `brew` installed on their Mac. However, I would like to look into alternatives for easy linux distribution, maybe even dropping debian packages in favor of something more universal.

### Misc

- Alternatives to installing `dpkg`
  - https://www.npmjs.com/package/debify
  - https://www.npmjs.com/package/unipkg
- Creating `.deb`'s with less boilerplate
  - https://blog.packagecloud.io/eng/2016/12/15/howto-build-debian-package-containing-simple-shell-scripts/
  - https://www.npmjs.com/package/node-deb
- Alternatives to `.deb`
  - https://appimage.org
  - https://docs.snapcraft.io/pre-built-apps/6739
