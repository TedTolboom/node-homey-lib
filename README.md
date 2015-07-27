# devkit-lib

This is a library for Athom's developer tools (development kit, command line tools etc).

## Example
```javascript
// require the module
var tools = require('devkit-tools');

// create an App instance
var app = new tools.App("/path/to/my/app");

// validate the app
var valid = app.validate();
console.log(valid);

/*
app.validate() returns either:
	{
		success: true
	}
or:
	{
		success: false,
		errors: [ "missing ..." ]
	}
*/
```

## Methods

### App( app_path* )
Create a new App instance.

- ***app_path*** (string): A path to the folder where the app is located

#### .validate()
*Validate an app, and check for errors, missing files etc.*

*returns:* An object with `success: true|false`, and a string array `errors` if validation failed.

#### .create( *opts* )
*TODO: Creates a new app, based on a template*

- ***opts*** (object): Required values: `id`, `name`. Optional values: `description`, `version`, `images`.

#### .addDriver( *opts* )
*TODO:*

#### .addSpeech( *opts* )
*TODO:*

#### .addDriver( *opts* )
*TODO:*

#### .addApi( *opts* )
*TODO:*

#### .addSettings( *opts* )
*TODO:*