# Shell Customizations

## Setup oh-my-zsh

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Install the Powerlevel10k theme

```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

Edit the `.zshrc` in your home directory and change the theme as follows:

```
ZSH_THEME="powerlevel10k/powerlevel10k"
```

Restart your terminal or type the following to configure the powerlevel10k theme:

```
source ~/.zshrc
```

Follow the prompts to setup the theme.

If you don't see the configuration process, or would like to re-run the configuration, use the following command:

```
p10k configure
```

## Install zsh plugins

### Install zsh-autosuggestions:

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

### Install zsh-syntax-highlighting:

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

Edit `.zshrc` and add the plugins:

```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting web-search)
```

## Install Useful Shell Utilities

### Exa, a modern replacement for ls

See https://github.com/ogham/exa for details.

Installation on MacOS:

```
brew install exa
```

Installation on Arch Linux:

```
pacman -S exa
```

### Bat, a replacement for the cat command

See https://github.com/sharkdp/bat for details.

Installation on MacOS:

```
brew install bat
```

Installation on Arch Linux:

```
pacman -S bat
```

### Command-line Fuzzy Finder (fzf)

See https://github.com/junegunn/fzf for details.

Installation on MacOS:

```
brew install fzf
```

Installation on Arch Linux:

```
pacman -S fzf
```
