# jgitver.github.io

[![Build Status](https://travis-ci.org/jgitver/jgitver.github.io.svg?branch=docs)](https://travis-ci.org/jgitver/jgitver.github.io)

here are hosted the source files for the site [https://jgitver.github.io](https://jgitver.github.io)

## Build

builds are performed by [travis-ci](https://travis-ci.org/jgitver/jgitver.github.io) automatically on each push on the `docs`.
On success the result of the build is commit back to the `master` branch of this repository and is then accessible at [https://jgitver.github.io](https://jgitver.github.io). 


## Local build

### windows

launch a docker image to compile asciidoctor files
```
docker run --rm -it -v %CD%\src:/documents/ asciidoctor/docker-asciidoctor /bin/bash  
```

```
rm -rf output && mkdir output 
watch -n 10 "cp -R images/ output/ && asciidoctor -D /documents/output index.adoc"
```
