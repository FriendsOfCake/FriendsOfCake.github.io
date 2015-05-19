#friendsofcake.com

[![Travis](https://img.shields.io/travis/chrisvogt/FriendsOfCake.github.io.svg?style=flat-square)](https://travis-ci.org/chrisvogt/FriendsOfCake.github.io)
[![Code Climate](https://img.shields.io/codeclimate/github/chrisvogt/FriendsOfCake.github.io.svg?style=flat-square)](https://codeclimate.com/github/chrisvogt/FriendsOfCake.github.io)
[![GitHub license](https://img.shields.io/github/license/FriendsOfCake/FriendsOfCake.github.io.svg?style=flat-square)](https://github.com/FriendsOfCake/FriendsOfCake.github.io/blob/master/LICENSE)
<img src="img/FOC.png" alt="Friends Of Cake" width="280" align="right">

This repository holds the source code to the [friendsofcake.com](http://friendsofcake.com) website, a [Jekyll](http://jekyllrb.com/)-powered site hosted for free on [GitHub Pages](https://pages.github.com/).

### Development Notes

#### Sitting up a local instance

This project is setup to use [Bundler](http://bundler.io/), [Jekyll](http://jekyllrb.com/), and [Bower](http://bower.io/).

After cloning this repository, run:

1. `bundle install` to download dependencies required to build.
2. `bower install` to download front-end packages into the `./components` directory. (This is not necessary for the `master` branch.)
3. `jekyll serve` to run locally or `jekyll build` to generate into `./site` directory.

### Screenshot

![friendsofcake.com screenshot](screenshot.png)

<img src="https://cdn.rawgit.com/jekyll/brand/master/jekyll-logo-light-transparent.png" alt="Made with Jekyll" width="140" align="right" /> <img src="http://bower.io/img/bower-logo.svg" alt="Made with Bower" height="70" align="right">
