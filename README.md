# Creenv easings

> A list of easings functions. This package is standalone and doesn't need the creative environment to work.

## 1. Installation

```bash
npm install --save @creenv/easings
```

## 2. Usage 

```js 
import EASINGS from "@creenv/easings";

let x = 0.4;

let xEased = EASINGS.linear(x);
```

## 3. Easings list 

| Name | Description |
| ---- | ----------- |
| **linear** | t => t |
| **quadIn** | t => t*t |
| **quadOut** | t => t*(2-t) |
| **quadInOut** | t => (t<0.5) ? 2*t*t : -1+(4-2*t)*t |
| **cubicIn** | t => t*t*t |
| **cubicOut** | t => (--t)*t*t+1 |
| **cubicInOut** | t => t<.5 ? 4*t*t*t : (t-1)*(2*t-2)*(2*t-2)+1 |
| **quartIn** | t => t*t*t*t |
| **quartOut** | t => 1-(--t)*t*t*t |
| **quartInOut** | t => t<.5 ? 8*t*t*t*t : 1-8*(--t)*t*t*t |
| **quintIn** | t => t*t*t*t*t |
| **quintOut** | t => 1+(--t)*t*t*t*t |
| **quintInOut** | t => t<.5 ? 16*t*t*t*t*t : 1+16*(--t)*t*t*t*t |

