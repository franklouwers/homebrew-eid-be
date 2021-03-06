# Homebrew tap for various tools I like, including the Belgian eid middleware

### How do I use the tap?

The following two commands will install the Middleware.

```
brew tap franklouwers/homebrew-franklouwers
brew install --cask eid-be
```

If you want to install the eID Viewer app as well, run this command after running the first two:

```
brew install --cask eid-be-viewer
```

The eID Viewer app is a stand-alone application that reads the (basic) data
from the eID card and allows you to create a nice printout of the eID data.

### Which version do you install?

Please see [the caskfile](Casks/eid-be.rb#L2) to see the current version. We use the "Quickinstall" version of the middleware installer.

On my freshly installed MacOS Catalina, this worked out of the box. Without rebooting, I
was able to pass the test at [eid.belgium.be](https://eid.belgium.be).

### Why does this tap exist?

For [various reasons](https://github.com/Homebrew/homebrew-cask/issues/59021),
the "official" eid tap for Homebrew was archived. The maintainer [isn't
happy](https://github.com/Homebrew/homebrew-cask/pull/65165#issuecomment-504672465) to add the eid Casks to one of the "official" casks.

### What else is in there?

- [my fork of kube-ps1](https://github.com/franklouwers/kube-ps1)
