# simpleImageCheck(current version: 0.4)

SimpleImageCheck is a jQuery plug-in that makes custom image checkboxes and radio buttons super easy. Simply use standard inputs and labels for your fields, then call the function to set up the custom UI. Your checkbox (or radio button) is still there (just hidden), and all form submissions will work as normal.

New Feature:  add initial state with `wasChecked` input parameter.

## Sample Usage
    $('#myCheckbox').simpleImageCheck({
      image: 'unchecked.png',
      imageChecked: 'check.png', 
      wasChecked: true,
      afterCheck: function(isChecked) {
        if (isChecked) {
          // do something
        }
      }
    });

## Requirements
 * jQuery 1.2+
 * jquery.simpleImageCheck (this plug-in)

## Feature List
 * Use custom images for checkboxes and radio buttons
 * Continue to use standards-compliant input fields and labels
 * Doesn't break form submission
 * Full ARIA implementation
 * Lightweight (1.93kb minified)
 * Tested Browsers
 * Mozilla Firefox 2/3
 * Microsoft Internet Explorer 7/8
 * Google Chrome
 * Opera

## Known Issues
 * IE 6 doesn't like my examples page...
 * All versions of IE (that I tested) have an issue when you attach a "change" event handler to the input node (otherwise you're fine). You will have to click on the image/checkbox multiple times in order to "tick" the box.
 * WORKAROUND: In order to get around this issue, you can use the "afterCheck" event handler option when instantiating the simpleImageCheck plugin:


Original source available at http://jordankasper.com/jquery/imagecheck/

Authors: 
 * Jordan Kasper (jquery@jordankasper.com)
 * Mr Rogers (mrrogers@bunnymatic.com)

Contributors:
 * [jewelsjacobs](https://github.com/jewelsjacobs)
