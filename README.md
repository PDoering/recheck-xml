# ![recheck logo](https://user-images.githubusercontent.com/1871610/41766965-b69d46a2-7608-11e8-97b4-c6b0f047d455.png) for XML

[![Build Status](https://travis-ci.com/retest/recheck-xml.svg?branch=master)](https://travis-ci.com/retest/recheck-xml)
[![Latest recheck-xml on Maven Central](https://maven-badges.herokuapp.com/maven-central/de.retest/recheck-xml/badge.svg?style=flat)](https://mvnrepository.com/artifact/de.retest/recheck-xml)
[![license](https://img.shields.io/badge/license-AGPL-brightgreen.svg)](https://github.com/retest/recheck-xml/blob/master/LICENSE)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg)](https://github.com/retest/recheck-xml/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
[![code with hearth by retest](https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%99%A5%20by-retest-C1D82F.svg)](https://retest.de/en/)

[recheck](https://github.com/retest/recheck) for XML. Replace manual asserts and check everything at once.


## Features

* Easy creation and maintenance of checks for XML.
* Semantic comparison of contents.
* Easily ignore formatting, volatile elements, attributes or sections.
* One-click maintenance to update tests with intended changes.
* No unexpected changes go unnoticed.


## Advantages

Instead of manually defining individual aspects that you want to check, check everything at once. So instead of writing lots of `assert`-statements (and still not have complete checks), write a single `re.check`. This saves a lot of effort when creating the tests. And makes sure to not [miss unexpected changes](https://hackernoon.com/assertions-considered-harmful-d3770d818054).

And even better: using the [retest GUI](https://retest.de/en/) (or the soon to come open source CLI), you can easily accept those changes with a single click (patent pending). This also saves a lot of time during maintenance. Any regular changing aspects or elements can easily be ignored.


## Setup

Download recheck-xml here on [GitHub](https://github.com/retest/recheck-xml/releases/) or add it as dependency through [Maven Central](https://search.maven.org/search?q=g:de.retest%20a:recheck-xml):

* group ID: `de.retest`
* artifact ID: `recheck-xml`
* version: [![Latest recheck-xml on Maven Central](https://maven-badges.herokuapp.com/maven-central/de.retest/recheck-xml/badge.svg?style=flat)](https://mvnrepository.com/artifact/de.retest/recheck-xml)

### Prerequisites

Currently available as a Java API with support for JUnit 4. 

Add any logging facility you want, that is compatible with [SLF4j](https://www.slf4j.org/).


## Building

To build this project locally, you have to skip JAR signing.

For normal builds use:

```
mvn deploy -Dgpg.skip=true
```

For making releases use:

```
mvn release:prepare -Darguments="-Dgpg.skip=true"
```


## License

This project is licensed under the [AGPL license](LICENSE).

