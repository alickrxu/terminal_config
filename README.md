# Setup instructions

## Provided Files
```
.zshrc - Includes env variables, powerlevel10k setup
.vimrc - VIM setup, includes linenumbers and highlighting
Arthur.itermcolors - My preferred iterm2 theme
```

## Install brew on zsh:
	
Add Homebrew to your PATH in `~/.zprofile`:
```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Setup VIM
### Install [Vundle (VIM package handler)](https://github.com/VundleVim/Vundle.vim)
```
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

## Use .vimrc
```
mv .vimrc ~/
```

## Create /backups directory for Vim Swap files
```
mkdir ~/.vim/backups
```
More info [here](https://github.com/neovim/neovim/issues/3498)

## Packages

### thefuck

```brew install thefuck```

### oh-my-zsh 

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Install [powerlevel10k](https://github.com/romkatv/powerlevel10k)

```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
p10k configure
```

Enable battery on command line
```
vi ~/.p10k.zsh
Uncomment battery
```

## Other Software

### [Sublime Text](https://www.sublimetext.com/)

```
Enable subl command:
export PATH="/Applications/Sublime Text.app/Contents/SharedSupport/bin:$PATH"
```
#### Useful Sublime Text Packages
- Package Control
- Vim Mode
- Markdown Preview
- Markdown Formatting
- JSON Formatter
