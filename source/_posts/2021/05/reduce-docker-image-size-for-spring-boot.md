title: Reduce Docker Image Size For Spring Boot
toc: true
cover: /gallery/covers/1.png
categories:
- Docker
- Spring Boot
tags:
- docker
- spring-boot
- jlink
- graalvm
---

How to reduce size of docker for spring boot application? In this blog post, I'm going to show you the different approach to building small size having docker image for spring boot.

<!-- more -->

## Background

Large docker images will take long time to build, upload, download and share between the team and cloud providers. To speedup the development and deployment it's worth to reduce docker image size as much as possible. In this article, I will discuss the possible ways to reduce docker image size for spring boot application.

## Using jlink

In JDK 9 the module system was introduced where java sdk library divided into modules and also provides jlink tool to assemble jdk with needed modules only.
