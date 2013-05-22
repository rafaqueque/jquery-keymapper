# jQuery Keymapper plugin
This jQuery plugin allows you to bind keys (and key combinations as well) on DOM elements to execute a certain function. <code>run demo/index.html</code> and press a few keys.
It's pretty basic at the moment, but hoping to improve it with your help.

## Examples
Bind a key combination to the whole webpage.

    $('body').keymapper({
      keys: 'ctrl+a',
      callback: function() { alert("Hey!"); }
    });
    
Yes, this allows you to create a CTRL+S shortcut on specific elements to save things.

    $('textarea').keymapper({
      keys: 'ctrl+s',
      callback: function() { alert("Saved!"); }
    });
    
You can bind only one key as well.

    $('textarea').keymapper({
      keys: 'h',
      callback: function() { alert("Help!"); }
    });

## Tests
This plugin was tested on:

*   Firefox
*   Safari
*   Chrome

All of them running on OSX.

## To-Do
*   Add more events like 'keypress' and 'keydown'
*   Allow multiple keys combination like 'abc', for example

## About
You can ping me on Twitter ([@rafaqueque](http://twitter.com/rafaqueque)) or check my homepage: [rafael.pt](http://rafael.pt)