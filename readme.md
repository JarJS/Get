# JarJS
JarJS is a framework to **facilitate** a creation of modules and creation of custom tags to HTML5

## Instalation

* npm
```
$ npm install jarjs@latest
```
* yarn
```
$ yarn add jarjs
```
## Usage

To use the JarJS fist, create a file .ts, it will be the module. In file write:
```
function MyModule(): void {
    console.log("I using JarJS!");
}

globalThis.module("myModule",MyModule);
```
Lets view line per line.

First, we create a function of type void, named "MyModule", this function write in console "I using JarJS!"

After this, we define the module using the Module class, with the first parameter is the name of the module end the second is the initalizator, it is what initalize the module, is this case, write is console.

To get the module create the index.html file and write:
```
globalThis.get("myModule",callback=>{
    callback();
});
```
Ok, this code import the file "jarjs.net.js" and execute a function gamed "get", this function execute the initalizator of the module.

Wait before leave, it is a part of the usage, you want more informations? Entry in my website [JarJS](https://docs.jarjs.com/?page=GetStart)
