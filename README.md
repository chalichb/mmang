# mmang

HMHCO MMA replacement based on dadi cdn

## Overview

This is a POC which presents the Dadi CDN nodeJS server as a replacement
for the current HMH MMA solution.

The Dadi CDN server could be configured as a remote mirror. In this mode,
any request for image or asset if not found, is retrieved from a remote server.
This would allow for a lazy loading of the CDN resources.

## Documentation

https://docs.dadi.cloud/
https://docs.dadi.cloud/cdn/3.2#installation

## Install

`npm i`

## Configuration

The configuration files are located in the ./config directory.
The `config.development.json` file is setup to front the local media server

## Start

`npm start`

The server is started on port 8080

## Use

Access any media server url and observe that a request is made to the media
server to fetch and cache the image.
