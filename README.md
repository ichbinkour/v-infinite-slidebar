# v-infinite-slidebar

> ✨ Infinite slide bar component for awesome vue project ✨

[![npm version](https://img.shields.io/npm/v/v-infinite-slidebar)](https://www.npmjs.com/package/v-infinite-slidebar)
[![npm downloads](https://img.shields.io/npm/dm/v-infinite-slidebar)](https://www.npmjs.com/package/v-infinite-slidebar)
[![GitHub stars](https://img.shields.io/github/stars/ichbinkour/v-infinite-slidebar?style=social&label=Star&maxAge=2592000)](https://github.com/ichbinkour/v-infinite-slidebar)



> [Demo](https://ichbinkour.github.io/#/v-infinite-slidebar)

## Installation

```js
npm i v-infinite-slidebar
```

Or

```js
yarn add v-infinite-slidebar
```

## Usage

```js
import vue from "Vue"
import VInfiniteSlidebar from "v-infinite-slidebar"

Vue.component('v-infinite-slidebar', VInfiniteSlidebar)
```

Or

```js
import VInfiniteSlidebar from "v-infinite-slidebar"

export default {
  components: {
    VInfiniteSlidebar
  }
}
```

## API

| Name            | Type      | Default  | Description                                                         |
| :-------------- | :-------- | :------- | ------------------------------------------------------------------- |
| `slideBarStyle` | `Object`  | `None`   | Style that will be applied to the component.                        |
| `duration`      | `String`  | `15s`    | Duration of the animation.                                          |
| `direction`     | `String`  | `normal` | Direction of the animation, you can also use 'reverse' for example. |
| `delay`         | `String`  | `0s`     | Delay before the animation starts.                                  |
| `paused`        | `Boolean` | `false`  | Stop the animation when set to true                                 |

Check on [Github](https://github.com/ichbinkour/v-infinite-slidebar)
