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
~~~bash
  mthomas@ubuntu:~/apps/hello-webpack$ npm install webpack --save-dev
~~~

