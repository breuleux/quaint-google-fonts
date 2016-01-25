
quaint-google-fonts
===================

This plugin lets you easily import fonts from Google Fonts for use in
your pages.


## Install

    quaint --setup google-fonts

Follow the instructions.


## Sample configuration

This configuration entry must be added in the `plugins` field of
`quaint.json`:

```json
"google-fonts": {
  "fonts": [
    "Open Sans",
    "Alegreya:400,400italic,700"
  ]
}
```


## Usage

The fonts you choose to import will be available for use in your CSS
files and directives, like any other font.


## Options

### `fonts`

An array of font names.

For each font you can also add styles (bold, italic) and character
sets you want (greek, cyrillic, etc). For example:

    "Open Sans:400,400italic,700&subset=latin,greek"

will load the Open Sans font with the normal (400), normal italic, and
bold (700) styles, and the latin and greek character sets. Note that
each style and subset you add will add to the size of the download, by
a factor equal to the number of possible combinations: just "Open
Sans" is about 15 KB, but the above set is 90 KB (but it will look
nicer).

Browse [Google Fonts](https://www.google.com/fonts) for the list of
fonts available. If you add them to your collection and then click
"Use" at the bottom, you get to pick the styles and character sets and
you can copy/paste the code given. Not all fonts have all possible
styles.
