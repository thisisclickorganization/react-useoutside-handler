# react-useoutside-handler
> This React hook allows you to detect clicks outside of a specified element.


## Installation

> Install using [NPM](https://www.npmjs.com/):

```sh
npm install react-click-outside-hook --save
```


> Install using [Yarn](https://yarnpkg.com):

```sh
yarn add react-click-outside-hook
```


## Usage

> Import:

```jsx
import useOutside from 'react-useoutside-handler';
```

> useOutside:

```jsx
useOutside(ref, handler);
```

> Example:

```jsx
import React, { useRef } from 'react';
import useOutside from 'react-useoutside-handler';

const HelloWorldComponent = () => {
  const refHelloWorldElement = useRef(null);

  useOutside(refHelloWorldElement, () => alert('You clicked outside of Hello world element'));

  return (
    <div>
      <div ref={refHelloWorldElement} className="hello-world-element">Hello World</div>
    </div>
  );
};
```
