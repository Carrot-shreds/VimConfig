# Personal NeoVim config based on [LazyVim](https://github.com/LazyVim/LazyVim).

# 🛠️ Installation

## Linux/MacOS

- Make a backup of your current Neovim files:

  ```sh
  # required
  mv ~/.config/nvim{,.bak}

  # optional but recommended
  mv ~/.local/share/nvim{,.bak}
  mv ~/.local/state/nvim{,.bak}
  mv ~/.cache/nvim{,.bak}
  ```

- Clone the starter

  ```sh
  git clone https://github.com/Carrot-shreds/VimConfig ~/.config/nvim
  ```
  
- Start Neovim!

  ```sh
  nvim
  ```

## Windows

- Make a backup of your current Neovim files:

  ```powershell
  # required
  Move-Item $env:LOCALAPPDATA\nvim $env:LOCALAPPDATA\nvim.bak

  # optional but recommended
  Move-Item $env:LOCALAPPDATA\nvim-data $env:LOCALAPPDATA\nvim-data.bak
  ```

- Clone the starter

  ```powershell
  git clone https://github.com/Carrot-shreds/VimConfig $env:LOCALAPPDATA\nvim
  ```
  
- Start Neovim!

  ```powershell
  nvim
  ```

  Refer to the comments in the files on how to customize **LazyVim**.

## Try it with Docker

```sh
  docker run -w /root -it --rm alpine:edge sh -uelic '
  apk add git lazygit fzf curl neovim ripgrep alpine-sdk --update
  git clone https://github.com/Carrot-shreds/VimConfig ~/.config/nvim
  cd ~/.config/nvim
  nvim
  '
```
