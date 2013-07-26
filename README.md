jquery-simplecolorpicker plugin for Hallo Editor
=====================================

[Hallo](https://github.com/bergie/hallo) was written by Henri Bergius
[jquery-simplecolorpicker](https://github.com/tkrotoff/jquery-simplecolorpicker) was written by Tanguy Krotoff

This plugin just works as an adapter for hallo so you can use the simplecolorpicker in it.

## Dependencies

Obvious the Hallo Editor and the jquery-simplecolorpicker as since they need jquery and jquery-ui you need to add them too.

## Using the Plugin

You need jQuery and jQuery UI loaded. An easy way to do this is to use Google's JS service:

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
<script src="https://ajax.googleapis.com/ajax/libs/jqueryui/1.8.18/jquery-ui.min.js"></script>
```

Then include Hallo and the jquery-simplecolorpicker themselves

```html
<script src="/path/to/your/hallo.js"></script>
<link rel="stylesheet" href="/path/to/your/jquery.simplecolorpicker.css">
<script src="/path/to/your/jquery.simplecolorpicker.js"></script>
```

Finally this plugin itself:

```html
<script src="hallo-simplecolorpicker-plugin.js"></script>
```

Using the Plugin is easy, just add the plugin into your hallo plugin:

```javascript
jQuery('p').hallo({
	plugins: {
		'hallosimplecolorpicker' : {}
	}
});
```

This example would enable the default colors.

### Options

The Plugin provides some options you can override:

* `colors`: the colors you want to configure the simplecolorpicker to work on.
* `simplecolorpicker`: the options for the simplecolorpicker jquery plugin which are passed through. See the plugins [README](https://github.com/tkrotoff/jquery-simplecolorpicker) for more information

The `colors` option uses an Option for the configuration where the key is the hex value and the value is the label for the select options.
```javascript
	colors: {
		"#7bd148": "Green",
		"#5484ed": "Bold blue",
		"#a4bdfc": "Blue",
		"#46d6db": "Turquoise",
		"#7ae7bf": "Light green",
		"#51b749": "Bold green",
		"#fbd75b": "Yellow",
		"#ffb878": "Orange",
		"#ff887c": "Red",
		"#dc2127": "Bold red",
		"#dbadff": "Purple",
		"#e1e1e1": "Gray",
		"#000000": "Black"
	}
```

## Licensing

Hallo is free software available under the [MIT license](http://en.wikipedia.org/wiki/MIT_License).
