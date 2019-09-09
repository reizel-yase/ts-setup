# Simple Typescript Setup

# Pre-requisites
* Node JS
* Typescript

# Installation
* Create an empty folder
* In command prompt, go to that folder directory
* Run `npm i typescript --save-dev`
* Create a `src` and `dist` folder in the folder's root
* Run `tsc --init`
> To create and initialise a `tsconfig.json` file that will contain typescript compilation configuration)
* Update the `tsconfig.json` file to be the same as the following:
  ```tsconfig.json
  {
    "compilerOptions": {
      "allowSyntheticDefaultImports": true,
      "jsx": "react",
      "module": "commonjs",
      "noImplicitAny": false,
      "outDir": "./dist/",
      "preserveConstEnums": true,
      "removeComments": true,
      "sourceMap": true,
      "target": "es2015",
      "lib": [
        "es5",
        "es6",
        "dom"
      ]
    },
    "include": [
      "./src/**/*"
    ]
  }
  ```
* Create a file under `/src` folder, say `index.ts`
* Inside it, write:
```
const func = () => {
	console.log("Hello World!")
}

func()
```
* Run tsc
