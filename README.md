# jgitver.github.io

[![Build Status](https://travis-ci.org/jgitver/jgitver.github.io.svg?branch=master)](https://travis-ci.org/jgitver/jgitver.github.io)

here are hosted the source files for the site [https://jgitver.github.io](https://jgitver.github.io)

## Build

builds are performed by [travis-ci](https://travis-ci.org/jgitver/jgitver.github.io) automatically on each push on the `master`.
On success the result of the build is commit back to the `gh-pages` branch of this repository and is then accessible at [https://jgitver.github.io](https://jgitver.github.io). 


## Local build

### windows

```
D:\dev\projects\jgitver.github.io> docker run --rm -it -v %CD%\src:/documents/ asciidoctor/docker-asciidoctor /bin/bash  

$ asciidoctor -D /documents/output *.adoc
```
