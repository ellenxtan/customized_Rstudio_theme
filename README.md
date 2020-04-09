# Customized RStudio Theme

# Custom R Theme to Resemble VS Code

The theme is modified based on  [Michael Asher's](https://github.com/michaelasher/CustomRStudioTheme) to resemble VS code.

Import your own R Studio theme. To do so, go to "Preferences" -> "Appearance" and click "Add..." the `.rstheme` file.

By default, R Studio will make the text for function calls the same color as variable the text for variable names. To change this, go to "Preferences" -> "Code" -> "Display" and check "Highlight R function calls." RStudio will subsequently reference the `.ace_entity.ace_name.ace_function` and `.ace_support.ace_class` parts of the rstheme document, which allows you to change the color of calls to functions and packages.

[This page](https://rstudio.github.io/rstudio-extensions/rstudio-theme-creation.html) is very helpful for outlining the different components of the rstheme code that makes up an RStudio theme.

## Changing RStudio so Surrounding Regions are Black

The updates, described above, change only the layout of the panes (e.g. the console, source, etc.). If you want to change the colors that surround the panes to further resemble VS code (which has a darker black color), you can add a new .css file to your `~/RStudio.app/Contents/Resources/www/` folder and make an update to the `index.htm` document to reference the new .css file. [Riley Roach](https://github.com/riley-roach/RStudio-Customizations) provides the necessary code to do so (along with instructions).
