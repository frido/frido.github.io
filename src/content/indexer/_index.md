---
title: "Indexer"
date: 2018-01-28T22:01:36+01:00
anchor: "indexer"
weight: 20
---

Indexer analyzes `pom.xml` files found in the maven repo. The Github API is used to gather additional data via the `GraphQL` data query language. The collected data are saved to a `Mongo` database hosted on `mLab`.

### Development

The project is hosted on [`Bitbucket`](https://bitbucket.org/frido/mvnrepo-indexer/). ~~`IntelliJ`~~ ~~`Eclipse Oxygen`~~ `Visual Studio Code` was used as IDE. Indexer is written in `Java10` and built with ~~`Ant`~~ ~~`Maven`~~ `Gradle`. Sometimes I use `Cloud9` or `Codenvy` virtual machine for small updates.

#### Libraries

* *logging*: `slf4j`+`logback` vs ~~`log4j`~~
* *http clients*: `Jersey` vs `Appache` vs `Spring`
* *json*: BSON
* xml: XML
* *mongo*: `MongoDB` vs ~~`Morphia`~~ vs ~~`Mongoose`~~ vs ~~`MongoJack`~~ 
* *testing*: `jUnit4` vs ~~`jUnit5`~~

### Test

Result of tests is published on `GitHub Pages` in `docs` folder.

#### Test Tools

| Tool | Reports |
| --- | ---|
| JUnit | https://frido.github.io/mvnrepo-indexer/junit/ |
| CheckStyle | https://frido.github.io/mvnrepo-indexer/checkstyle/main.html |
| FindBugs | https://frido.github.io/mvnrepo-indexer/findbugs/ |
| PMD | https://frido.github.io/mvnrepo-indexer/pmd/ |
| JaCoCo | https://frido.github.io/mvnrepo-indexer/jacoco/test/html/ |
| SonarCloud | https://sonarcloud.io/organizations/frido-bitbucket/projects |

### Quality

To check code quality I use `CodeFactor` and `SonatQube`.

| Tool | Badge |
| --- | --- |
| CodeFactor | [![CodeFactor](https://www.codefactor.io/repository/bitbucket/frido/mvnrepo-indexer/badge)](https://www.codefactor.io/repository/bitbucket/frido/mvnrepo-indexer) |
| SonarQube | ![sonarqube](https://sonarcloud.io/api/project_badges/measure?project=mvnrepo-indexer&metric=alert_status) |

### Documentation

JavaDoc is located on [GitHub Pages](https://frido.github.io/mvnrepo/)

### Deployment

The continuous integration is done by `CircleCI`.

| Tool | Badge |
| --- | --- |
| CircleCI | [![CircleCI](https://circleci.com/bb/frido/mvnrepo-indexer.svg?style=svg)](https://circleci.com/bb/frido/mvnrepo-indexer) |

### Maitenance

TODO: Log File???

### Books

Very usefull books are *Effective Java* and *Clean Code*. TODO: amazon (promoted) link

### Summary

Everything is summarized on `StackShare`.

| Tool | Badge |
| --- | --- |
| StackShare | [![StackShare](https://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](https://stackshare.io/frido/mvnrepo-indexer) |

