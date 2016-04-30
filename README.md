# hello_webpack
Learning Webpack basics.

[![Webpack](https://webpack.github.io/assets/what-is-webpack.png)](https://webpack.github.io/)

Summary
-------
The purpose of this repo is to learn Webpack fundamentals.   In this tutorial, we will go from zero to a very basic file-based web page with basic styling.  Ultimately, the purpose is to build very sophisticated web apps using Angular 2, Webpack, Bootstrap, Nginx and Golang.   

Development Environment
-----------------------

Here's my development environment:
>  * Ubuntu 14.04
>  * npm 2.11.3
>  * various npm packages specified later

Let's get started!

Create an app folder
---------------------
From a shell prompt (I use bash), create a new folder:
~~~bash
  mkdir hello-webpack
~~~
Then cd into that folder:
~~~bash
  cd hello-webpack
~~~
Verify npm is properly installed
--------------------------------
~~~bash
  npm -v
~~~
If npm is installed properly you will see output like this:
~~~bash
  mthomas@ubuntu:~/apps/hello-webpack$ npm -v
  2.11.3
~~~
If you get an error, check the [NPM](https://www.npmjs.com/) documentation and installation guide for help.
Install Webpack
---------------
When installing Webpack (or any other npm package), you can install globally or locally.  Installing npm packages locally means that packages are installed only in the current project folder, hello-webpack in this case, and are not intended for other apps.  **__I recommend installing npm packages locally as it gives you the freedom to use different versions of packages in different projects.__**

Now let's install Webpack in our local project:
~~~bash
  mthomas@ubuntu:~/apps/hello-webpack$ npm install webpack --save-dev
~~~

~~~bash
mthomas@ubuntu:~/apps/hello-webpack$ npm install webpack --save-dev
npm WARN optional dep failed, continuing fsevents@1.0.12
webpack@1.13.0 node_modules/webpack
├── interpret@0.6.6
├── tapable@0.1.10
├── clone@1.0.2
├── supports-color@3.1.2 (has-flag@1.0.0)
├── async@1.5.2
├── loader-utils@0.2.14 (object-assign@4.0.1, big.js@3.1.3, json5@0.5.0, emojis-list@1.0.1)
├── enhanced-resolve@0.9.1 (graceful-fs@4.1.3, memory-fs@0.2.0)
├── mkdirp@0.5.1 (minimist@0.0.8)
├── optimist@0.6.1 (wordwrap@0.0.3, minimist@0.0.10)
├── acorn@3.1.0
├── memory-fs@0.3.0 (errno@0.1.4, readable-stream@2.1.2)
├── webpack-core@0.6.8 (source-list-map@0.1.6, source-map@0.4.4)
├── watchpack@0.2.9 (graceful-fs@4.1.3, async@0.9.2, chokidar@1.4.3)
├── uglify-js@2.6.2 (uglify-to-browserify@1.0.2, async@0.2.10, source-map@0.5.5, yargs@3.10.0)
└── node-libs-browser@0.5.3 (https-browserify@0.0.0, tty-browserify@0.0.0, constants-browserify@0.0.1, path-browserify@0.0.0, os-browserify@0.1.2, string_decoder@0.10.31, process@0.11.2, punycode@1.4.1, querystring-es3@0.2.1, assert@1.3.0, timers-browserify@1.4.2, domain-browser@1.1.7, events@1.1.0, vm-browserify@0.0.4, util@0.10.3, stream-browserify@1.0.0, console-browserify@1.1.0, http-browserify@1.7.0, readable-stream@1.1.14, url@0.10.3, buffer@3.6.0, browserify-zlib@0.1.4, crypto-browserify@3.2.8)
~~~
