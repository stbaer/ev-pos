# ev-pos

[![experimental](http://badges.github.io/stability-badges/dist/experimental.svg)](http://github.com/badges/stability-badges)

> relative position of mouse/touch events to element

## Usage

`npm i ev-pos`

[![NPM](https://nodei.co/npm/ev-pos.png)](https://www.npmjs.com/package/ev-pos)

```
var evPos = require('ev-pos');

document.querySelector('.some-element').addEventListener('click', function(ev){
    console.log('relative to currentTarget', evPos(ev));
    console.log('relative to document.body:', evPos(ev, document.body));
});
```

## API

** evPos(event, [toElement]) **

*if toElement is undefined it defaults to ev.currentTarget*


## Licence

MIT, see [LICENSE.md](http://github.com/stbaer/ev-pos/blob/master/LICENSE.md) for details.
