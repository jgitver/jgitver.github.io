# jgitver.github.io

[![Build Status](https://travis-ci.org/jgitver/jgitver.github.io.svg?branch=docs)](https://travis-ci.org/jgitver/jgitver.github.io)

This project hosts the source files for the site [https://jgitver.github.io](https://jgitver.github.io)

## Build

builds are performed by [travis-ci](https://travis-ci.org/jgitver/jgitver.github.io) automatically on each push on the `docs` branch.
On success the result of the build is commit back to the `master` branch of this repository and is then accessible at [https://jgitver.github.io](https://jgitver.github.io) via [github pages](https://pages.github.com/). 

## Local build

The easiest way to build and serve this site locally is to use `docker-compose`.

- launch docker images that build and http serve the result: `docker-compose up`
- navigate to [http://localhost:8090](http://localhost:8090)
- when done shutdown the docker images: `docker-compose down`
