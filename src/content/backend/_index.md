---
title: "Backend"
date: 2018-01-28T22:01:36+01:00
anchor: "backend"
weight: 30
---

Backend is RESTful service. It provide access to data stored in `Mongo` database hosted on `mLab`.

### Development 

Project is hosted on [`Bitbucket`](https://bitbucket.org/frido/mvnrepo-backend/src/master/).
I used `InteliJ` to coding in `Kotlin` and to build with `Gradle`. Backend provides REST API what built on `Spring Boot`.
~~I monitor service via Actuator endpoints.~~

#### Libraries

* `spring boot`
* `swagger2`
* *json*: `Jackson`
* *mongo*: `MongoDB` vs ~~`Morphia`~~ vs ~~`Mongoose`~~ vs ~~`MongoJack`~~

*NOTE*: `JAX-RS` or `Jersey` are alternatives for `Spring-Web`. But why use something else when you already have Spring in your classpath.

### Tests

TODO: JUnit5 for example

### Quality

Are there any static code analysis tools for Kotlin?

### Documentation

TODO: https://github.com/Kotlin/dokka

### Deployment

`Bitbucket` provides [`Pipelines`](https://bitbucket.org/frido/mvnrepo-backend/addon/pipelines/home#!/) as a tool for CI.
`Buddy` pipeline is triggered on git push action and it deploys the application.

Application is deployed on [`Heroku`](https://mvnrepo-backend.herokuapp.com/)

You can try REST via [`Swagger`](https://mvnrepo-backend.herokuapp.com/swagger-ui.html).

*NOTE: Disadvantagve of free Dyno on Heroku is that it get asleep after 30 minutes of inactivity. I dont believe backend has enought traffic to be still alive. So I configured `Buddy` pipeline to make request to Backend every 15 minutes. 1000 free dynos hours per month should be enought to keep Backend alive all month.*

| Tool | Badge |
| ---  | ---   |
| Buddy | [![buddy pipeline](https://app.buddy.works/fridrichpeter/mvnrepo-backend/pipelines/pipeline/128730/badge.svg?token=7e655371adbe49225d540916417d681bfffc656638c4af50ee9f6b6c2e1801bd "buddy pipeline")](https://app.buddy.works/fridrichpeter/mvnrepo-backend/pipelines/pipeline/128730) |

### Maitenance

It is hard to check logs directly on Heroku, so `LogEntries` integration was implemented.

### Books

I recomend to reading the book [***Spring Boot in Action***](https://www.amazon.com/Spring-Boot-Action-Craig-Walls/dp/1617292540).

### Summary

For more info see `StackShare`

| Tool | Badge |
| ---  | ---   |
| StackShare | [![StackShare](https://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](https://stackshare.io/frido/mvnrepo-backend) |
