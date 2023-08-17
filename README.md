## Pretty Pink - Syntax Theme

Pretty Pink is a syntax highlight theme for Visual Studio Code. It tries to highlight in mostly analogous, but still distinguishable colors from the magenta and pink region with a bit of contrast sprinkled in. It was made for people who don't like overly colorful highlights and instead prefer a more uniform and muted color scheme.

![Preview image](https://raw.githubusercontent.com/nptr/pretty-pink/master/images/preview.png)

---

![Preview image 2](https://raw.githubusercontent.com/nptr/pretty-pink/master/images/preview2.png)


### Installation

**Automatically:** From the extensions tab within VSCode, search for and install 'Pretty Pink Syntax Theme'. Once installed, themes can be switched using the menu item `File -> Preferences -> Color Theme` or via `Ctrl+K Ctrl+T`.

**Manually:** Copy or clone the repository into `~/.vscode/extensions/` and restart the editor.

---

### Advanced Modification

**Bracket Colorization:** VSCode supports different bracket colors based on nesting level. This theme disables that by using one color for all pairs.

* Change or remove the `editorBracketHighlight.foregroundX` key in `~/.vscode/extensions/themes/pretty-pink-XXXX.json`

**Status Bar Color:** This theme changes the status bar color, which might not fit everybody.

* Change or remove the `statusBar.XXXX` keys in `~/.vscode/extensions/themes/pretty-pink-XXXX.json`

**Editor Inlays:** VSCode can annotate your code with hints for certain languages. The default look is rather ugly with a strong background color. Without the background, distinction between inlay and actual code can be a bit hard. A custom font and/or font size can help here, but must be done in user settings:

* Press Ctrl+Shift+P, type _"user settings"_, select _"Preferences: Open User Settings (JSON)"_. The recommended settings are as follows, but can be changed to your liking.

```json
{
    // advanced inlay modification
    "editor.inlayHints.fontFamily": "Monospace",
    "editor.inlayHints.fontSize": 12,

    // ... other settings
}
```