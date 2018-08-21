---
title: "Indexer"
date: 2018-01-28T22:01:36+01:00
anchor: "indexer"
weight: 20
---

Indexer analyzes `pom.xml` files found in the maven repo. The Github API is used to gather additional data via the `GraphQL` data query language. The collected data are saved to a `Mongo` database hosted on `mLab`.

### Development

The project is hosted on [`Bitbucket`](https://bitbucket.org/frido/mvnrepo-indexer/). ~~`IntelliJ`~~ `Eclipse Photon` and `Visual Studio Code` was used as IDE. Indexer is written in `Java10` and built with ~~`Ant`~~ ~~`Maven`~~ `Gradle`. Sometimes I use `Cloud9` or `Codenvy` virtual machine for small updates.

#### Libraries

* *logging*: `slf4j`+`logback` vs ~~`log4j`~~
* *http clients*: `Jersey` vs ~~`Appache`~~ vs ~~`Spring`~~
* *json*: BSON
* xml: XML
* *mongo*: `MongoDB` vs ~~`Morphia`~~ vs ~~`Mongoose`~~ vs ~~`MongoJack`~~ 
* *testing*: `jUnit4` vs ~~`jUnit5`~~

### Test

Result of tests is published on `GitHub Pages` in `docs` folder.

| Tool | Reports |
| --- | ---|
| JUnit4 | [Reports](https://frido.github.io/mvnrepo-indexer/junit/) |

### Quality

| Tool | Badge |
| --- | --- |
| CheckStyle | [Reports](https://frido.github.io/mvnrepo-indexer/checkstyle/main.html) |
| FindBugs | [Reports](https://frido.github.io/mvnrepo-indexer/findbugs/) |
| PMD | [Reports](https://frido.github.io/mvnrepo-indexer/pmd/) |
| JaCoCo | [Reports](https://frido.github.io/mvnrepo-indexer/jacoco/test/html/) |
| CodeFactor | [![CodeFactor](https://www.codefactor.io/repository/bitbucket/frido/mvnrepo-indexer/badge)](https://www.codefactor.io/repository/bitbucket/frido/mvnrepo-indexer) |
| SonarCloud | ![sonarqube](https://sonarcloud.io/api/project_badges/measure?project=mvnrepo-indexer&metric=alert_status) |
| Codacy | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f32f5fe80218464a935fce3b231806af)](https://www.codacy.com/project/frido/mvnrepo-indexer/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=frido/mvnrepo-indexer&amp;utm_campaign=Badge_Grade_Dashboard) |

### Documentation

JavaDoc is located on [GitHub Pages](https://frido.github.io/mvnrepo-indexer/javadoc/)

### Deployment

The continuous integration is done by ~~`CircleCI`~~ `Buddy`.

| Tool | Badge |
| --- | --- |
| Buddy | [![buddy pipeline](https://app.buddy.works/fridrichpeter/mvnrepo-indexer-1/pipelines/pipeline/148732/badge.svg?token=7e655371adbe49225d540916417d681bfffc656638c4af50ee9f6b6c2e1801bd "buddy pipeline")](https://app.buddy.works/fridrichpeter/mvnrepo-indexer-1/pipelines/pipeline/148732) |

### Books

Very usefull books are [***Effective Java***](https://www.amazon.com/Effective-Java-3rd-Joshua-Bloch/dp/0134685997) and [***Clean Code***](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882).

### Summary

Everything is summarized on `StackShare`.

| Tool | Badge |
| --- | --- |
| StackShare | [![StackShare](https://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](https://stackshare.io/frido/mvnrepo-indexer) |

