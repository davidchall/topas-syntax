# topas-syntax
Syntax highlighting for [TOPAS](http://topasmc.org) parameter files in [Sublime Text](http://www.sublimetext.com).

![Screenshot](https://github.com/davidchall/topas-syntax/raw/master/topas_syntax.png)

## Installation
Installing packages for Sublime Text is easiest through the [Package Control](https://packagecontrol.io) plugin, and this package is no different.

Once you have Package Control, follow these instructions:
* open the Command Palette (`cmd+shift+p` on Mac, `ctrl+shift+p` on Linux/Windows)
* select `Package Control: Install Package`
* search for `Topas Syntax`

## Usage
Since TOPAS parameter files use the ubiquitous `.txt` file extension, it is not enabled by default.
To apply the syntax highlighting to an opened file, select `View > Syntax > Topas`.

As this could become laborious when managing many parameter files, I recommend saving your directory tree as a [Sublime Text project](https://www.sublimetext.com/docs/3/projects.html).
I personally use the excellent [Project Manager](https://packagecontrol.io/packages/Project%20Manager) package for managing my projects, though this isn't necessary.
Then you can use the [Project Specific Syntax Settings](https://packagecontrol.io/packages/Project%20Specific%20Syntax%20Settings) package to tell Sublime Text to use the TOPAS syntax highlighting for your project, by choosing `Edit Project` from the Command Palette:

```json
{
    ...
    "syntax_override": {
        "\\.txt$": ["Topas Syntax", "Topas"]
    }
}
```

### Addendum
It might be possible to import the `Topas.tmLanguage` grammar file into other editors such as [TextMate](https://macromates.com). However, I stick to Sublime Text. :-)
Please let me know if you install it on another editor, and I can update the README.
