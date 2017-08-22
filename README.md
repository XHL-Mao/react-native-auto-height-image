# react-native-auto-height-image

Initialized by [vivaxy/gt-npm-package](https://github.com/vivaxy/gt-npm-package)

[![NPM Version](http://img.shields.io/npm/v/react-native-auto-height-image.svg?style=flat-square)](https://www.npmjs.com/package/react-native-auto-height-image)
[![NPM Downloads](https://img.shields.io/npm/dt/react-native-auto-height-image.svg?style=flat-square)](https://www.npmjs.com/package/react-native-auto-height-image)
[![MIT License](https://img.shields.io/npm/l/react-native-auto-height-image.svg?style=flat-square)](./LICENSE)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square)](https://conventionalcommits.org)

This component provides you a simple way to load a remote image and automatically set `Image` height to the image dimension which fits the provided width.

ReactNative `Image` component needs users to set both `width` and `height` props.

## Installation

`yarn add react-native-auto-height-image`

`npm install react-native-auto-height-image`

## Usage

```js
import React, { Component } from 'react';
import AutoHeightImage from 'react-native-auto-height-image';

export default class Demo extends Component {
    render() {
        return (
            <AutoHeightImage
                width={100}
                imageURL={'http://placehold.it/350x150'}
            />
        );
    }
}
```

### Props

| name              | type      | isRequired    | default           | description                                                           |
| ---               | ---       | ---           | ---               | ---                                                                   |
| `width`           | number    | ✔             | N/A               | image width to fit                                                    |
| `imageURL`        | string    | ✔             | N/A               | remote image url                                                      |
| `onHeightChange`  | func      | ✖             | (height) => {}    | called when updating image height, the argument `height` might be `0` |

Other image props except `source` and `resizeMode` are accepted.

## Change Log

[Change log](./CHANGELOG.md)

## Contributing

[Contributing](./CONTRIBUTING.md)

## Licence

[MIT](./LICENSE)
