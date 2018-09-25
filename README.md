# core.plugin.prepend

this plugin adds a `core.prepend` function which takes two string arguments and returns one string which is a combination of the two strings with a dot between them.

```js
let core = new require('core.constructor')();

core.plugin([
  require('core.plugin.prepend')
]);

core.prepend('some', 'key'); // => 'some.key'

// it will not duplicate if already exists
core.prepend('some', 'some.key'); // => 'some.key'

```
