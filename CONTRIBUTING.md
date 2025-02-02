## Contributing

The files to modify are under the `src` folder. `src/assets` are JavaScript files written in es6 that get compiled
through babel into `lib/sitemapper.js`.

### Pre-requisite

Make sure to perform these steps before building: 

Check babel if installed
```bash
babel --version
```
Install using this command
```bash
npm install -g babel-cli
```

Check if typescript is installed
```bash
tsc --version
```
Install using this command
```bash
npm install -g typescript
```
Check if Mocha is installed
```bash
mocha --version
```
Install using this command:
```bash
npm install -g mocha
```

Install is-url: 
```bash
npm install -g is-url
```

Run this command: 
```bash
npm i --save-dev @types/jest
```

### Build

To build the `lib` directory with the compiled assets use this command
```bash
npm run build
```
This uses [Babel](http://babeljs.io/) to compile the files. Make sure to run `npm run build` before submitting a pull request.

# Run examples/index.js
npm start
```

### Testing

Make sure all tests pass using
```bash
npm test
```
This will run [Mocha](https://mochajs.org/) for testing and [ESLint](http://eslint.org/) for style guides
The tests run will be `mocha` and `eslint`.
Make sure your style follows the style guide in `.eslintrc`

### Style Guide

To see if your code passes the linter use
```bash
npm run lint
```

### Pull Requests

Be sure to build your code with `npm run build` before making a pull request.
Pull requests will use [TravisCI](https://travis-ci.com/) to run your code.
If you would like to be an owner of this repository to approve pull requests, create an issue that I will review.

### Structure

```
lib/
  assets/
    sitemapper.js
  examples/
    index.js
  tests/
    test.js
src/
  assets/
    sitemapper.js
  examples/
    index.js
  tests/
    test.js
````
