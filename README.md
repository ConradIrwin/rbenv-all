Provides `rbenv all` so that you can run the same code under all of the ruby versions you have installed.

Installation
============

Just git clone this repository into a new subdirectory of your rbenv plugins directory:

```
git clone https://github.com/ConradIrwin/rbenv-all ~/.rbenv/plugins/rbenv-all
````

Usage
=====

Just `rbenv all <code you want to run>`. For example to run rspec against all ruby versions that you have installed, use:

```
$ rbenv all rspec
```

By default rbenv all will output a little notification explaining what it is doing for each ruby:

```
$ rbenv all ruby --version
1.8.7-p371>> ruby --version
ruby 1.8.7 (2012-10-12 patchlevel 371) [i686-darwin12.1.0]

1.9.3-p392>> ruby --version
ruby 1.9.3p392 (2013-02-22 revision 39386) [x86_64-darwin12.1.0]
```

To suppress this, pass --bare

```
$ rbenv all --bare ruby --version
ruby 1.8.7 (2012-10-12 patchlevel 371) [i686-darwin12.1.0]

ruby 1.9.3p392 (2013-02-22 revision 39386) [x86_64-darwin12.1.0]
```

Credit
======

This was written by [Sheldon Hearn](https://github.com/sheldonh) in a [pull request](https://github.com/sstephenson/rbenv/pull/110) to rbenv. I just packaged it.
