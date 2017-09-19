# What it is

Typescript express seed is a very crude solution to start a typescript project, using the oh-so-famous express Javascript framework

# What it contains

* Basic folder layout
* A production and a development configuration
* Basic linting rules to keep code clear
* Basic typings needed for best autocompletion with express
* In development mode:
    * a command that keeps a server updated (through nodemon) and your tests running (through mocha)
    * configuration to be able to debug inside vscode

# How to use

## Initialization 
Clone the repository:
```
git clone https://github.com/fhemery/typescript-express-seed.git
```

In the created folder, reinit your own git repository, changing name of package in the meantime:
```
rm -rf .git
git init
git add .
git commit -m "Init"
```

## Working

### Development
```
npm run dev
```
Transpiles, lints, launches a nodemon (port 3000 unless changed) and the unit tests, and watches for any change afterwards.

```
npm test
```
Will launch the transpiling + the unit tests, in watch mode

### Production
```
npm build
```
Just outputs everything in dist folder to be deployed.

### Heroku bonus
Deployment is seamless in Heroku thanks to the postinstall step that will perform the compiling on the fly.

## Contributes
Ideas? Updates? Feel free to let an issue or a comment!