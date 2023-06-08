- **Normal**
    
    ```jsx
    code --install-extension Angular.ng-template
    code --install-extension Avetis.tokyo-night
    code --install-extension christian-kohler.path-intellisense
    code --install-extension ecmel.vscode-html-css
    code --install-extension GitHub.copilot
    code --install-extension LeonardSSH.vscord
    code --install-extension meganrogge.template-string-converter
    code --install-extension ms-vscode-remote.remote-wsl
    code --install-extension PKief.material-icon-theme
    code --install-extension Vue.volar
    code --install-extension Vue.vscode-typescript-vue-plugin
    ```
    
    ```jsx
    {
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
        // "https://unpkg.com/primeflex@^3/primeflex.css",
      ],
      "css.enabledLanguages": [
        "html"
      ],
      "editor.inlineSuggest.enabled": true,
      "explorer.confirmDelete": false,
      "volar.inlayHints.eventArgumentInInlineHandlers": false,
      "javascript.updateImportsOnFileMove.enabled": "always"
    }
    }
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
  // Show open tabs
  {
    "key": "ctrl+oem_3",
    "command": "workbench.action.showAllEditors"
  },
  {
    "key": "ctrl+[Semicolon]",
    "command": "workbench.action.showAllEditors"
  },
  {
    "key": "ctrl+enter",
    "command": "-github.copilot.generate",
    "when": "editorTextFocus && github.copilot.activated && !inInteractiveInput && !interactiveEditorFocused"
  },
  ]
  ```