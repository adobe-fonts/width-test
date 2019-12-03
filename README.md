# Width Test

Width Test (&#x5E45;&#x30C6;&#x30B9;&#x30C8; is its Japanese name) is a special-purpose OpenType/CFF font that is intended to be used to test the extent to which applications and other text-handling environments support the various width-related GSUB features, specifically '[fwid](https://www.microsoft.com/typography/otspec/features_fj.htm#fwid)' (*Full Widths*), '[hwid](https://www.microsoft.com/typography/otspec/features_fj.htm#hwid)' (*Half Widths*), '[twid](https://www.microsoft.com/typography/otspec/features_pt.htm#twid)' (*Third Widths*), and '[qwid](https://www.microsoft.com/typography/otspec/features_pt.htm#qwid)' (*Quarter Widths*).

* The glyph set includes the mandatory *.notdef* glyph at CID+0, along with a *space* (U+0020) glyph at CID+1.

* CID+2 is the glyph for zero (U+0030) that was taken from the Regular weight of [Source Code Pro](https://github.com/adobe-fonts/source-code-pro/) and which has a 600-unit horizontal advance. This glyph serves as a default glyph whose horizontal advance can be considered proportional.

* CIDs 3 through 6 are full-, half-, third-, and quarter-width glyphs that are made up of black boxes that correspond to the denominator portion of their width value when expressed as a fraction, and the use of the 'fwid', 'hwid', 'twid', or 'qwid' GSUB features will substitute zero (U+0030) with the appropriate glyph.

* CIDs 3 through 6 are additionally mapped from one (U+0031) through four (U+0034) for the purpose of easing the creation of reference tests. CID+3 is also mapped from full-width zero (U+FF10).

The image below shows the glyphs for CIDs 2 through 6 with registration marks:

![alt text](https://raw.githubusercontent.com/adobe-fonts/width-test/master/resources/width-test.jpg "img-View")

## Font installation instructions

* [macOS](https://support.apple.com/en-us/HT201749)
* [Windows](https://www.microsoft.com/en-us/Typography/TrueTypeInstall.aspx)
* [Linux/Unix-based systems](https://github.com/adobe-fonts/source-code-pro/issues/17#issuecomment-8967116)

## Building the font from source

### Requirements

To build the binary font file from source, you need to have installed the [Adobe Font Development Kit for OpenType](http://www.adobe.com/devnet/opentype/afdko.html) (AFDKO). The AFDKO tools are widely used for font development today, and are part of most font editor applications.

### Building the font

In this repository, all necessary files are in place for building the OpenType/CFF font, and the COMMANDS.txt file provides the command lines that are used.

## Getting Involved

For any suggestions for changes, please [create a new issue](https://github.com/adobe-fonts/width-test/issues) for consideration.
