---
tags:
  - product
aliases:
  - VS
slug: vs
organizations:
  - microsoft
url:
---

# Visual Studio

## Summary


## Quotes


## References

1. [Debug your Python code in Visual Studio](https://learn.microsoft.com/en-us/visualstudio/python/debugging-python-in-visual-studio?view=vs-2022)

## People

- 

## Integrations

- 
## Notes

### My config

-  `Tools -> Options -> Text Editor`, in the `Display` group, uncheck **Highlight current line**
- first remove the existing mapping  `Options > Environment > Keyboard` then
	- `selectcurrentword` -> Remove
	- `window.closedocumentwindow` - map to `Ctrl-w` -> Assign
- To disable the annoying **Map Mode** code browser on the far right
	- `Tools -> Options -> Text Editor -> All Languages -> Scroll Bars` and disable 'Show vertical scroll bar '
- To disable the vertical dashed lines, also known as **structure guide lines**: `Tools → Options -> Text Editor → General`, uncheck the option **Show structure guide lines**.

	This will remove the vertical dashed lines from your code editor in Visual Studio. [If you’re using an extension like Productivity Power Tools, you might need to adjust the settings within the extension options to disable the lines](https://stackoverflow.com/questions/42763074/remove-vertical-dotted-indentation-lines-in-visual-studio-2017)[1](https://stackoverflow.com/questions/42763074/remove-vertical-dotted-indentation-lines-in-visual-studio-2017)[2](https://stackoverflow.com/questions/42439962/how-to-remove-vertical-dashed-lines).

### Themes

- [JFlepp.VS.Theme.DarkYellow](https://marketplace.visualstudio.com/items?itemName=J-Flepp.JFleppVsThemeDarkYellow)
- [Deepdark Material Theme](https://marketplace.visualstudio.com/items?itemName=Nimda.vs-deepdark-material)

### No go themes

- [Visual Studio Theme Pack](https://marketplace.visualstudio.com/items?itemName=idex.vsthemepack)
- [Matrix Theme](https://marketplace.visualstudio.com/items?itemName=pritompurkayasta.matrixtheme)
- [CyberPunk Theme](https://marketplace.visualstudio.com/items?itemName=T0uchM3.CTVS19)
- [Dark Theme (2019)](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.DarkTheme2019)
### Installing Python Packages

To install PyYAML inside Visual Studio, you can use the built-in Python package manager. Here’s how you can do it:

2. Go to the **Solution Explorer** and right-click on your Python environment under the **Python Environments** section.
3. Select **Manage Python Packages…** from the context menu.

![[Visual Studio - Manage Python Packages.png]]

1. In the package manager, search for `PyYAML`
2. Once you find it, select it and click on the **Install** button.

This installs PyYAML in the Python environment currently associated with your project. Make sure you’re working in the correct environment if you have multiple ones. After the installation, you should be able to import and use the `yaml` module in your project without any issues. If you encounter any further problems, feel free to ask for more assistance!

### To see the packages installed

![[Visual Studio - Python Environment.png]]

### To show README.md

![[Visual Studio show all files.png]]
### Python debugging

The key thing is to have a project first, doesn't seem to support command line parameters if you just open a folder

1. Click the project e.g. `hal_md` 
2. Select `Project` menu then `Properties` at the bottom
3. Click the `Debug` tab
4. Fill in `Script Arguments`

![[Python Debug in Visual Studio.png]]

### Once you're debugging

- To see debug values: `Debug -> Windows -> Locals`

### Also saw this but don't know if it works

- right-click on the `.py` file:
	- `Add Debug Configuration`
- to edit, right-click on the `.py` file:
	- `Open Debug and Launch Settings`
- right-click on the `.py` file and 'Set as Startup Item'

![[Pasted image 20240404093952.png]]