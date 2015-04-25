#friendsofcake.com

[![Build Status](https://travis-ci.org/chrisvogt/FriendsOfCake.github.io.svg?branch=gh-pages)](https://travis-ci.org/chrisvogt/FriendsOfCake.github.io) [![Code Climate](https://codeclimate.com/github/chrisvogt/FriendsOfCake.github.io/badges/gpa.svg)](https://codeclimate.com/github/chrisvogt/FriendsOfCake.github.io) [![GitHub license](https://img.shields.io/github/license/chrisvogt/FriendsOfCake.github.io.svg?style=flat-square)]() <img src="https://cdn.rawgit.com/chrisvogt/FriendsOfCake.github.io/develop/img/FOC.png" alt="Friends Of Cake" width="280" align="right" />

This repository holds the [friendsofcake.com](http://friendsofcake.com) website code, currently powered by [GitHub Pages](https://pages.github.com/) and [Jekyll](http://jekyllrb.com/).

### Development Notes

#### Setup a local instance

This project is setup to use [Bundler](http://bundler.io/), [Jekyll](http://jekyllrb.com/), and [Bower](http://bower.io/). After cloning this repository, run:

1. `bundle install` to download dependencies required to build.
2. `bower install` to download front-end packages into the `./components` directory.  
3. `jekyll serve` to run locally or `jekyll build` to generate into `./site` directory.

#### Development workflow

The workflow for contributing to this project is as follows:

1. Create a fork of the repository.
2. Base your feature branch on the `develop` repository.
3. Open a [new issue](https://github.com/FriendsOfCake/FriendsOfCake.github.io/issues) describing the bug, feature, or work you will be contributing.
3. Submit pull requests against the `develop` repository.

### Screenshot

![friendsofcake.com screenshot](http://i.imgur.com/7r6JKzP.gif)

<img src="https://cdn.rawgit.com/jekyll/brand/master/jekyll-logo-light-transparent.png" alt="Made with Jekyll" width="140" align="right" /> <img src="http://bower.io/img/bower-logo.svg" alt="Made with Bower" height="70" align="right" />
