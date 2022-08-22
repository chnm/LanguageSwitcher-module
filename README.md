# Switch Language Omeka Module 

An Omeka S module to support language switching for *Chile 88*. This module allow users to choose the website language. Admins can configure the public languages available and the default website language. 

This is a modification of [the original plugin for Omeka Classic](https://gitlab.com/TIME_LAS/Omeka_Plugin_SwitchLang/-/tree/master), designed to handle some specifics from *Chile 88* and work with Omeka S.

## Requirements

Omeka S.

## Installation

1. Download the Chile 88 Language Switcher from Github: 

```$ git clone https://github.com/chnm/LanguageSwitcher-module.git```

2. Upload the module to the  directory of your Omeka installation in a "SwitchLanguage" directory. See [Modules Management](https://omeka.org/s/docs/user-manual/modules/) for details.

 ```$ mv LanguageSwitcher-module $OMEKA_PATH/modules/SwitchLanguage```

3. Once it's uploaded in the `modules` directory, go to the modules management interface and click on the green "Install" button in the listing for the Switch Language module.

## Configure the module 

The Switch Language module lets you choose the following options:

* Choose the default language: this will be both the default public language and the admin interface language.
* Choose the display type:
    * Drop-down menu, links, or banners (flags) 
    * Displaying language name, language code, or flags only
* If you want to use customized flags, put files on a subdirectory of your theme and specify it as a module option
    * File names must be: "flag-$LANGCODE.png" (e.g. "flag-fr.png")
    * Images have to be PNG and will be display with height and width of 25px
    * If no flag is found in the theme, module flags will be used
    * If no subdirectory is specified, the module will look for an "img/" directory
    * Subdirectory must finish by "/" (e.g. "custom-flag/")
* Choose the language which will be available on the public interface
    * List only the language which have a translate file in your $OMEKA/application/languages/ directory
