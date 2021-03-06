[![npm](https://img.shields.io/npm/v/react-radio-buttons-group.svg)](https://www.npmjs.com/package/react-radio-buttons-group)
[![npm](https://img.shields.io/npm/dt/react-radio-buttons-group.svg)](https://www.npmjs.com/package/react-radio-buttons-group)

React Radio Buttons Group
============
React component for a group of radio buttons built with and for [React](http://facebook.github.io/react/index.html).

![demo](http://g.recordit.co/gqXy6MNVCP.gif)

[![stacklevel](http://i.imgur.com/mCxql4Z.png)](http://stacklevel.org/)

## Installation
`npm install react-radio-buttons-group --save`

## Usage

`<ReactRadioButtonsGroup/>` with a list of `<ReactRadioButton/>` components generate a hidden radio inputs that contain checked value, so you can submit it as part of a standard form.

When the value is changed, `onChange(inputRadioValue)` will fire.

```javascript
import { ReactRadioButtonsGroup, ReactRadioButton } from 'react-radio-buttons-group';

const RadioButtons = () => (
    <ReactRadioButtonsGroup group='sex' onChange={(value) => console.log(value)}>
        <ReactRadioButton value='male'>Male 👨</ReactRadioButton>
        <ReactRadioButton value='female'>Female 👩</ReactRadioButton>
    </ReactRadioButtonsGroup>
);
```

## Demo & Examples

> Coming soon...

![demo](http://i.imgur.com/qZI1yVd.gif)

## Components API

##### `<ReactRadioButtonsGroup/>`

Property | Type | Description
:---|:---|:---
`children` | function | Child function responsible for rendering the `<ReactRadioButton/>` components.
`group` | string | Field name, for hidden `<input />` tags
`onChange` | function | Function responsible for handling radio group changes. `(inputRadioValue) => { }`


##### `<ReactRadioButton/>`

Property | Type | Description
:---|:---|:---
`children` | function | Child function responsible for rendering the content into the `<label>`.
`value` | string | Attribute `value` for hidden `<input type='radio' />` tag. Also uses as `id` attribute for `<input type='radio' />` and `for` attribute for `<label>`.
