# useForceUpdate [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=useForceUpdate%20is%20a%20React%20Hook%20that%20forces%20your%20functional%20component%20to%20re-render!&url=https://www.npmjs.com/package/use-force-update&via=CharlesStover&hashtags=react,reactjs,javascript,typescript,webdev,webdevelopment) [![version](https://img.shields.io/npm/v/use-force-update.svg)](https://www.npmjs.com/package/use-force-update) [![minified size](https://img.shields.io/bundlephobia/min/use-force-update.svg)](https://www.npmjs.com/package/use-force-update) [![minzipped size](https://img.shields.io/bundlephobia/minzip/use-force-update.svg)](https://www.npmjs.com/package/use-force-update) [![downloads](https://img.shields.io/npm/dt/use-force-update.svg)](https://www.npmjs.com/package/use-force-update) [![build](https://api.travis-ci.com/CharlesStover/use-force-update.svg)](https://travis-ci.com/CharlesStover/use-force-update/)

`useForceUpdate` is a React Hook that forces your functional component to
re-render.

`useForceUpdate` does not serve a purpose in and of itself. It is a tiny
package that aims to be integrated into larger hooks, making obsolete any class
functionality that is still reliant on `this.forceUpdate`.

## Install

* `npm install use-force-update` or
* `yarn add use-force-update`

## Use

```JavaScript
import useForceUpdate from 'use-force-update';

const MyButton = () => {

  const forceUpdate = useForceUpdate();

  const handleClick = () => {
    alert('I will re-render now.');
    forceUpdate();
  };

  return <button onClick={handleClick} />;
};
```
