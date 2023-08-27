# Overview

This example application helps understand concepts of both Declarative and Scripted pipelines. 

Pipeline will build a Docker image for a node application which displays `Hello world` message. 

Once Docker image is build Pipeline will test image and assert expected value. 

If test step is successful, it will upload Docker image to Docker hub - https://hub.docker.com/r/devcwm/node-application

There are two functional pipelines:
* Jenkinsfile-declarative
* Jenkinslfile-scripted

Both pipelines try to use any many options as possible to be near real-world pipelines. 

These pipelines are good starting point to have your initial pipelines setup.

Note - pipeline sometimes uses `label` to select docker agents. Feel free to chagne it accordinly or replace it with `any` if you don't have agents setup yet.