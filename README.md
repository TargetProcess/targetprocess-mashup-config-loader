
# targetprocess-mashup-config-loader

Webpack loader to create Targetprocess mashup config from JSON file.

## Usage

```js
// config.json
{
    "name": "something"
}
```

```js
require('targetprocess-mashup-config-loader?libraryTarget=MyMashup!./manifest.json');
// will produce
// tau.mashups.addModule('MyMashup/config', {
//    "name": "something"
// })
```

## Options

### libraryTarget

Set root module name.

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
