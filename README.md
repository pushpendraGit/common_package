# common_package
How to create a npm package

What is npm package?
A npm package means nothing, but a reuseable code available in npm(node package manager).

How you can create your own npm package?

It is as simpple as you writing you code.
suppose you want to create a npm package that will resturn a users github repo list

```
mkdir common_package
```
2. Add package.json file

```
{
  "name": "@pushpendragit/common_package",
  "version": "1.0.0",
  "description": "First NPM package",
  "main": "index.js",
  "scripts": {
    "start": "node index.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [
    "npm",
    "package",
    "How",
    "to",
    "create",
    "npm",
    "package"
  ],
  "author": "Pushpendra Singh",
  "license": "ISC",
  "dependencies": {
    "axios": "^0.20.0"
  }
}

```
<h4>Note:-</h4> Make sure that the name should be in same format @yournpmusername/packagename.

2. Index.js is containing code for genric fn to get git repository.

<h2>How We can Publish NPM package</h2>

1. Login into npm 

```
npm login

```
2. Add you cred

3. Publish package

```
npm publish --access public
```
<h4>Note:-</h4> Make sure --access should me public if you dont have a paid account
