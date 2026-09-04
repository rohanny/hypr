# VS Code Custom Configuration

This folder contains your VS Code settings, custom UI styles, and keybindings.

## Files

- `settings.json`: Your editor configuration including typography, formatting, and the inline `custom-ui-style.stylesheet` rules.
- `custom.css`: Standalone stylesheet containing all custom CSS rules (floating rounded cards, pill-shaped activity bar, custom breadcrumbs, status bar, and dialog styles).
- `keybindings.json`: Custom keybindings (`alt+x` vim toggle, `alt+q` vim escape, terminal toggles, chat bindings).

## Applying Custom CSS on VS Code

### Option 1: Using `custom-ui-style` Extension
1. Install the **Custom UI Style** extension in VS Code.
2. Ensure the `"custom-ui-style.stylesheet"` block in `settings.json` is present in your VS Code `settings.json`.
3. Reload VS Code.

### Option 2: Using `vscode-custom-css` Extension
1. Install **Custom CSS and JS Loader** (`be5invis.vscode-custom-css`).
2. Add the path to `custom.css` in your `settings.json`:
   - **Linux**: `"vscode_custom_css.imports": ["file:///home/<user>/.config/vscode/custom.css"]`
   - **Windows**: `"vscode_custom_css.imports": ["file:///C:/Users/<user>/hypr/vscode/custom.css"]`
3. Press `Ctrl + Shift + P` (or `Cmd + Shift + P`) and run **Enable Custom CSS and JS**.
4. Restart VS Code.
