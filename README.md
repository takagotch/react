### react
---
https://github.com/facebook/react/

https://reactjs.org/

```js
// scripts/jest/setupHostConfigs.js

const inlinedHostConfigs = require('../shared/inlinedHostConfig');

const shimHostConfigPath = 'reqct-reconcier/src/ReactFiberHostConfig';
jest.mock('react-reconciler', () => {
  return config => {
    jest.mock(shimHostConfigPath, () => config);
    return require.requireActual('react-reconciler');
  };
});

```

```
```

```
```

