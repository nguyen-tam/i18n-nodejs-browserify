## Install

```shell
npm install i18n-nodejs-browserify --save
```

## Usage

### New

```index.js

var locale = require('./locale.json');
var lang = "fr";
var i18n_module = require('i18n-nodejs-browserify');

var i18n = new i18n_module(lang, locale);
console.log(i18n.__('Welcome'));
```

### Languages file

Put it in the same folder as index.js

```locale.json
{
	"Welcome": {
		"ar": "مرحبا",
		"fr": "Bienvenue"
	},
	"Looking for user": {
		"ar": "نبحث الان عن مستخدم اخر"
	},
	"You have disconnected.": {
		"ar": "تم قطع الاتصال."
	},
	"Chat": {
		"ar": "شات"
	}
}
```
