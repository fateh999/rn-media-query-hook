# rn-media-query-hook

[![npm version](https://img.shields.io/npm/v/rn-media-query-hook.svg?style=for-the-badge)](https://www.npmjs.com/package/rn-media-query-hook)
[![npm downloads](https://img.shields.io/npm/dm/rn-media-query-hook.svg?style=for-the-badge)](https://www.npmjs.com/package/rn-media-query-hook)
[![npm](https://img.shields.io/npm/dt/rn-media-query-hook.svg?style=for-the-badge)](https://www.npmjs.com/package/rn-media-query-hook)
[![npm](https://img.shields.io/npm/l/rn-media-query-hook?style=for-the-badge)](https://github.com/fateh999/rn-media-query-hook/blob/master/LICENSE)

React Native Media Query Hook

#### Demo :

https://snack.expo.dev/@fateh999/rn-media-query-hook

#### Steps to install :

```javascript

npm install rn-media-query-hook

```

or

```javascript

yarn add rn-media-query-hook

```

```javascript
import useMediaQuery from "rn-media-query-hook";

// In functional component
const { mediaQuery, mediaQueryLogic } = useMediaQuery();
```

or

```javascript
import useMediaQuery from "rn-media-query-hook";

// In functional component
const { mQ, mQL } = useMediaQuery();
```

#### Usage :

```javascript
// For dimensions
const responsiveWidth = mQ([100, 200, 300, 400, 500]);

// order is important [base, sm, md, lg, xl]

// or

const responsiveWidth = mQ({ base: 100, sm: 200, md: 300, lg: 400, xl: 500 });

// For any logic
const show = mQL([true, true, true, false, false]);

// order is important [base, sm, md, lg, xl]

// or

const show = mQ({ base: true, sm: true, md: true, lg: false, xl: false });
```

### Default Breakpoints :

```javascript
const initialBreakPoints: BREAK_POINTS = {
  base: 0,
  sm: 480,
  md: 768,
  lg: 992,
  xl: 1280,
};
```

### Custom Breakpoints :

```javascript
const newBreakPoints: BREAK_POINTS = {
  base: 0,
  sm: 380,
  md: 868,
  lg: 892,
  xl: 1180,
};

// In functional component

const { mediaQuery, mediaQueryLogic } = useMediaQuery(newBreakPoints);
```

### Note :

- Only base dimension or logic is required, rest are optional

<p><a href="https://www.buymeacoffee.com/fateh999"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="fateh999" /></a></p><br><br><br>
