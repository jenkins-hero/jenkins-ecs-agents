[![CI](https://github.com/tkgregory/jenkins-ecs-agents/actions/workflows/gradle.yml/badge.svg)](https://github.com/tkgregory/jenkins-ecs-agents/actions/workflows/gradle.yml)

## Overview

Creates Jenkins Docker image for use in article *[Using Jenkins Configuration as Code to setup AWS slave agents automatically](https://tomgregory.com/using-jenkins-configuration-as-code-to-setup-aws-slave-agents-automatically/)*.

## Running

Build image and run Jenkins locally with `./gradlew docker dockerRun`.

Access Jenkins at http://localhost:8080 and use the `JENKINS_USERNAME` and `JENKINS_PASSWORD` credentials defined in [build.gradle](build.gradle)

## Deploying

Push image to Docker Hub with `./gradlew docker dockerTagLatest dockerPushLatest`.