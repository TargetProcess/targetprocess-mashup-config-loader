
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

### parse

Parse and output config as valid JSON, set to `false` to use comments in JSON.

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
