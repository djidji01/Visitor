<p align="center">
  <img src="https://static.igorora-project.net/Image/Hoa.svg" alt="Hoa" width="250px" />
</p>

---

<p align="center">
  <a href="https://travis-ci.org/igororaproject/Visitor"><img src="https://img.shields.io/travis/igororaproject/Visitor/master.svg" alt="Build status" /></a>
  <a href="https://coveralls.io/github/igororaproject/Visitor?branch=master"><img src="https://img.shields.io/coveralls/igororaproject/Visitor/master.svg" alt="Code coverage" /></a>
  <a href="https://packagist.org/packages/igorora/visitor"><img src="https://img.shields.io/packagist/dt/igorora/visitor.svg" alt="Packagist" /></a>
  <a href="https://igorora-project.net/LICENSE"><img src="https://img.shields.io/packagist/l/igorora/visitor.svg" alt="License" /></a>
</p>
<p align="center">
  Hoa is a <strong>modular</strong>, <strong>extensible</strong> and
  <strong>structured</strong> set of PHP libraries.<br />
  Moreover, Hoa aims at being a bridge between industrial and research worlds.
</p>

# igorora\Visitor

[![Help on IRC](https://img.shields.io/badge/help-%23igororaproject-ff0066.svg)](https://webchat.freenode.net/?channels=#igororaproject)
[![Help on Gitter](https://img.shields.io/badge/help-gitter-ff0066.svg)](https://gitter.im/igororaproject/central)
[![Documentation](https://img.shields.io/badge/documentation-hack_book-ff0066.svg)](https://central.igorora-project.net/Documentation/Library/Visitor)
[![Board](https://img.shields.io/badge/organisation-board-ff0066.svg)](https://waffle.io/igororaproject/visitor)

This library provides interfaces to apply the visitor pattern.

[Learn more](https://central.igorora-project.net/Documentation/Library/Visitor).

## Installation

With [Composer](https://getcomposer.org/), to include this library into
your dependencies, you need to
require [`igorora/visitor`](https://packagist.org/packages/igorora/visitor):

```sh
$ composer require igorora/visitor '~2.0'
```

For more installation procedures, please read [the Source
page](https://igorora-project.net/Source.html).

## Testing

Before running the test suites, the development dependencies must be installed:

```sh
$ composer install
```

Then, to run all the test suites:

```sh
$ vendor/bin/igorora test:run
```

For more information, please read the [contributor
guide](https://igorora-project.net/Literature/Contributor/Guide.html).

## Quick usage

We propose to explain the basis of this library. We have two entities: an
element to visit and a visitor, for example a node of a tree and a dumper. The
element to visit will implement the `igorora\Visitor\Element` interface and the
visitor will implement the `igorora\Visitor\Visit` interface. The first one will ask
to implement the `accept` method in order to define what data it holds will be
visited. The second one will ask to implement the `visit` method which will
contain the visitor computations. We will find several examples in Hoa
libraries.

## Documentation

The
[hack book of `igorora\Visitor`](https://central.igorora-project.net/Documentation/Library/Visitor)
contains detailed information about how to use this library and how it works.

To generate the documentation locally, execute the following commands:

```sh
$ composer require --dev igorora/devtools
$ vendor/bin/igorora devtools:documentation --open
```

More documentation can be found on the project's website:
[igorora-project.net](https://igorora-project.net/).

## Getting help

There are mainly two ways to get help:

  * On the [`#igororaproject`](https://webchat.freenode.net/?channels=#igororaproject)
    IRC channel,
  * On the forum at [users.igorora-project.net](https://users.igorora-project.net).

## Contribution

Do you want to contribute? Thanks! A detailed [contributor
guide](https://igorora-project.net/Literature/Contributor/Guide.html) explains
everything you need to know.

## License

Hoa is under the New BSD License (BSD-3-Clause). Please, see
[`LICENSE`](https://igorora-project.net/LICENSE) for details.
