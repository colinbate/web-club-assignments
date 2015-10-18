# Intro to Node.js / NPM

This assignment aims to introduce you to the world of server-side JavaScript using Node.js and the Node Package Manager (NPM).

It is difficult to do any serious web development these days without running into Node.js in some way. Even if you are creating and server-side resources in your projects, many of the web-focused build tools like Grunt, Gulp and others use Node.js to run on your machines.

## Assignment

1. If it isn't there already, install a recent version of Node.js on your machine.
2. Create a new project on your machine which comprises the following:
    * A valid `package.config` file
    * Runs a web server which displays your name and its own version number at the root URL.
    * Web server should have a `/ping` route which displays a page listing any query string parameters passed to it. This page should be generated on the server.
    * At least one node module in your `dependencies` should be referenced (although it is possible to complete the above requirements without doing so).
    * At least one item in your `devDependencies` which is used to perform some build operation. You can use `grunt`, `gulp`, `brunch`, `broccoli`, `npm run` scripts, or whatever other build tool you like as it is cross-platform. For this simple assignment, it might just be something to run JSHint on your server code.
    * A `README.md` file sould be included with instructions on how to run your server locally including any build tasks.
3. Host your code somewhere accessible like Bitbucket or GitHub.
4. Host your running server somewhere online. [OpenShift][os] seems to offer a free option which allows for three different processes to be run.
5. Post the code URL and the server URL into the assignment channel.

[os]: https://www.openshift.com/products/pricing/plan-comparison
