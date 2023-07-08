# react-typescript-package

sample react typescript package


----

# Development

## Clone:

```bash
git clone https://github.com/jsh1400/react-typescript-package.git
```

## instalation:

```bash
cd react-typescript-package
npm i
npm start
```



# Publish React Typescript Package

- check package json <package_name>  
- change package json <version>  
- run build command

```bash
npm run build

```


## publish package in local

```bash
npm pack

```


## publish package in npmjs.org

```bash
npm publish

```

## remove package from npmjs.org

```bash
npm unpublish <package_name>@<version>  

```


----

# Use React Typescript Package

## Installation:

```bash
npm install <package_name> --save-dev
```

or

```bash
yarn add -D <package_name>
```

## Usage :

Add `MyCounter` to your component:

```js
import React from 'react'
import ReactDOM from 'react-dom/client'
import { MyCounter } from '<package_name>'

const root = ReactDOM.createRoot(document.getElementById('root') as HTMLElement)
root.render(
    <React.StrictMode>
        <div>
            <h2>Default counter</h2>
            <MyCounter />
        </div>
        <hr />
        <div>
            <h2>Counter with predefined value</h2>
            <MyCounter value={5} />
        </div>
    </React.StrictMode>,
)

```