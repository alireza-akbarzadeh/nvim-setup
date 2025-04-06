# 🚀 Modern Neovim Configuration

<div align="center">

![Neovim](https://img.shields.io/badge/NeoVim-%2357A143.svg?&style=for-the-badge&logo=neovim&logoColor=white)
![Lua](https://img.shields.io/badge/lua-%232C2D72.svg?style=for-the-badge&logo=lua&logoColor=white)

</div>

A modern, feature-rich Neovim configuration focused on providing an excellent development experience with a clean, minimalist interface. This configuration uses Lazy.nvim for plugin management and is written entirely in Lua.

## ✨ Features

- 🔍 **Fuzzy Finding**: Fast file navigation with Telescope
- 🌳 **File Explorer**: Easy file browsing with NvimTree
- 🎨 **Beautiful UI**: Custom Tokyo Night theme with Lualine status bar
- 🔌 **LSP Support**: Integrated language servers for intelligent code completion
- 🧩 **Autocompletion**: Smart suggestions with nvim-cmp
- 🔄 **Auto Pairs**: Automatic bracket and quote pairing
- 🔍 **Syntax Highlighting**: Enhanced syntax highlighting with Treesitter
- 📝 **Formatting & Linting**: Automatic code formatting and linting
- 🔧 **Git Integration**: Git status in the editor with Gitsigns
- 📊 **Session Management**: Auto-session for persistent workspaces
- 🔑 **Which Key**: Keybinding hints with which-key

## 📋 Prerequisites

- Neovim >= 0.8.0
- Git
- A [Nerd Font](https://www.nerdfonts.com/) (optional, but recommended for icons)
- Node.js and npm (for LSP features)
- Ripgrep (for Telescope grep functionality)

## 🔧 Installation

1. Backup your existing Neovim configuration if you have one:

```bash
mv ~/.config/nvim ~/.config/nvim.backup
```

2. Clone this repository:

```bash
git clone https://github.com/yourusername/nvim-config.git ~/.config/nvim
```

3. Start Neovim:

```bash
nvim
```

The configuration will automatically install Lazy.nvim and all the plugins on the first run.

## ⌨️ Key Mappings

> Leader key is set to `Space`

### General

| Mapping | Description |
| --- | --- |
| `jk` | Exit insert mode |
| `<leader>nh` | Clear search highlights |
| `<leader>+` | Increment number |
| `<leader>-` | Decrement number |

### Window Management

| Mapping | Description |
| --- | --- |
| `<leader>sv` | Split window vertically |
| `<leader>sh` | Split window horizontally |
| `<leader>se` | Make splits equal size |
| `<leader>sx` | Close current split |

### Tab Management

| Mapping | Description |
| --- | --- |
| `<leader>to` | Open new tab |
| `<leader>tx` | Close current tab |
| `<leader>tn` | Go to next tab |
| `<leader>tp` | Go to previous tab |
| `<leader>tf` | Open current buffer in new tab |

### File Explorer (NvimTree)

| Mapping | Description |
| --- | --- |
| `<leader>ee` | Toggle file explorer |
| `<leader>ef` | Toggle file explorer on current file |
| `<leader>ec` | Collapse file explorer |
| `<leader>er` | Refresh file explorer |

### Telescope

| Mapping | Description |
| --- | --- |
| `<leader>ff` | Find files |
| `<leader>fr` | Find recent files |
| `<leader>fs` | Find string in files |
| `<leader>fc` | Find string under cursor |
| `<leader>ft` | Find TODOs |

### LSP

| Mapping | Description |
| --- | --- |
| `gR` | Show LSP references |
| `gD` | Go to declaration |
| `gd` | Show LSP definitions |
| `gi` | Show LSP implementations |
| `gt` | Show LSP type definitions |
| `<leader>ca` | See available code actions |
| `<leader>rn` | Smart rename |
| `<leader>D` | Show buffer diagnostics |
| `<leader>d` | Show line diagnostics |
| `K` | Show documentation for what is under cursor |

### Formatting

| Mapping | Description |
| --- | --- |
| `<leader>mp` | Format file or range |

## 🧩 Plugins

This configuration uses the following plugins:

### Core
- [lazy.nvim](https://github.com/folke/lazy.nvim) - Plugin manager
- [plenary.nvim](https://github.com/nvim-lua/plenary.nvim) - Lua functions library
- [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) - Seamless navigation between tmux panes and vim splits

### UI
- [tokyonight.nvim](https://github.com/folke/tokyonight.nvim) - Tokyo Night colorscheme
- [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim) - Status line
- [nvim-web-devicons](https://github.com/nvim-tree/nvim-web-devicons) - Icons
- [alpha-nvim](https://github.com/goolord/alpha-nvim) - Dashboard
- [bufferline.nvim](https://github.com/akinsho/bufferline.nvim) - Buffer line
- [indent-blankline.nvim](https://github.com/lukas-reineke/indent-blankline.nvim) - Indentation guides

### Editor
- [nvim-tree.lua](https://github.com/nvim-tree/nvim-tree.lua) - File explorer
- [telescope.nvim](https://github.com/nvim-telescope/telescope.nvim) - Fuzzy finder
- [nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter) - Syntax highlighting
- [nvim-autopairs](https://github.com/windwp/nvim-autopairs) - Auto pairs
- [Comment.nvim](https://github.com/numToStr/Comment.nvim) - Easy commenting
- [vim-surround](https://github.com/tpope/vim-surround) - Surround selections
- [vim-maximizer](https://github.com/szw/vim-maximizer) - Maximize split windows

### LSP & Completion
- [nvim-lspconfig](https://github.com/neovim/nvim-lspconfig) - LSP configuration
- [mason.nvim](https://github.com/williamboman/mason.nvim) - LSP installer
- [nvim-cmp](https://github.com/hrsh7th/nvim-cmp) - Completion engine
- [LuaSnip](https://github.com/L3MON4D3/LuaSnip) - Snippet engine

### Git
- [gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim) - Git integration
- [lazygit.nvim](https://github.com/kdheepak/lazygit.nvim) - Git UI

### Utilities
- [which-key.nvim](https://github.com/folke/which-key.nvim) - Keybinding helper
- [auto-session](https://github.com/rmagatti/auto-session) - Session management
- [conform.nvim](https://github.com/stevearc/conform.nvim) - Formatting
- [trouble.nvim](https://github.com/folke/trouble.nvim) - Pretty diagnostics
- [todo-comments.nvim](https://github.com/folke/todo-comments.nvim) - Highlight TODO comments

## 🎨 Customization

This configuration is designed to be easily customizable. Most settings are in the `lua/josean/core/options.lua` and `lua/josean/core/keymaps.lua` files.

To add or modify plugins, check the files in the `lua/josean/plugins/` directory.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [Josean Martinez](https://github.com/josean-dev) for the inspiration and tutorials
- [NvChad](https://github.com/NvChad/NvChad) for UI inspiration
- [LunarVim](https://github.com/LunarVim/LunarVim) for some configuration ideas

---

<div align="center">

⭐ If you found this configuration helpful, please consider giving it a star! ⭐

</div>