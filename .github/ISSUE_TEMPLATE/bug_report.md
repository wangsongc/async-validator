---
name: 🐛 Bug report
about: Create a report to help us improve
title: '[BUG] XYZ'
labels: ':bug: Bug'
---

## 🐛 Bug Report

<!-- A clear and concise description of what the bug is. -->

Lib version: X.Y.Z

## Steps To Reproduce

<!-- The exact steps required to reproduce the issue, ideally with a code example -->

```javascript
import schema from 'async-validator';
var descriptor = {
  name: {
    type: "string",
    required: true,
    validator: (rule, value) => value === 'muji',
  },
  age: {
    type: "number",
    asyncValidator: (rule, value) => {
        return new Promise((resolve, reject) => {
          if (value < 18) {
            reject("too young");  // reject with error message
          } else {
            resolve();
          }
        });
      }
  }
};
```

## The expected behaviour:

<!-- A clear and concise description of what you expected to happen. -->


## Possible solution (optional, but very helpful):

```javascript

```
