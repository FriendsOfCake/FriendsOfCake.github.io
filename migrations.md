---
layout: default
title: migrations
---

# Migration Guide

These are steps you can take to help comply with the Friends Of Cake [project requirements](requirements.html).

## Continuous integration with TravisCI
- Add a `.travis.yml` file to the root of your project and [activate the GitHub webhook](http://docs.travis-ci.com/user/getting-started/#Step-two%3A-Activate-GitHub-Webhook).

- Ensure your matrix includes the PHP versions from the boarding requirements.
- Ensure your matrix includes the CakePHP versions from the boarding requirements.
- Please keep `Notifications: email` set to `false` to avoid spamming (_perhaps add IRC notifications?_).

[Review an example `.travis.yml`](https://github.com/FriendsOfCake/crud/blob/develop/.travis.yml) from a Friends Of Cake project.

## CakePHP code style guide
*phpcs --standard=CakePHP* is used to check coding standards. More information is available on GitHub at [cakephp-codesniffer](https://github.com/cakephp/cakephp-codesniffer).

## Composer support
- Add a `composer.json` file to the root of your project, see http://getcomposer.org/doc/04-schema.md
- Set the [vendor part of your name property](https://getcomposer.org/doc/04-schema.md#name) to `friendsofcake` (i.e. friendsofcake/yet-another-wonderful-name).
- Ensure you [use the `installer-name` extra](https://github.com/composer/installers#custom-install-names) as Composer package names don't allow uppercases, yet CakePHP expects your plugin folder name to be CamelCased.

[Review an example `composer.json`](https://github.com/FriendsOfCake/crud/blob/develop/composer.json) from a Friends Of Cake project.

## Code coverage with Coveralls
- Write tests. 🙇
- Add a `.coveralls.yml` file to the root of your project.
- Ensure Travis handles Coveralls (see Travis example above).

## Packagist
Submit the package to [Packagist](https://packagist.org/).

## MIT license
Add a `LICENSE.txt` file to the root of your project.

[Review an example `LICENSE.txt`](https://github.com/FriendsOfCake/crud/blob/develop/LICENSE.txt) from a Friends Of Cake project.

## Documenation
- Must have well documented code (docblocks, @annotations etc)
- Must have well documented user guide with examples.
- GitHub Wiki pages should not be used for documentation. Use gh-pages or README.md.

## GitHub releases
[Releases](https://help.github.com/articles/about-releases/) and [Tags](http://git-scm.com/book/en/v2/Git-Basics-Tagging) must use [semantic versioning](http://semver.org/) with descriptive changelogs. Head to GitHub for more [information on creating releases](https://help.github.com/articles/creating-releases).

## Branching
- Must use `master` for stable release, `develop` for integration branch and feature branches for the rest.
