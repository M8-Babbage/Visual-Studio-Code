
- **VIM**
    
    ```jsx
    code --install-extension ryuta46.multi-command
    code --install-extension vscodevim.vim
    ```
    
    ```jsx
    {
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
            "workbench.action.quickOpen"
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
    
    ```jsx
    [
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
      // Vim settings
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
    ]
    ```