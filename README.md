# getOsLocalesCrossPlatform

A cross platform alternative to get locales used on the platform. Works on Node, Electron, NW.js and Browsers

This script is largely based on https://github.com/sindresorhus/os-locale

What I did is compile everything on a single script and add browser compatibility.

The scripts exports only one function to the global scope

# getOsLocales([options])

## options - Object with two parameters

### spawn - Boolean . Set to false if you want the function to try and get the locale without spawning any child processes. Doesn't do anything on browser.

### defaultLocale - String . The default locale to fallback to if nothing else works.

You can import this module using these:

```JS
const getOsLocales = require("getoslocalescrossplatform");
```

```JS
import getOsLocales from "getoslocalescrossplatform";
```

Or by integrating the file directly

```JS
import getOsLocales from "./getOsLocalesCrossPlatform.js";
```

```HTML
<script src="./getOsLocalesCrossPlatform.js"/>
```

Or by executing the content of the file and using the global function `getOsLocales()` it creates on the global scope.
