Docker Maven/Java + Npm/Node
============================

(from https://hub.docker.com/r/mukeshrijhwani/mvn-plus-npm)

A Dockerfile that builds an docker image containing

 - open jdk 8 (latest from Ubuntu 16.04 repos)
 - maven (latest from Ubuntu 16.04 repos)
 - node 6.x (using install instructions from nodejs.org)

Using the pre-built image from dockerhub
==============================

     docker run -it xraybat/mvn-plus-npm

Building the image:
===================

To build the image, I run this command:

     docker build -t xraybat/mvn-plus-npm .

You should change the `-t` argument to something else
typically: `${your-dockerhub-id}/${some-name-you-choose}`.

Publishing the image to dockerhub:
==================================

After building the image it is pushed to dockerhub like so:

    docker push xraybat/mvn-plus-npm

Again, change `xraybat` to your own docker-hub-id.
