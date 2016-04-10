My Sublime Text 3 preferencies
==============================

A little package of Sublime Text config files.

[![MIT licensed][shield-license]](#)

Table of Contents
-----------------

  * [Requirements](#requirements)
  * [Installation](#installation)
  * [Setup](#setup)
  * [Keyboard shortcuts](#keyboard-shortcuts)
  * [Thanks](#thanks)
  * [License](#license)


Requirements
------------

Some plugins require the following to run:

  * [Node.js][node]
  * [npm][npm] (normally comes with Node.js)
  * [Hack Font][hack]
  * [Cmder][cmder]


Installation
------------

1. Go to Sublime Text
2. Find the `Preferences -> Browser packages...` from the menu and click it
3. Open the `User` folder
4. Close Sublime Text
5. Put all the files there
6. Follow this Hack installation [instructions][hack-installation]
7. Follow this Cmder installation [instructions][cmder-installation]


Setup SublimeLinter
-------------------

The SublimeLinter-jshint and SublimeLinter-csslint plugins can be easiest installed with [npm][npm]:

`npm install -g jshint` and `npm install -g csslint`

For SublimeLinter-php you must ensure that PHP path is available to use. If it is not, follow this [instructions][sublimelinter-path].

**Note:** The SublimeLinter-json no needs aditional setup.

## Error handling

You can visit the plugins' homepages for more details:

  * [SublimeLinter-jshint][sublimelinter-jshint-installation]
  * [SublimeLinter-csslint][sublimelinter-csslint-installation]
  * [SublimeLinter-php][sublimelinter-php-installation]
  * [SublimeLinter-json][sublimelinter-json-installation]


Keyboard shortcuts
------------------

### Terminal plugin

* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>T</kbd> : Open the Cmder in current file folder
* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd> : Open the Cmder in current project folder

More details available in [Terminal][terminal].

### PHP Companion plugin

  * <kbd>F6</kbd> : Expand the class under the cursor to its FQCN (Fully Qualified Class Name)
  * <kbd>Shift</kbd>+<kbd>f6</kbd> : Expand the class under the cursor to its FQCN (Fully Qualified Class Name) with the leading namespace separator `\`
  * <kbd>F5</kbd> + Cursor hover : It will show you the different namespace that match your class
  * <kbd>F4</kbd> : It will add the namespace definition based on the absolute filename of the current file
  * <kbd>Shift</kbd>+<kbd>f12</kbd> : It will search for a method definition based on the current scope
  * <kbd>F7</kbd> : It will insert both a constructor argument and its according property

More details and commands available in [PHP Companion][php-companion].


Thanks
------

Especial thanks to:

  * Sublime Text
  * Node.js and npm
  * Hack's author and contribuitors
  * Shields.io's author and contribuitors
  * And all Sublime Text's plugins authors and contribuitors


License
-------

This package is licensed under the [MIT](#) license.
Copyright &copy; 2016, Brendo Maciel



[node]: https://nodejs.org/
[npm]: https://www.npmjs.com/
[hack]: https://github.com/chrissimpkins/Hack
[cmder]: https://github.com/cmderdev/cmder
[terminal]: https://packagecontrol.io/packages/Terminal
[php-companion]: https://packagecontrol.io/packages/PHP%20Companion
[sublimelinter-path]: http://sublimelinter.readthedocs.org/en/latest/troubleshooting.html#finding-a-linter-executable
[hack-installation]: https://github.com/chrissimpkins/Hack#desktop-installation
[cmder-installation]: https://github.com/cmderdev/cmder#installation
[sublimelinter-jshint-installation]: https://github.com/SublimeLinter/SublimeLinter-jshint#installation
[sublimelinter-csslint-installation]: https://github.com/SublimeLinter/SublimeLinter-csslint#installation
[sublimelinter-php-installation]: https://github.com/SublimeLinter/SublimeLinter-php#installation
[sublimelinter-json-installation]: https://github.com/SublimeLinter/SublimeLinter-json#installation
[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
