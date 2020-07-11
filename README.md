# Project Title

Create a npm package with GitHub

## Getting Started

Profile -> Setttings ->  Developer settings -> Personal access tokens -> Generate new token.

Check this options

```
 repo  Full control of private repositories
  repo:status  Access commit status
  repo_deployment  Access deployment status
  public_repo  Access public repositories
  repo:invite  Access repository invitations
  security_events  Read and write security events
  
  write:packages  
  read:packages   
```

You will see the name and the permisions Name — read:packages, repo, write:packages

### Installing

```
nano ~/.npmrc -> add //npm.pkg.github.com/:_authToken=YOUR TOKEN
```

```
create a node js project -> npm init -y
```

```
// Step 1: Use `publishConfig` option in your package.json
"publishConfig": { "registry": "https://npm.pkg.github.com/" }

// Step 2: Authenticate
$ npm login --registry=https://npm.pkg.github.com
> Username: USERNAME
> Password: TOKEN
> Email: PUBLIC-EMAIL-ADDRESS

// Step 3: Publish
$ npm publish
```

```
{
    "name": "@e2517/github-package-demo",
    "version": "1.0.2",
    "description": "",
    "main": "index.js",
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "keywords": [],
    "author": "",
    "publishConfig": {
        "registry": "https://npm.pkg.github.com/"
    },
    "license": "ISC"
}
```
## React project

```
npm init create-react-app name
```

```
create .npmrc and add -> registry=https://npm.pkg.github.com/e2517
```

```
    "dependencies": {
        "@e2517/github-package-demo": "^1.0.2",
        "@testing-library/jest-dom": "^4.2.4",
        "@testing-library/react": "^9.5.0",
        "@testing-library/user-event": "^7.2.1",
        "react": "^16.13.1",
        "react-dom": "^16.13.1",
        "react-scripts": "3.4.1"
    },
```
```
npm install
```

## Deployment

```
npm start
```

![react-code][]
![react][]

## Built With

* [npm package gihub](https://github.com/E2517/NodeMongoGraphQL/packages) 
* [React project](https://github.com/E2517/react-package-github)
* [react-code]: http://achoweb.es/wp-content/uploads/2020/07/reactcode.png
* [react]: http://achoweb.es/wp-content/uploads/2020/07/react.png

## Authors

* **e2517**


