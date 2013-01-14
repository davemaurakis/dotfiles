brownbathrobes's dotfiles
==================

My system configuration. ([Inspiration](http://zachholman.com/2010/08/dotfiles-are-meant-to-be-forked/))

installation
------------

    git clone git://github.com/brownbathrobe/dotfiles.git ~/.dotfiles
    cd ~/.dotfiles
    rake install
    vim +BundleInstall +qall

notes
-----

- **bin/**: Anything in `bin/` will be added to your `$PATH` and be made
  available everywhere.

- **topic/\*.sh**: Any files ending in `.sh` get loaded into your environment.

- **topic/\*.symlink**: Any files ending in `*.symlink` get symlinked into
  your `$HOME`. (These files get symlinked when you run `rake install`.)

  - symlinks can be generated in cases where these standard **topic/\*.symlink**
  symlink rules do not apply; see the `:install` task of the `Rakefile` for details.

- **.localrc**: Create a file called `.localrc` to store any data that you do
  not want committed to the git repository (secrets, etc.).

system
------

OS X, with the [Homebrew package manager](http://mxcl.github.com/homebrew/).

thanks
------

These dotfiles are heavily based on [Zach Holman's dotfiles](https://github.com/holman/dotfiles).

Includes code from the following dotfiles:
- [Michael J. Russo](http://github.com/mjrusso/dotfiles)
- [Daniel Russo](https://github.com/drusso/dotfiles)
- [Shane Jonas](https://github.com/shanejonas/dotfiles)
- [Nino D'Aversa](https://github.com/ndaversa/vim)
- [Mathias Bynens](https://github.com/mathiasbynens/dotfiles)
- [Andrew Sardone](https://github.com/andrewsardone/dotfiles)
