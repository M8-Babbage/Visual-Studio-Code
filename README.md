# Visual Studio Code

[Setup with VIM](./VIM.md)

[Normal setup](./NORMAL.md)

**Unificada**
    
```jsx
code --install-extension Angular.ng-template
code --install-extension Avetis.tokyo-night
code --install-extension christian-kohler.path-intellisense
code --install-extension ecmel.vscode-html-css
code --install-extension GitHub.copilot
code --install-extension LeonardSSH.vscord
code --install-extension meganrogge.template-string-converter
code --install-extension PKief.material-icon-theme
code --install-extension ryuta46.multi-command
code --install-extension vscodevim.vim
code --install-extension Vue.volar
code --install-extension Vue.vscode-typescript-vue-plugin
```
    
```jsx
[
  // Terminal settings
  {
    "key": "shift+n",
    "command": "workbench.action.terminal.new",
    "when": "terminalFocus"
  },
  {
    "key": "shift+q",
    "command": "workbench.action.terminal.kill",
    "when": "terminalFocus"
  },
  {
    "key": "shift+j",
    "command": "workbench.action.terminal.focusNext",
    "when": "terminalFocus"
  },
  {
    "key": "shift+k",
    "command": "workbench.action.terminal.focusPrevious",
    "when": "terminalFocus"
  },
  // General settings
  {
    "key": "alt+k",
    "when": "editorTextFocus && !editorReadonly",
    "command": "editor.action.moveLinesUpAction"
  },
  {
    "key": "alt+j",
    "when": "editorTextFocus && !editorReadonlyc",
    "command": "editor.action.moveLinesDownAction"
  },
  {
    "key": "ctrl+k",
    "when": "inQuickOpen",
    "command": "workbench.action.quickOpenSelectPrevious"
  },
  {
    "key": "ctrl+j",
    "when": "inQuickOpen",
    "command": "workbench.action.quickOpenSelectNext"
  },
  {
    "key": "shift+k",
    "command": "workbench.action.nextEditor",
    "when": "!terminalFocus"
  },
  {
    "key": "shift+j",
    "command": "workbench.action.previousEditor",
    "when": "!terminalFocus"
  },
  {
    "key": "ctrl+k",
    "when": "suggestWidgetMultipleSuggestions",
    "command": "selectPrevSuggestion",
  },
  {
    "key": "ctrl+j",
    "when": "suggestWidgetMultipleSuggestions",
    "command": "selectNextSuggestion",
  },
  // Utilities settings
  {
    "key": "alt+e",
    "command": "editor.emmet.action.wrapWithAbbreviation"
  },
  {
    "key": "ctrl+shift+b",
    "command": "workbench.action.toggleActivityBarVisibility",
  },
  {
    "key": "ctrl+b",
    "command": "workbench.action.toggleSidebarVisibility",
  },
  {
    "key": "ctrl+shift+j",
    "command": "workbench.action.terminal.toggleTerminal"
  },
  // Vim Settings
  {
    "key": "a",
    "command": "explorer.newFile",
    "when": "!inputFocus && !activeWebviewPanelId"
  },
  {
    "key": "c",
    "command": "explorer.newFolder",
    "when": "!inputFocus && !activeWebviewPanelId"
  },
  {
    "key": "r",
    "command": "renameFile",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus && !activeWebviewPanelId"
  },
  {
    "key": "d",
    "command": "deleteFile",
    "when": "!inputFocus && !activeWebviewPanelId"
  },
  {
    "key": "ctrl+h",
    "command": "workbench.action.navigateLeft",
    "when": "!inQuickOpen && !suggestWidgetVisible",
  },
  {
    "key": "ctrl+l",
    "command": "workbench.action.navigateRight",
    "when": "!inQuickOpen && !suggestWidgetVisible",
  },
  {
    "key": "ctrl+k",
    "command": "workbench.action.navigateUp",
    "when": "!inQuickOpen && !suggestWidgetVisible",
  },
  {
    "key": "ctrl+j",
    "command": "workbench.action.navigateDown",
    "when": "!inQuickOpen && !suggestWidgetVisible",
  },
]
```

```jsx
{
  // Workbench settings
  "workbench.startupEditor": "none",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Tokyo Night Gogh",
  "workbench.sideBar.location": "right",
  "workbench.editor.showTabs": true,
  "workbench.editor.tabCloseButton": "off",
  "workbench.statusBar.visible": false,
  "workbench.colorCustomizations": { // Can customize each aspect
    "tab.activeBackground": "#7fa9e020",
    "tab.activeBorder": "#417ff1"
  },
  // Editor settings
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.smoothScrolling": true,
  "editor.cursorBlinking": "expand",
  "editor.occurrencesHighlight": false,
  "editor.wordWrap": "on",
  "editor.overviewRulerBorder": false,
  "editor.hideCursorInOverviewRuler": true,
  "editor.scrollbar.vertical": "auto",
  "editor.codeActionsOnSave": {
    "source.organizeImports": true
  },
  "editor.glyphMargin": false,
  "editor.fontLigatures": true,
  "editor.fontFamily": "Cascadia Code, Consolas, 'Courier New', monospace",
  "editor.inlineSuggest.enabled": true,
  "editor.linkedEditing": true,
  "editor.minimap.enabled": false,
  "editor.bracketPairColorization.enabled": true,
  "editor.tabSize": 2,
  "editor.formatOnSave": true,
  "editor.guides.indentation": false,
  // Window settings  
  "window.menuBarVisibility": "toggle",
  // Explorer settings
  "explorer.compactFolders": false,
  // General settings
  "terminal.integrated.fontFamily": "Cascadia Code, Consolas, 'Courier New', monospace",
  "breadcrumbs.enabled": false,
  "html.hover.documentation": false,
  "html.hover.references": false,
  "git.autofetch": true,
  "css.styleSheets": [
    // "https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css",
    "https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/css/bootstrap.min.css"
  ],
  "css.enabledLanguages": [
    "html"
  ],
  "explorer.confirmDelete": false,
  "volar.inlayHints.eventArgumentInInlineHandlers": false,
  "javascript.updateImportsOnFileMove.enabled": "always",
  // Vim settings
  "editor.lineNumbers": "relative",
  "vim.easymotion": true,
  "vim.leader": "<space>",
  "vim.startInInsertMode": false,
  "vim.useCtrlKeys": true,
  "vim.useSystemClipboard": true,
  "vim.normalModeKeyBindingsNonRecursive": [
    {
      "before": [
        "j"
      ],
      "after": [
        "g",
        "j"
      ]
    },
    {
      "before": [
        "k"
      ],
      "after": [
        "g",
        "k"
      ]
    },
    {
      "before": [
        "d"
      ],
      "after": [
        "\"",
        "_",
        "d"
      ]
    },
    {
      "before": [
        "D"
      ],
      "after": [
        "\"",
        "_",
        "D"
      ]
    },
    {
      "before": [
        "d",
        "d"
      ],
      "after": [
        "\"",
        "_",
        "d",
        "d"
      ]
    },
    {
      "before": [
        "<BS>"
      ],
      "after": [
        "\"",
        "_",
        "d"
      ]
    },
    {
      "before": [
        "<Del>"
      ],
      "after": [
        "\"",
        "_",
        "d"
      ]
    },
    // Atajo para el easy motion
    {
      "before": [
        "leader",
        "s"
      ],
      "after": [
        "leader",
        "leader",
        "2",
        "s"
      ]
    },
    // Punto y coma al final de la linea
    {
      "before": [
        "leader",
        ";"
      ],
      "after": [
        "$",
        "a",
        ";",
        "<Esc>"
      ]
    },
    // Coma al final de la línea
    {
      "before": [
        "leader",
        ","
      ],
      "after": [
        "$",
        "a",
        ",",
        "<Esc>"
      ]
    },
    // Scroll rápido hacia abajo
    {
      "before": [
        "J"
      ],
      "after": [
        "9",
        "<C-e>"
      ]
    },
    // Scroll rápido hacia arriba
    {
      "before": [
        "K"
      ],
      "after": [
        "9",
        "<C-y>"
      ]
    },
    // Guardar archivo actual
    {
      "before": [
        "leader",
        "w"
      ],
      "after": [
        ":",
        "w",
        "<CR>"
      ]
    },
    // Cerrar archivo actual
    {
      "before": [
        "leader",
        "q"
      ],
      "after": [
        ":",
        "q",
        "<CR>"
      ]
    },
    // Abrir modal con archivos recientes
    {
      "before": [
        "leader",
        "f"
      ],
      "commands": [
        "workbench.action.showAllEditors"
      ]
    },
    // Cerrar todos los buffers
    {
      "before": [
        "leader",
        "Q"
      ],
      "commands": [
        "workbench.action.closeAllEditors"
      ]
    },
    // Seleccionar todo
    {
      "before": [
        "<c-a>"
      ],
      "after": [
        "g",
        "g",
        "0",
        "v",
        "G",
        "$"
      ]
    },
    {
      "before": [
        "<C-c>"
      ],
      "after": [
        "\"",
        "+",
        "y"
      ]
    },
    {
      "before": [
        "<C-v>"
      ],
      "after": [
        "\"",
        "+",
        "p"
      ]
    }
  ],
  // Salir de modo insert
  "vim.insertModeKeyBindings": [
    {
      "before": [
        "j",
        "j"
      ],
      "after": [
        "<Esc>"
      ]
    }
  ],
  // Configuraciones visuales VIM
  "vim.visualModeKeyBindings": [
    {
      "before": [
        ">"
      ],
      "commands": [
        "editor.action.indentLines"
      ]
    },
    {
      "before": [
        "<"
      ],
      "commands": [
        "editor.action.outdentLines"
      ]
    },
    {
      "before": [
        "<C-c>"
      ],
      "after": [
        "\"",
        "+",
        "y"
      ]
    },
    {
      "before": [
        "<C-v>"
      ],
      "after": [
        "\"",
        "+",
        "p"
      ]
    }
  ],
  "vim.visualModeKeyBindingsNonRecursive": [
    {
      "before": [
        "d"
      ],
      "after": [
        "\"",
        "_",
        "d"
      ]
    },
    {
      "before": [
        "D"
      ],
      "after": [
        "\"",
        "_",
        "D"
      ]
    },
    {
      "before": [
        "d",
        "d"
      ],
      "after": [
        "\"",
        "_",
        "d",
        "d"
      ]
    },
    {
      "before": [
        "<BS>"
      ],
      "after": [
        "\"",
        "_",
        "d"
      ]
    },
    {
      "before": [
        "<Del>"
      ],
      "after": [
        "\"",
        "_",
        "d"
      ]
    }
  ],
}
```