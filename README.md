# phantom-component
Render react component without div wrapper

##### Usage:

```javascript
import React from 'react';
import PhantomComponent from 'phantom-component';

const Foo = () =>
  <div>foo</div>;

const Bar = () =>
  <div>bar</div>;
  
const Foobar = () =>
  <PhantomComponent>
    <Foo />
    <Bar />
  </PhantomComponent>;
  
const Render = () =>
  <PhantomComponent>
    <Foo />
    <Bar />
    <Foobar />
  </PhantomComponent>
```

##### Render result:

```html
<div>foo</div>
<div>bar</div>
<div>foo</div>
<div>bar</div>
```
