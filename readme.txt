=== Google Webfonts For Woo Framework ===
Contributors: judgej
Donate link: 
Tags: woothemes, google webfonts, typography, fonts, woo framework
Requires at least: 3.3
Tested up to: 3.5.1
Stable tag: 1.2.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Give the WooThemes framework access to the full range of current Google Webfonts.

== Description ==

The purpose of this plugin is to make all available Google webfonts available to the WooThemes Canvas theme, and any other themes that use the WooThemes framework.

It works like this:

1. You register for a Google API key, and make sure it is enabled for web fonts. Set the API key in the plugin settings menu.
2. The key is used to download the full list of Google web fonts. This is cached locally, and will only be refreshed when you save the plugin settings page.
3. The full list of fonts and all variants replaces the list that the Woo framework defines internally.

What you should then see, is the ability to select any available Google web font in the WooThemes theme administration pages, and have those fonts displayed in your theme.

Register for a Google API key, and turn on "webfonts" for the key here:

[http://code.google.com/apis/console](http://code.google.com/apis/console)

This plugin has been tested against PHP5.3 and the project repository is here:

[https://github.com/academe/google-webfonts-for-woo-framework/](https://github.com/academe/google-webfonts-for-woo-framework/)

Changes have been made so that it works with PHP5.2 and has been reported as working. However, I work underat least 5.3 so some incompatibilities may creep in by accident from time-to-time - just report them and I will do my best to fix as quickly as possible.

Please let me know how this plugin works for you, whether you like it, and how it can be improved.

== Installation ==

1. Upload google-fonts-for-woo-framework/ to the `/wp-content/plugins/` directory or google-fonts-for-woo-framework.zip through the "Add Plugins" administration page.
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Add your Google API key to the settings page for the plugin.

== Frequently asked questions ==

= What if I don't have a Google API key? =

No problem! From version 1.2.0 this plugin carries a list of fonts and variants as a fall-back. If the API key is not
entered or the API key is invalid, then the plugin will use the fallback list. This list initially contains 652 fonts
but will slowly get out of date as Google extends its fonts. It will be refreshed on each new version of the plugin
however.

= Where do I get a Google API key? =

A Google API key can be obtained here: http://code.google.com/apis/console

= How can I contribute to this plugin? =

This plugin is managed on github here https://github.com/academe/google-webfonts-for-woo-framework
Feel free to raise issues there and make pull requests, as well as in the normal way on wordpress.org

= I have installed this plugin and my API key seems to be already set. How? =

The option used to store your API key shares it name with several other popular Google Webfonts plugins.
If you have used, or are using, those plugins too, then the API key setting will be shared. This is by design.

= I see errors reported when fetching the nerw Google webfonts =

Some hosts may not be set up to allow your site to fetch data from remote sites. Please report any 
such errors on the plugin page or github, and we will try looking for a workaround.

= Can I use the new fonts in a page body? =

Yes. WooThemes themes provides a short-code tag that allows you to embed any font in the body of a page or ppst.
However, the list of fonts that the short-code quick-create function inb the content editor provides, will not
be the full list of all fonts. So work around this, just select any random font, then change the name of the
font manually in the short-code tag.

== Screenshots ==

1. 
2. 

== Changelog ==

= Version 1.2.0 =
* Introduction of fallback list of fonts when Google cannot be contacted for any reason.
* Cache is no incdefinite; it is refreshed only when saving the settings page.
* The list of fonts from Google completely replaces the list in the Woo Framework, rather than merging in.
* The font list shown on the settings page shows the available variants more clearly.
* The font preview function supports italic style and the main font weights (nine weights from 100 to 900).

= Version 1.1.0 =
* Reports errors fetching Google fonts.
* Updates the built-in framework fonts with new variations, improving quality of displayed fonts.

= Version 1.0.0 =
* i18n complete.
* Show fonts used by the theme as selected in admin page.
* Split admin functions into a separate script and class.
* Ability to preview fonts.

== Upgrade notice ==
