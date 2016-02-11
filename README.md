# PLEASE DO NOT USE THIS PACKAGE
This repo currently only exists to support a few applications floating out there in the world.  Reasonable PhantomJS 2 support via npm is now available and there is no longer a good reason for this to exist.

phantomjs
=========

An NPM wrapper for [PhantomJS](http://phantomjs.org/) *version 2*, headless webkit with JS API. 

This is a fork of [a fork](https://github.com/zeevl/phantomjs2) of [Medium/phantomjs](https://github.com/Medium/phantomjs), which currently only installs phantomjs v1.9.x.

The point of this fork is:
- to provide phantomjs 2 support to OS X and Ubuntu 14.04
- to use the "phantomjs" naming, so as to be useful as a peer dependency (unlike the [zeevl phantomjs2 fork](https://github.com/zeevl/phantomjs2))

For Travis support add these lines to your config

```YAML
- mkdir travis-phantomjs
- wget https://s3.amazonaws.com/travis-phantomjs/phantomjs-2.0.0-ubuntu-12.04.tar.bz2
  -O $PWD/travis-phantomjs/phantomjs-2.0.0-ubuntu-12.04.tar.bz2
- tar -xvf $PWD/travis-phantomjs/phantomjs-2.0.0-ubuntu-12.04.tar.bz2 -C $PWD/travis-phantomjs
- export PATH=$PWD/travis-phantomjs:$PATH
```
