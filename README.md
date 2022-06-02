<img align="center" src="./assets/01-header.png">

<br>

<div align="center">

[Treehouse](https://teamtreehouse.com) - [Blog](https://teamtreehouse.com/blog) - [Twitter](https://twitter.com/treehouse) - [Youtube](https://www.youtube.com/gotreehouse) - [Instagram](https://www.instagram.com/teamtreehouse/) - [Linkedin](https://www.linkedin.com/school/treehouse-island-inc-/)

</div>

# <p align="center">Gulpfile Setup using gulp.js</p>

<br><br>

## **Introduction to gulp.js**

What is gulp? According to their homepage ([gulpjs.com](https://www.gulpjs.com)), it's _a toolkit to automate & enhance your workflow._ What exactly does that mean? Well, for medium to large sized projects you may want to have a folder with all your styles and scripts minified. This can significantly decrease file sizes and is usually best practice when deploying your app. Gulp can do all the hard work for you. It can throw all your final code into a new folder, minify it, even adding extra things to your make your code even better!

I'm going to take you through setting up a basic gulpfile for your own projects and apps. Once we're done, you should have a clear understanding of how gulp works as well as adding even more features to making your gulpfile even more powerful. Let's get started!

### - Prerequisites

To get the most out of this content, it is advised you have a decent understanding of JavaScript as well as a basic understanding of Node.js and npm. If those topics aren't familiar to you or need a refresher, I've provided some links to Treehouse resources blow 👇🏼

1. [JavaScript Basics](https://teamtreehouse.com/library/javascript-basics)
2. [Node.js Basics](https://teamtreehouse.com/library/nodejs-basics-3)
3. [npm Basics](https://teamtreehouse.com/library/npm-basics-2)

<br>

## Getting Started

I encourage you to read through this README.md file and follow along in your own text editor. If you get stuck, you can take a look at the code in this repository. Ready? Let's go! 🚀

<br>

### Initializing the project

On your desktop (or wherever you'd like to store your project), create a new folder. Let's call it `gulpfile-setup`. Once done, open it up in your text editor. Next we'll need to open up the terminal. Make sure you're inside your new project folder. To get things started, we'll need a `package.json` file. We can set that up pretty easily by running `npm init -y`

<br> 
<img align="center" src="./assets/02-npm-init.png">

<br>

You'll notice a `package.json` file is automatically generated for you. Don't worry about it's contents as that isn't too important for this guide. It should look pretty similar to this:

<br>
<img align="center" src="./assets/03-package.png">

<br>

Next, we'll need to install some packages for gulp via npm. This will create a `node_modules` folder inside our project folder. Generally, this folder will have lots of packages inside and is usually not a good idea to be tracked with git. So let's first create a `.gitignore` file inside our project.Once created, we can ignore our node modules folder by writing `./node_modules`

<br>
<img align="center" src="./assets/04-node-modules.png">
⭐ Pro tip: You may or may not be using git to track this project but it's always good practice to do this anyway.

<br>

Next, we'll want to install the npm packages we'll need to work with gulp. For this basic gulp setup, we'll be installing a package to compile our css to scss, add auto-prefixers to our compiled css, minify our css, and minify our javascrip. So here are the packages we'll be installing. I'll link the individual packages to their documentation on the gulp.js website:

<br>

1. gulp
2. [gulp-sass](https://www.npmjs.com/package/gulp-sass)
3. [sass](https://www.npmjs.com/package/sass)
4. gulp-clean-css (minifies our css) -
5. gulp-autoprefixer (adds auto-prefixers to our css) -
6. gulp-terser (minifies our javascript) -
