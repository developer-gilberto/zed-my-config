# Zed settings
Para ativar essas configuracoes, basta colar os seguintes arquivos json "settings.json" e "keymap.json" no diretorio: /home/gilberto/.config/zed
salvar e pronto, as configs ja estarao funcionando.

## settings.json:
{
    "context_servers": {},
    "agent": {
        "default_profile": "write",
        "default_model": {
            "provider": "copilot_chat",
            "model": "gpt-4.1"
        },
        "single_file_review": true,
        "always_allow_tool_actions": false,
        "model_parameters": [],
        "dock": "left"
    },
    "git_panel": {
        "dock": "right"
    },
    "tab_size": 4,
    "scrollbar": { "show": "auto" },
    "icon_theme": "Material Icon Theme",
    "base_keymap": "VSCode",
    "buffer_font_family": "JetBrains Mono NL",
    "ui_font_size": 16,
    "buffer_font_size": 16,
    "preferred_line_length": 80,
    "soft_wrap": "preferred_line_length",
    "theme": {
        "mode": "dark",
        "light": "One Light",
        "dark": "Dracula Solid"
    },
    "terminal": {
        "blinking": "on",
        "font_family": "JetBrains Mono NL",
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
