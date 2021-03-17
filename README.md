# **Applabit Hugo**

A Hugo boilerplate for creating websites

Boilerplate for using Hugo as a static site generator and NPM Scripts as your asset pipeline.

Setup uses SCSS and Babel for CSS and JavaScript compiling/transpiling.

# Usage

**Prerequisites**

Install Hugo using Homebrew.

`brew install hugo`

To verify your new install:

`hugo version`

You need to have the latest/LTS node and npm versions installed in order to use Applabit Hugo Boilerplate.

Next step, clone this repository and run:

`npm install`

This will install all packages necessary to run Pigment Hugo and it's tasks.

# **Development**

While developing your website, use:

`npm run dev`

Then visit http://localhost:1313/ to preview your new website. Setup uses built in Hugo server for serving page and live reloading assets.

# **Static build**

To build a static version of the website inside the /public folder, run:

npm run build
See package.json for all tasks.

# **Basic Concepts**

More about Hugo's template language in their documentation here:

https://gohugo.io/templates/overview/

The most useful page there is the one about the available functions:

https://gohugo.io/templates/functions/

For assets that are completely static and don't need to go through the asset pipeline, use the `site/static` folder. Images, font-files, etc, all go there.

Files in the static folder ends up in the web root. So a file called `site/static/`favicon.ico will end up being available as `/favicon.ico` and so on...

The `src/script/app.js` file is the entrypoint and will be built to `/public/app.js`.

You can use ES6 and use both relative imports or import libraries from npm.

Any CSS file directly under the `src/style/` folder will get compiled with to `/public/{filename}.css`. Import statements will be resolved as part of the build.

# **Deployment**

Run

`npm run build`

to get minifed version of website, ready for deploy.

# **Deploying to Netlify**

Push your clone to your own GitHub repository.

[Create a new site on Netlify](https://app.netlify.com/start) and link the repository.

Now Netlify will build and deploy your site whenever you push to git.

You can also use netlify-cli for deploying /public folder.

# **Cvit**

[Cvit site](https://www.cvit-travel.com/)