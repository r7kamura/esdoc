[![Build Status](https://travis-ci.org/h13i32maru/esdoc.svg?branch=master)](https://travis-ci.org/h13i32maru/esdoc)
[![Coverage Status](https://coveralls.io/repos/h13i32maru/esdoc/badge.svg)](https://coveralls.io/r/h13i32maru/esdoc)
[![Document](https://doc.esdoc.org/github.com/h13i32maru/esdoc/badge.svg)](https://doc.esdoc.org/github.com/h13i32maru/esdoc)

# ESDoc

ESDoc is a documentation generator for JavaScript(ES6).

<img class="screen-shot" src="https://esdoc.org/image/top.png" width="500px" style="max-width: 500px; border: 1px solid rgba(0,0,0,0.1); box-shadow: 1px 1px 1px rgba(0,0,0,0.5);">

# Feature
- Generates detailed document.
- Measures document coverage.
- Integrate test codes into documentation.

# Demo
- [ESDoc](https://esdoc.org/esdoc) is self-hosting &#x1F604;

# Install

```
npm install -g esdoc
esdoc -h
```

# Usage

```
esdoc -c esdoc.json
```

# Example
```
├── esdoc.json
└── src/MyClass.js
```

``src/MyClass.js``

```javascript
/**
 * this is MyClass.
 */
export default class MyClass {
  /**
   * @param {number} param this is param.
   * @return {number} this is return.
   */
  method(param){}
}
```

``esdoc.json``

```json
{
  "source": "./src",
  "destination": "./esdoc"
}
```

exec esdoc

```
esdoc -c esdoc.json
open ./esdoc/index.html
```

# Document
please visit [esdoc.org](https://esdoc.org) to see more document.

# License
MIT
