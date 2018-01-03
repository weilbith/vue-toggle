[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Issues](https://img.shields.io/codeclimate/issues/github/me-and/mdf.svg)](#issues)
# vue-toggle
A [Vue](https://vuejs.org) component that provides the functionality of a toggle or rather a switcher.<br>
It is rarely different than other such components. In fact it is more a custom solution on my own with some sepcial implementations.

<!-- TOC Begin -->
- [Demo](#demo)
- [Installation](#installation)
  - [Browser](#browser)
  - [Module](#module)
- [Usage](#usage)
  - [Props](#props)
<!-- TOC End -->


## Demo
Using different labels for both toggle states:<br>
![Values Demo](https://github.com/weilbith/vue-toggle/blob/master/doc/demo/Values-Demo.gif?raw=true)

## Installation

```js
npm install weilbith/vue-toggle
```

### Browser

Include the script file, then install the component with `Vue.use(VueToggle);` e.g.:

```html
<script type="text/javascript" src="node_modules/vuejs/dist/vue.min.js"></script>
<script type="text/javascript" src="node_modules/vue-toggle/dist/vue-toggle.min.js"></script>
<script type="text/javascript">
  Vue.use(VueToggle);
</script>
```

### Module

```js
import Vue from 'vue'
import VueToggle from 'vue-toggle'

Vue.component('vue-toggle', VueToggle)
```

## Usage

Once installed, it can be used in a template as simply as:

```html
<vue-toggle v-model="toggle" :size="15" :values="['Toggled', 'Not Toggled']" />
```

### Props

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| checked | _Boolean_ | none | The renamed `v-model` property |
| change | _Event_ | none | The renamed `@event` property |
| size | _Number_ | 20 | Interpreted in `px` and used as the absolute height. |
| values | _Array_ | none | Have to contain exactly two `Strings` that are used to display the toggle state.<br>E.g.: `['Toggled', 'Not Toggled']` |
