My Sublime Text 3 preferencies
==============================

A little package of Sublime Text config files in Windows environment.

[![MIT licensed][shield-license]][license]
[![Sublime Text 3][shield-sublime]][sublime]

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
  * [Hyper][hyper]


Installation
------------

```
$ git clone https://github.com/brendomaciel/sublime-preferences
```

1. Clone the repository or simply download [here][download]
2. Go to Sublime Text
3. Find the `Preferences -> Browser packages...` from the menu and click it
4. Open the `User` folder
5. Close Sublime Text
6. Extract and uut all the files there
7. Follow this Hack installation [instructions][hack-installation]
8. Follow this Hyper installation [instructions][hyper-installation]


Setup
-----

### SublimeLinter

The SublimeLinter-jshint and SublimeLinter-csslint plugins can be easiest installed with [npm][npm]:

`npm install -g jshint` and `npm install -g csslint`

**Note:** The SublimeLinter-php and SublimeLinter-json plugins don't need additional setup, but you must ensure that PHP command is available to use the same way as node.js. If it is not, follow this [instructions][sublimelinter-path].

#### Error handling

You can visit the plugins' homepages for more details:

  * [SublimeLinter-jshint][sublimelinter-jshint-installation]
  * [SublimeLinter-csslint][sublimelinter-csslint-installation]
  * [SublimeLinter-php][sublimelinter-php-installation]
  * [SublimeLinter-json][sublimelinter-json-installation]

### Terminal

You must change the path of the Hyper executable in the `Terminal.sublime-settings` file. Probably you just need to correct the username of the Windows profile.

I tried to use the `%LOCALAPPDATA%` variable on the path so that this step was not necessary, but it did not work.


Keyboard shortcuts
------------------

### Terminal plugin

* <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>T</kbd> : Open the Hyper in current file folder

Note: I could not get the <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd> shortcut work properly using Hyper, which should open Hyper in the current project folder.

Bonus: If you're interested, you can check out my Hyper settings [here][hyper-preferences].

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
  * Hyper's author and contribuitors
  * Hack's author and contribuitors
  * Shields.io's author and contribuitors
  * And all Sublime Text's plugins authors and contribuitors


License
-------

This package is licensed under the [MIT][license] license.
Copyright &copy; 2016 Brendo Maciel



[download]: https://github.com/brendomaciel/sublime-preferences/archive/master.zip
[sublime]: https://www.sublimetext.com/3
[license]: https://github.com/brendomaciel/sublime-preferences/blob/master/LICENSE
[node]: https://nodejs.org/
[npm]: https://www.npmjs.com/
[hack]: https://github.com/chrissimpkins/Hack
[hyper]: https://github.com/zeit/hyper
[hyper-preferences]: https://github.com/brendomaciel/hyper-preferences
[terminal]: https://packagecontrol.io/packages/Terminal
[php-companion]: https://packagecontrol.io/packages/PHP%20Companion
[sublimelinter-path]: http://sublimelinter.readthedocs.org/en/latest/troubleshooting.html#finding-a-linter-executable
[hack-installation]: https://github.com/chrissimpkins/Hack#desktop-installation
[hyper-installation]: https://github.com/zeit/hyper
[sublimelinter-jshint-installation]: https://github.com/SublimeLinter/SublimeLinter-jshint#installation
[sublimelinter-csslint-installation]: https://github.com/SublimeLinter/SublimeLinter-csslint#installation
[sublimelinter-php-installation]: https://github.com/SublimeLinter/SublimeLinter-php#installation
[sublimelinter-json-installation]: https://github.com/SublimeLinter/SublimeLinter-json#installation
[shield-sublime]: https://img.shields.io/badge/Sublime%20Text-3-orange.svg
[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
