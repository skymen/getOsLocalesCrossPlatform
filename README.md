# getOsLocaleCrossPlatform
A cross platform alternative to get locales used on the platform. Works on Node, Electron, NW.js and Browsers


This script is largely based on https://github.com/sindresorhus/os-locale

What I did is compile everything on a single script and add browser compatibility.

The scripts exports only one function to the global scope

# getOsLocale([options])
## options - Object with two parameters
### spawn - Boolean . Set to false if you want the function to try and get the locale without spawning any child processes. Doesn't do anything on browser.
### defaultLocale - String . The default locale to fallback to if nothing else works.
