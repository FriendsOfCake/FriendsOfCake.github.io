# MIGRATION GUIDE

List of steps to take to comply to the requirements

## Setup Travis CI

- Add a `.travis.yml` file to the root of your project and activate the github hook for travis, see
http://about.travis-ci.org/docs/user/getting-started/#Step-one%3A-Sign-in
Example `.travis.yml` file for cakephp plugin: https://github.com/FriendsOfCake/crud/blob/develop/.travis.yml
- Ensure your matrix includes the PHP versions from the boarding requirements
- Ensure your matrix inlcudes the CakePHP versions from the boarding requirements
- Please keep Notifications: email as `false` to avoid spamming (perhaps add irc notifications?)

## CakePHP code guidelines

phpcs --standard=CakePHP is used to check coding standards
More info: https://github.com/cakephp/cakephp-codesniffer
Ensure the travis build matrix includes a PHPCS job, see the above eample `.travis.yml`

## Setup composer support

- Add a composer.json file to the root of your project, see http://getcomposer.org/doc/04-schema.md
- Use `friendsofcake` as vendorname
- Ensure you use installer-name, as composer package names don't allow uppercases, but CakePHP expects your
plugin foldername to be CamelCased
Example file: https://github.com/FriendsOfCake/crud/blob/develop/composer.json

## Code coverage and coveralls

- Write tests :)
- Add `.coveralls.yml` file to the root of your project
- Ensure travis handles coveralls (see the above example `.travis.yml`)

## Packagist

Submit the package to packagist, https://packagist.org/packages/submit

## MIT license

Add LICENSE.txt to the root of your project
Example: https://github.com/FriendsOfCake/crud/blob/develop/LICENSE.txt

## Documenation

- Must have well documented code (docblocks, @annotations etc)
- Must have well documented user guide with examples
- GitHub wiki pages should not be used for documentation. Use gh-pages or README.md

## GitHub releases

Use GitHub releases and git atgs using semantic versioning with descriptive changelogs
More info: https://help.github.com/articles/creating-releases

## Branching

- Must use `master` for stable release, `develop` for integration branch and feature branches for the rest
