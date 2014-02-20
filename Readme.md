*This repository is a mirror of the [component](http://component.io) module [component/normalized-upload](http://github.com/component/normalized-upload). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-normalized-upload`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# normalized-upload

  Normalized DataTransfer items for less upload item handling pain.

## Installation

    $ component install component/normalized-upload

## Example

```js
var normalize = require('normalized-upload');

document.onpaste = function(e){
  console.log(e);
  normalize(e, function(){
    e.items.forEach(function(item){
      console.log(item);
    });
  });
};
```

## License

  MIT
