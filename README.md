# Zed settings
Para ativar essas configuracoes, basta colar os seguintes arquivos json "settings.json", "keymap.json" e o diretorio themes no diretorio: /home/gilberto/.config/zed
salvar e pronto, as configs ja estarao funcionando.

## settings.json:
{
    "features": {
        "edit_prediction_provider": "none"
    },
    "notification_panel": {
        "dock": "right"
    },
    "context_servers": {},

    "git_panel": {
        "dock": "right"
    },
    "tab_size": 4,
    "scrollbar": { "show": "auto" },
    "icon_theme": "Zed (Default)",
    "base_keymap": "VSCode",
    "buffer_font_family": "JetBrains Mono NL",
    "ui_font_size": 16,
    "buffer_font_size": 16,
    "preferred_line_length": 80,
    "soft_wrap": "preferred_line_length",
    "diagnostics": {
        "button": true,
        "include_warnings": true,
        "lsp_pull_diagnostics": {
            "enabled": true,
            "debounce_ms": 50
        },
        "inline": {
            "enabled": true,
            "update_debounce_ms": 150,
            "padding": 4,
            "min_column": 0,
            "max_severity": null
        }
    },
    "theme": {
        "mode": "dark",
        "light": "One Light",
        "dark": "One Dark"
    },
    "terminal": {
        "blinking": "on",
        "font_family": "MesloLGL Nerd Font Mono",
        "cursor_shape": "bar"
    },
    "current_line_highlight": "none",
    "project_panel": {
        "button": true,
        "default_width": 240,
        "dock": "right",
        "entry_spacing": "comfortable",
        "file_icons": true,
        "folder_icons": true,
        "git_status": true,
        "indent_size": 20,
        "auto_reveal_entries": true,
        "auto_fold_dirs": false,
        "scrollbar": {
            "show": "auto"
        },
        "show_diagnostics": "all",
        "indent_guides": {
            "show": "always"
        },
        "hide_root": false
    }
}

## keymap.json
[
    {
        "context": "Workspace",
        "bindings": {
            // "shift shift": "file_finder::Toggle"
            "ctrl-alt-b": "workspace::ToggleLeftDock",
            "ctrl-b": "workspace::ToggleRightDock"
        }
    },
    {
        "context": "Editor",
        "bindings": {
            // "j k": ["workspace::SendKeystrokes", "escape"]
            "alt-shift-down": "editor::DuplicateLineDown",
            "alt-shift-up": "editor::DuplicateLineUp"
        }
    }
]
