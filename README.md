# AWS & DevOps: Heroku Example App

This repo contains an example app for learning about to Heroku deployment process.

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

4. Run `npm install express --save`.

## References

* [Deploying Node.js Apps on Heroku](https://devcenter.heroku.com/articles/deploying-nodejs)
* [Process Types and the Procfile](https://devcenter.heroku.com/articles/procfile)
* [npm-scripts](https://docs.npmjs.com/misc/scripts)
