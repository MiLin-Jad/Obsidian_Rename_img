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
## Baseline Theme 
Please keep the theme file in the root directory of the plugin: 
```text
Copy image/
baseline-manifest.json
baseline-theme.css
```

After enabling `Use Baseline theme`, the plugin will copy the theme to the current vault's `.obsidian/themes/Baseline/` directory and then attempt to switch to the `Baseline` theme. 
## Uploading Files to GitHub 
Suggested to upload these files: 
- `manifest.json`
- `main.js`
- `main.ts`
- `build.js`
- `package.json`
- `package-lock.json`
- `tsconfig.json`
- `README.md`
- `CHANGELOG.md`
- `.gitignore`
- `baseline-manifest.json`
- `baseline-theme.css`

It is not recommended to upload the `node_modules/` folder. This directory can be deleted, and dependencies can be restored by running `npm install` when rebuilding. 
## Building 
```bash
npm run build
```