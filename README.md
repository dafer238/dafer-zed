# Zed Editor Configuration

Personal Zed editor configuration optimized for Vim-style workflow with Python development support.

## 📁 Files Overview

- `keymap.json` - Custom keybindings with Vim-centric navigation
- `settings.json` - Editor appearance, behavior, and language configurations
- `tasks.json` - Quick run tasks for multiple languages
- `debug.json` - Debug configurations for Python and JavaScript
- `themes/` - Custom color schemes
- `snippets/` - Code snippets

## ⌨️ Keymaps

### Navigation (Normal Mode)
- `Ctrl+h/j/k/l` - Navigate between panes (left/down/up/right)
- `Alt+j/k` - Switch between tabs (previous/next)
- `Ctrl+u/d` - Scroll up/down (centered)
- `n` - Next search match (centered)

### Leader Key Shortcuts (Space)
- `Space Space` - Tab switcher
- `Space f m` - Format document
- `Space s f` - File finder
- `Space s g` - Project search
- `Space c a` - Code actions
- `Space d b` - Start debugger
- `Space s n` - Open settings
- `Space t` - Toggle project panel
- `Space g g` - Toggle git panel
- `Space r` - Run task

### Other Bindings
- `;` - Command palette (Normal mode)
- `j k` - Exit insert mode (Insert mode)
- `F2` - Rename symbol
- `Ctrl+Alt+t` - New terminal
- `Ctrl+w` - Close active item/dock

## 🚀 Tasks

### Python
- **Run (Python)** - Executes Python files using the currently selected interpreter
  - Uses: `$ZED_PYTHON` (respects active environment)
  - Working directory: Project root

### Python (UV)
- **Run (uv)** - Executes Python files using UV package manager

### Rust
- **Run (cargo)** - Builds and runs Rust projects

### Zig
- **Run (zig)** - Builds and runs Zig projects

### C/C++
- **Run (C/C++ - Linux/Windows)** - Compiles with Clang and executes
  - Platform-specific variants for Windows and Linux

## 🐛 Debug Configurations

### Python
- **Debug active Python file**
  - Adapter: Debugpy
  - Runs current file from project root

### JavaScript
- **Debug active JavaScript file**
  - Adapter: JavaScript (pwa-node)
  - Runs current file from project root

- **JavaScript debug terminal**
  - Interactive debugging in integrated terminal

## ⚙️ Settings Highlights

### Appearance
- **Font**: Cascadia Code (18pt buffer, 18pt UI)
- **Theme**: Gruvbox (system-aware dark/light)
- **Icons**: Material Icon Theme
- **Line Length**: 100 characters

### Editor Behavior
- **Vim Mode**: Enabled
- **Autosave**: On focus change
- **Format on Save**: Enabled
- **Scroll Margin**: 5 lines

### Python Configuration
- **Language Servers**: Ruff, Ty
- **Debugger Timeout**: 10 seconds

### Terminal
- **Font Size**: 14pt
- **Copy on Select**: Enabled
- **Working Directory**: Current project directory

### AI Assistant
- **Model**: Claude Sonnet 4.5 (via Copilot Chat)
- **Default Profile**: Write
- **Auto-allow Tool Actions**: Enabled
- **Notifications**: All screens
- **Sound on Completion**: Enabled

## 🎯 Workflow Philosophy

This configuration is optimized for:
- **Vim-style navigation** with minimal hand movement
- **Python development** with virtual environment support
- **Quick task execution** for multiple languages
- **Centered scrolling** for better focus
- **Minimal UI distractions** (no breadcrumbs, reduced toolbar)

## 📝 Notes

- All Python tasks automatically use the selected Python environment via `$ZED_PYTHON`
- Tasks run from project root for consistent import resolution
- Keybindings work across all panels (editor, terminal, git, debug)
- Diagnostics show inline at column 50+ to avoid code clutter

## 🔗 Resources

- [Zed Documentation](https://zed.dev/docs)
- [Key Bindings Guide](https://zed.dev/docs/key-bindings)
- [Configuring Zed](https://zed.dev/docs/configuring-zed)
