# Udagram Simple Frontend

Udagram is a simple cloud application developed awhich allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.



## Getting Setup

> _tip_: this frontend is designed to work with [The RestAPI User API Backend](https://github.com/pai-amit/udagram-user-api) and [The RestAPI Feed API Backend](https://github.com/pai-amit/udagram-feed-api). It is recommended you stand up the backend first, test using Postman, and then the frontend should integrate.

In addition, the deployments are done using [Kubernetes](https://github.com/pai-amit/udagram-k8s-deployments)

### Installing Node and NPM
This project depends on Nodejs and Node Package Manager (NPM). Before continuing, you must download and install Node (NPM is included) from [https://nodejs.com/en/download](https://nodejs.org/en/download/).

### Installing Ionic Cli
The Ionic Command Line Interface is required to serve and build the frontend. Instructions for installing the CLI can be found in the [Ionic Framework Docs](https://ionicframework.com/docs/installation/cli).

### Installing project dependencies

This project uses NPM to manage software dependencies. NPM Relies on the package.json file located in the root of this repository. After cloning, open your terminal and run:
```bash
npm install
```
>_tip_: **npm i** is shorthand for **npm install**

### Configure The Backend Endpoint
Ionic uses enviornment files located in `./src/enviornments/enviornment.*.ts` to load configuration variables at runtime. By default `environment.ts` is used for development and `enviornment.prod.ts` is used for produciton. The `apiHost` variable should be set to your server url either locally or in the cloud.

***
### Running the Development Server
Ionic CLI provides an easy to use development server to run and autoreload the frontend. This allows you to make quick changes and see them in real time in your browser. To run the development server, open terminal and run:

```bash
ionic serve
```
