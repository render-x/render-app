# render-app

<p>
<a href="https://www.npmjs.com/package/@x.render/render-app" target="__blank"><img src="https://img.shields.io/npm/v/@x.render/render-app" alt="NPM version" /></a>

<a href="https://www.npmjs.com/package/@x.render/render-app" target="__blank"><img src="https://img.shields.io/npm/dm/%40x.render%2Frender-app" alt="NPM Downloads" /></a>

</p>

[中文文档](./README.zh.md)

## Introduce

Provides commonly used hooks and utility functions for React.

## Usage

```sh
npm i @x.render/render-app -S
```

## Hooks

Many commonly used hooks are provided in render-app

### usePageShow

usePageShow is used to execute related callback functions when the page is visible and invisible.

```javascript
import { usePageShow } from "@x.render/render-app";

const Demo = () => {
  const pageShow = () => {
    console.log("Page not visible");
  };

  const pageHidden = () => {
    console.log("Page  visible");
  };
  usePageShow(pageShow, pageHidden);
  return <div>demo</div>;
};
export default Demo;
```

the parameters executed by usePageShow are not required.
