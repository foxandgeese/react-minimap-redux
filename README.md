- Originally forked from
  [jeremy-carbonne/react-minimap](https://github.com/jeremy-carbonne/react-minimap)

# react-minimap

A minimap for React based on
[jquery-minimap](https://github.com/john-bai/jquery-minimap)

## Demo

[react-minimap](https://jeremy-carbonne.github.io/react-minimap/)

## Installation

`yarn add react-minimap-redux`

## Usage

```js
import Minimap from "react-minimap-redux";
import "react-minimap-redux/dist/react-minimap.css";
```

```html
<Minimap selector=".card">
  <div className="card">
    <h1>Title</h1>
  </div>
  <div className="card">
    <h1>Title 2</h1>
    <div className="card">
      <h1>Titles are never rendered by the Minimap</h1>
    </div>
  </div>
</Minimap>
```

## Configuration

The `Minimap` supports the following props:

| Prop name        | Type    | Default value      | Description                                                                   |
| ---------------- | ------- | ------------------ | ----------------------------------------------------------------------------- |
| selector         | string  | is required        | A css selector for specify what you want to render inside the minimap         |
| className        | string  | ''                 | A className for the minimap component                                         |
| width            | number  | `200`              |                                                                               |
| height           | number  | `200`              |                                                                               |
| keepAspectRatio  | boolean | `false`            |                                                                               |
| childComponent   | any     | Internal Component | Allows customizing how components matched by selector are rendered (optional) |
| onMountCenterOnX | boolean | `false`            |                                                                               |
| onMountCenterOnY | boolean | `false`            |                                                                               |
