# Cole

A stationery-inspired theme with vintage earth tones.

![Screenshot of Neovim with Cole colorscheme](https://raw.githubusercontent.com/thekylehuang/cole/refs/heads/main/.github/assets/social-banner.png)

## About

Cole was inspired by the look and feel of [LEUCHTTURM1917](https://www.leuchtturm1917.us) notebooks.

Designed to be an ergonomic color scheme, Cole has restrained yet contrasted colors for long hours of staring at a terminal. The background consists of a grey-black which provides a warm foundation without the harshness of a true OLED black. The look and feel is between a retro theme like [gruvbox](https://github.com/morhetz/gruvbox) and a soft matte theme like [everforest](https://github.com/sainnhe/everforest).

## Installation

The Cole colorscheme is supported on many different tools. There are separate repositories containing Cole for ![Neovim](https://github.com/thekylehuang/cole.nvim) and for ![Tmux](https://github.com/thekylehuang/cole-tmux).

### Terminals

Refer to `./terminals/` for the terminal emulator you use. Each folder contains a README with installation instructions.

## Palette

![Color palette of the Cole colorscheme](https://raw.githubusercontent.com/thekylehuang/cole/main/.github/assets/palette.png)

## Contribution

Thank you for wanting to help expand the Cole ecosystem! Whether you're fixing a bug in the Nvim highlights or porting the theme to a new platform, your help is appreciated.

### Porting Guidelines

When porting Cole, please refer to `./palette/cole.yml` so the colors are consistent everywhere. `cole.yml` in this repo is the one source of truth, and all ports have to follow the same hex codes.

Follow the directory structure of this repo. If you want to bring Cole to a terminal, make a new folder under `./terminals/` with the name of the terminal in **snake case**. If you want to bring it to a type of tool that doesn't have a folder yet, like an IDE or CAD software, create one in the PR and the name can be finalized in the review. Additionally, each port should include a brief `README.md` explaining how to install to that specific tool.

Finally, we use [Conventional Commits](https://www.conventionalcommits.org). Use this format for each commit you make as well as titles of pull requests. Pull requests should be suffixed with your GitHub username in parentheses.

Commit message example:

```
fix(alacritty): edit colors to maintain accuracy to cole.yml
```

PR title example:

```
feat(port): add alacritty support
```

### Expansion Roadmap

I want Cole to be available everywhere. If you use a platform that's not already supported (or want to improve an existing implementation), PRs are highly encouraged! Refer to the checklist below or open an issue to discuss a new port.

- [ ] Neovim (Lua): On the [cole.nvim](https://github.com/thekylehuang/cole.nvim) repo, add comprehensive support for color highlighting and LSPs
- [ ] VS Code: Port the colors to JSON and post it on the marketplace
- [ ] JetBrains: Add support for IntelliJ, PyCharm, and WebStorm
- [ ] Alacritty: TOML config
- [ ] Kitty: `.conf` format
- [ ] iTerm2: Pull request to [iTerm2 Color Schemes](https://github.com/mbadolato/iTerm2-Color-Schemes)
- [x] Ghostty: Support in Ghostty's theme format 
- [x] Tmux: On the [cole-tmux](https://github.com/thekylehuang/cole-tmux) repo, add full color support for Cole
- [ ] Zsh: Syntax highlighting for the command line
- [ ] Starship: Cole-themed prompt preset
- [ ] Btop: Custom color file for the system monitor
