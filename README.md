# AWS & DevOps: Heroku Example App

This repository contains an example application for learning about the Heroku application deployment process.

## Procedure

1. Use npm to initialize create the `package.json` file and initialize the project.

   ```
   cd node-example
   npm init
   ```

2. Specify the Node.js version to use by adding the following to `package.json`:

   ```
   "engines": {
      "node": "8.9.1"
   },
   ```

   This will be used by Heroku to select the appropriate version of Node.js to run your application.

3. Set up `.gitignore` for Node.js using the [Node.gitignore](https://github.com/github/gitignore/blob/master/Node.gitignore) file provided by GitHub. Additional `.gitignore` templates are available in the [github/gitignore](https://github.com/github/gitignore) repository.

4. Run `express --view=ejs aws-devops-heroku-example` to generate an Express project.

5. Update the express project. Move `./www/bin` to `./app.js` and change the line `var app = require("../app")` to `var app = require("./app")`.

6. Run `heroko login` to login to Heroku and `heroku create` to create a Heroku application.

7. Deploy to Heroku with `git push heroku master`.

## References

* [Deploying Node.js Apps on Heroku](https://devcenter.heroku.com/articles/deploying-nodejs)
* [Process Types and the Procfile](https://devcenter.heroku.com/articles/procfile)
* [npm-scripts](https://docs.npmjs.com/misc/scripts)
