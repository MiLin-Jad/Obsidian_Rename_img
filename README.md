# Image Auto Rename

  

An Obsidian plugin that automatically renames newly created or pasted images, along with small tools for managing file lists, Bases, and themes.

## Version

Current version: `1.0.2`

## Default Settings

- `Image filename display`: `Show on hover`  

- `Hide PNG files in file list`: Enabled  

- `Use Baseline theme`: Enabled  

- `Auto reveal active file in file list`: Disabled  

- `Add Base name style rule` Default rules:  

- `canvas`: `#f9a8d4`  

- `md`: `#3f3f46`

## Main Features

- Automatically rename images when creating, pasting, or within the current file.  

- After pasting and renaming images, automatically update image references in Markdown and Canvas to reduce occasional "image not found" issues.  

- Hide `png` files from the file list.  

- Control how Canvas displays image filenames: show always, hide, or show on hover.  

- Enable or disable "auto-scroll file list to current file."  

- Create a default `Files.base` with built-in rules: - `file.ext is not png`

- `file.ext is not base`

- Default Base attributes include:

- Name

- Extension - tags

- aliases

- File backlinks  

- Modification time  

- Multiple Base name style rules can be added, allowing you to set text color and boldness for names based on file extensions.  

- Base name style colors support both hexadecimal input and color picker.  

- After plugin loading, it will attempt to install and enable the Baseline theme from `baseline-theme.css` and `baseline-manifest.json` in the plugin directory.




## Building

```bash

npm run build

```