# Guía y configuración de Visual Studio Code

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

  // Vim
  "vim.useSystemClipboard": true,
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
    {
      "before": ["<leader>", "w"],
      "commands": [":w"]
    },
    {
      "before": ["<leader>", "q"],
      "commands": [":q"]
    }
  ],

  // NERDTree
  "nerdtree.alwaysShowSidebar": false,

  // Prettier
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },

  // Workbench
  "workbench.colorTheme": "Kanagawa"
}
```

## Keyboard Settings (JSON)

```json
// Place your key bindings in this file to override the defaults
[
  {
    "key": "shift+h",
    "command": "workbench.action.previousEditor",
    "when": "editorTextFocus"
  },
  {
    "key": "shift+l",
    "command": "workbench.action.nextEditor",
    "when": "editorTextFocus"
  },
  {
    "key": "ctrl+t",
    "command": "workbench.action.terminal.toggleTerminal",
    "when": "terminal.active"
  },
  {
    "key": "ctrl+n",
    "command": "nerdtree.unfocusSidebarOrClose",
    "when": "filesExplorerFocus && sideBarVisible"
  },
  {
    "key": "ctrl+n",
    "command": "-nerdtree.unfocusSidebarOrClose",
    "when": "filesExplorerFocus && sideBarVisible"
  }
]
```
