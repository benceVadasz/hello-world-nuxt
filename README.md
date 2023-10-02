## Dependency Management

Kinsta automatically installs dependencies defined in your `package.json` file during the deployment process.

## Web Server Setup

### Port

Kinsta automatically sets the `PORT` environment variable. You should **not** define it yourself and you should **not** hard-code it into the application.

### Start Command

When deploying an application, Kinsta automatically creates a web process with `npm start` as the entry point. Make sure to use this command to run your server.

## Deployment Lifecycle

Whenever a deployment is initiated (through creating an application or re-deploying due to an incoming commit) the `npm build` command is run, followed by the `npm start` command.

## What is NuxtJS
NuxtJS is an open-source web development framework that allows you to build server-side rendered Vue.js applications and static sites. More information is available on the [Nuxtjs.org](https://nuxtjs.org/) website.
