# Introduction
This is a simple dotfile collection to config development environment for macs using:

1. Colorls file system forterminal
2. zshell with powerline9k
3. iTerm2
4. Neovim

# Installation

The Powerline9k and the iTerm2 is installed following [this blog post](https://towardsdatascience.com/the-ultimate-guide-to-your-terminal-makeover-e11f9b87ac99)

## Colorls

1. Install and update the ruby version to >= 2.6 (initially used the 3.1.2p20)
2. Install Nerd Font
3. Run the `gem install colorls` command
4. Enable tab completion for flags by entering the configuration file to ~/.zshrc: 
```
source $(dirname $(gem which colorls))/tab_complete.sh
```
5. All the aliases are already on the .zshrc

## nvim 
With all the configurations bellow done, run `:PlugInstall` to install all the dependencies

### DEFX

Install `python >= 3.6.1` and `neovim >= 0.4.0` 
Run the `:echo has('python3')` and, if it returns 1, it's already enabled. If not, run `pip3 install --user pynvim`
If DEFX was installed pripr to Python support being added to Neovim, run `:UpdateRemotePlugins`.

### Telescope && FZF
This telescope configuration uses fzf for better search performance

### Language Servers
This are the lists of language servers used, you can install then by folowing each on [this github post](https://github.com/neovim/nvim-lspconfig/blob/master/doc/configs.md)

1. vuels
2. flow
3. tsserver
4. cssmodules_ls
5. diagnosticls
