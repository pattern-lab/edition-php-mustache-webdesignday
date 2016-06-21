![license](https://img.shields.io/github/license/pattern-lab/edition-php-mustache-webdesignday.svg?maxAge=2592000)
[![Packagist](https://img.shields.io/packagist/v/pattern-lab/edition-mustache-webdesignday.svg?maxAge=2592000)](https://packagist.org/packages/pattern-lab/edition-mustache-webdesignday) [![Gitter](https://img.shields.io/gitter/room/pattern-lab/php.svg?maxAge=2592000)](https://gitter.im/pattern-lab/php)

# Pattern Lab Web Design Day Edition for Mustache

The Web Design Day Edition for Mustache gives attendees a clean and stable base from which to follow-along with the Pattern Lab workshop.

## Packaged Components

The Web Design Day Edition for Mustache comes with the following components:

* `pattern-lab/core`: [GitHub](https://github.com/pattern-lab/patternlab-php-core), [Packagist](https://packagist.org/packages/pattern-lab/core)
* `pattern-lab/patternengine-mustache`: [documentation](https://github.com/pattern-lab/patternengine-php-mustache#mustache-patternengine-for-pattern-lab-php), [GitHub](https://github.com/pattern-lab/patternengine-php-mustache), [Packagist](https://packagist.org/packages/pattern-lab/patternengine-mustache)
* `pattern-lab/styleguidekit-assets-default`: [GitHub](https://github.com/pattern-lab/styleguidekit-assets-default), [Packagist](https://packagist.org/packages/pattern-lab/styleguidekit-assets-default)
* `pattern-lab/styleguidekit-mustache-default`: [GitHub](https://github.com/pattern-lab/styleguidekit-twig-default), [Packagist](https://packagist.org/packages/pattern-lab/styleguidekit-twig-default)
* `pattern-lab/plugin-faker`: [GitHub](https://github.com/pattern-lab/plugin-php-faker), [Packagist](https://packagist.org/packages/pattern-lab/plugin-faker)
* `pattern-lab/plugin-reload`: [GitHub](https://github.com/pattern-lab/plugin-php-reload), [Packagist](https://packagist.org/packages/pattern-lab/plugin-reload)

## Installing

There are two methods for downloading and installing the Web Design Day Edition for Mustache:

* [Download a pre-built project](#download-a-pre-built-package)
* [Use Composer to create a project](#use-composer-to-create-a-project)

### Download a pre-built project

The fastest way to get started with the Web Design Day Edition for Mustache is to [download the pre-built version](https://github.com/pattern-lab/edition-php-mustache-webdesignday/releases) from the [releases page](https://github.com/pattern-lab/edition-php-mustache-webdesignday/releases).

**Please note:** Pattern Lab uses [Composer](https://getcomposer.org/) to manage project dependencies. To upgrade the Web Design Day Edition for Mustache after the event you'll need to [install Composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx). We recommend that you [install it globally](https://getcomposer.org/doc/00-intro.md#globally).

### Use Composer to create a project

Pattern Lab uses [Composer](https://getcomposer.org/) to manage project dependencies.

#### 1. Install Composer

Please follow the directions for [installing Composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx) on the Composer website. We recommend you [install it globally](https://getcomposer.org/doc/00-intro.md#globally).

#### 2. Install the Web Design Day Edition for Mustache

Use Composer's [`create-project` command](https://getcomposer.org/doc/03-cli.md#create-project) to install the Standard Edition for Twig into a location of your choosing. In Terminal type:

    cd install/location/
    composer create-project pattern-lab/edition-mustache-webdesignday your-project-name && cd $_

This will install the Web Design Day Edition for Mustache into a directory called `your-project-name` in `install/location/`. You will be automatically dropped into the project directory after the process is finished.

## Installing the Web Design Day StarterKit and Exercise Files

### Exercise 1
Type the following where your project was installed:

    php core/console --starterkit --suggestions
    // when prompted choose 'exercise1start'
    php core/console --generate
    php core/console --server --quiet & php core/console --watch

### Exercise 2
If you would like a clean start with exercise two type the following where your project was installed:

    php core/console --starterkit --suggestions
    // when prompted choose 'exercise2start' and to replace source
    php core/console --generate
    php core/console --server --quiet & php core/console --watch
    
### Exercise 3 (Complete)
If you would like a clean start with exercise three type the following where your project was installed:

    php core/console --starterkit --suggestions
    // when prompted choose 'complete' and to replace source
    php core/console --generate
    php core/console --server --quiet & php core/console --watch

## Updating Pattern Lab

To update Pattern Lab please make sure you've [installed Composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx). From the root of your project you can then run:

    php composer update

## Helpful Commands

These are some helpful commands you can use on the command line for working with Pattern Lab.

### List all of the available commands

To list all available commands type:

    php core/console --help

To list the options for a particular command type:

    php core/console --help --[command]

### Generate Pattern Lab

To generate the front-end for Pattern Lab type:

    php core/console --generate

### Watch for changes and re-generate Pattern Lab

To watch for changes and re-generate the front-end for Pattern Lab type:

    php core/console --watch

### Start a server to view Pattern Lab

You can use PHP's built-in web server to review your Pattern Lab project in a browser. In a seperate window type:

    php core/console --server

Then open [http://localhost:8080](http://localhost:8080) in your browser.

### Install a StarterKit

To install a near-empty StarterKit as a starting point for your project type:

    php core/console --starterkit --init

To install a specific StarterKit from GitHub type:

    php core/console --starterkit --install <starterkit-vendor/starterkit-name>
    
To view the suggested StarterKits for your edition and install one type:

    php core/console --starterkit --suggestions
