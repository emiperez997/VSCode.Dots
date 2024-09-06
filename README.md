# Guía y configuración de Visual Studio Code

## Extensions

- Angular Language Service
- Docker
- Error Lens
- Icons
- Kanagawa
- Live Preview
- NERDTree
- Prettier
- Prisma
- Supermaven
- Tailwind CSS InteliSense
- Vim
- WSL

## User Settings (JSON)

```json
{
  // Editor
  "editor.cursorBlinking": "expand",
  "editor.formatOnSave": true,
  "editor.glyphMargin": false,
  "editor.hideCursorInOverviewRuler": true,
  "editor.inlineSuggest.enabled": true,
  "editor.lineNumbers": "relative",
  "editor.minimap.enabled": false,
  "editor.overviewRulerBorder": false,
  "editor.scrollbar.vertical": "auto",
  "editor.lineNumbers": "relative",
  "editor.suggest.insertMode": "replace",
  "editor.linkedEditing": true,
  "breadcrumbs.enabled": false,
  "editor.tabSize": 2,

  // Javascript Settings
  "javascript.updateImportsOnFileMove.enabled": "always",

  // Vim
  "vim.useSystemClipboard": true,
  "vim.highlightedyank.enable": true,
  "vim.hlsearch": true,
  "vim.autoindent": true,
  "vim.handleKeys": {
    "<C-d>": false,
    "<C-n>": false,
    "<C-s>": false,
    "<C-z>": false
  },
  "vim.insertModeKeyBindings": [
    {
      "after": ["<Esc>"],
      "before": ["k", "j"]
    }
  ],
  "vim.leader": "<space>",
  "vim.normalModeKeyBindingsNonRecursive": [
    // Navigation
    { "before": ["<S-h>"], "commands": [":bprevious"] },
    { "before": ["<S-l>"], "commands": [":bnext"] },

    // Splits
    { "before": ["<leader>", "v"], "commands": [":vsplit"] },
    { "before": ["<leader>", "s"], "commands": [":split"] },

    // Panes
    { "before": ["<C-h>"], "commands": ["workbench.action.focusLeftGroup"] },
    { "before": ["<C-j>"], "commands": ["workbench.action.focusBelowGroup"] },
    { "before": ["<C-k>"], "commands": ["workbench.action.focusAboveGroup"] },
    { "before": ["<C-l>"], "commands": ["workbench.action.focusRightGroup"] },

    //   // Nice to have
    { "before": ["<leader>", "w"], "commands": [":w!"] },
    { "before": ["<leader>", "q"], "commands": [":q!"] },
    { "before": ["<leader>", "x"], "commands": [":x"] },
    { "before": ["<leader>", "f"], "commands": ["workbench.action.quickOpen"] }
  ],
  "vim.visualModeKeyBindings": [
    { "before": ["<leader>", "c"], "commands": ["editor.action.commentLine"] }
  ],
    "vim.statusBarColors.visualline": "#005f5f",

  // NERDTree
  "nerdtree.alwaysShowSidebar": false,

  // Prettier
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  // Theme
  "terminal.integrated.fontFamily": "'IosevkaTerm Nerd Font Mono'",
  "editor.fontFamily": "'IosevkaTerm Nerd Font Mono'",
  "workbench.colorTheme": "Kanagawa",
  "workbench.iconTheme": "icons",
  "editor.fontLigatures": true,
  "window.zoomLevel": 0,
  "explorer.compactFolders": false,

  "workbench.activityBar.location": "hidden",
  "workbench.colorCustomizations": {
    "editorCodeLens.foreground": "#bbb",
    "terminalCursor.foreground": "#bbb",
    "statusBar.background": "#005f5f",
    "statusBar.noFolderBackground": "#005f5f",
    "statusBar.debuggingBackground": "#005f5f",
    "statusBar.foreground": "#ffffff"
  },
  "vim.statusBarColors.visualline": "#005f5f",
}
```

## Keyboard Settings (JSON)

```json
// Place your key bindings in this file to override the defaults
[ 
  {
    "key": "ctrl+shift+a",
    "command": "workbench.action.terminal.focusNext",
    "when": "terminalFocus"
  },
  {
    "key": "ctrl+shift+b",
    "command": "workbench.action.terminal.focusPrevious",
    "when": "terminalFocus"
  },
  {
    "key": "ctrl+t",
    "command": "workbench.action.terminal.toggleTerminal",
    "when": "terminal.active"
  },
  {
    "command": "workbench.action.toggleSidebarVisibility",
    "key": "ctrl+e"
  },
  {
    "command": "workbench.files.action.focusFilesExplorer",
    "key": "ctrl+h",
    "when": "editorTextFocus"
  }
]
```
