# react-typescript-package

![npm-typescript]


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

# Use React Typescript Package

## Installation:

```bash
npm install react-typescript-package --save-dev
```

or

```bash
yarn add -D react-typescript-package
```

## Usage :

Add `MyCounter` to your component:

```js
import React from 'react'
import ReactDOM from 'react-dom/client'
import { MyCounter } from 'react-typescript-package'

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