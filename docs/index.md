# Home

## Introduction
here is Introduction

## Outline  

* ### [Components](./Components_Home.md) 

* ### [Methods](./Methods_Home.md)

* ### [Routes](./Routes.md)

### Installation & Environment
[![](https://img.shields.io/badge/npm-v8.12.2-brightgreen)](https://shields.io)  [![](https://img.shields.io/badge/node-v16.15.1-orange)](https://shields.io)
### How it run on localhost:
**1. Clone the project to local**

```
git clone git@github.com:ZhihaoWan/Integ_CRC.git
```
**2. Run `npm install`** 
**3. Run `npm start`** 

----
Website Link: [voyages3-react page](https://voyages3-react.crc.rice.edu)

##### Deploy Manually

  Since we found `package-lock.json` will casuse `OCI` deployment process error, we summarized a workflow to avoid that:

1. use nvm (Node version management) tool make sure node -version is "correct <same version everybody>"
 
    1.1: Check your local node version by `node -v` and npm version with `npm -v`
 
    1.2: Make sure the versions are same as top of this README

2. Delete `node_modules` && `package-lock.json` file
3. run `npm install`
4. Delete `node_modules` 
5. run `npm ci` 
6. Locally test (run `npm start`, if all functions gose well, Prefect!)
7. If funciton on local serve is perfect then push & merge


##### Deploy with Makefile
Quick Way with Makefile

1. Make sure you are in the `main` branch
2. if you use this make file first time, just run `chmod u+x Makefile`
3. run `make deploy`, util see `"deploy successfully"`
