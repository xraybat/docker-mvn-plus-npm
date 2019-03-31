Docker Maven/Java + Npm/Node
============================

(from https://hub.docker.com/r/mukeshrijhwani/mvn-plus-npm)

A Dockerfile that builds an docker image containing

 - open jdk 8 (latest from Ubuntu 16.04 repos)
 - maven (latest from Ubuntu 16.04 repos)
 - node 6.x (using install instructions from nodejs.org)

Using the pre-built image from dockerhub
==============================

     docker run -it mukeshrijhwani/mvn-plus-npm

Building the image:
===================

To build the image, I run this command:

     docker build -t mukeshrijhwani/mvn-plus-npm .

You should change the `-t` argument to something else
typically: `${your-dockerhub-id}/${some-name-you-choose}`.

Publishing the image to dockerhub:
==================================

After building the image it is pushed to dockerhub like so:

    docker push mukeshrijhwani/mvn-plus-npm

Again, change `mukeshrijhwani` to your own docker-hub-id.
