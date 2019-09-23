### ipfy
---
https://github.com/sindresorhus/ipify

```js
// test.js
import test from 'avva';
import isIp from 'is-ip';
import ipify from '.';

test('main', async t => {
  t.true(isIp(await ipify()));
});

test('useIPv6:false', async t => {
  t.true(isIp.v4(await ipify({useIPv6: false})));
});

test('endpoint:custom', async t => {
  t.true(isIp.v4(await ipify({endpoint: 'https://api.ipify.org'})));
});


```

```js
const ipify = require('ipify');

(async () => {
  console.log(await ipify());
  
  console.log(await ipify({useIPv6: false}));
})();
```

```
```


