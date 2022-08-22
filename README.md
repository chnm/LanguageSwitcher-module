# Switch Language Omeka Plugin

An Omeka S plugin to support language switching for *Chile 88*. This plugin allow users to choose the website language. Admins can configure the public languages available and the default website language. 

This is a modification of [the original plugin](https://gitlab.com/TIME_LAS/Omeka_Plugin_SwitchLang/-/tree/master).

## Requirements

Omeka S.

## Installation

1. Download the Chile 88 Language Switcher from Github: 

```$ git clone https://github.com/chnm/chile88-language-switcher.git```

2. Upload the plugin to the plugins directory of your Omeka installation in a "SwitchLanguage" directory. See the [Installing a Plugin](http://omeka.org/codex/Installing_a_Plugin) page for details.

 ```$ mv chile88-language-switcher $OMEKA_PATH/plugins/SwitchLanguage```

3. Once it's uploaded in the `plugins` directory, go to the plugins management interface and click on the green "Install" button in the listing for the Switch Language plugin.

## Configure the plugin

The Switch Language plugin lets you choose the following options:
* Choose the default language: this will be both the default public language and the admin interface language.

* Choose the display type:
 * Drop-down menu, links, or banners (flags) 
 * Displaying language name, language code, or flags only

* If you want to use customized flags, put files on a subdirectory of your theme and specify it as a plugin option
 * File names must be: "flag-$LANGCODE.png" (e.g. "flag-fr.png")
 * Images have to be PNG and will be display with height and width of 25px
 * If no flag is found in the theme, plugin flags will be used
 * If no subdirectory is specified, the plugin will look for an "img/" directory
 * Subdirectory must finish by "/" (e.g. "custom-flag/")

* Choose the language which will be available on the public interface
 * List only the language which have a translate file in your $OMEKA/application/languages/ directory
