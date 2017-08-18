# iTerm2 and oh-my-zsh setup
Configuration for iTerm2 and oh-my-zsh

## Steps

### Install iTerm2

Go and [download](https://www.iterm2.com/downloads.html) iTerm2. Double-click for starting the installation.

### Install oh-my-zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### Change the iTerm2 theme

See the [solarized theme instructions](https://github.com/altercation/solarized/tree/master/iterm2-colors-solarized):

> Open iTerm 2, open Preferences, click on the "Profiles" icon in the preferences toolbar, then select the "colors" tab. Click on the "load presets" and select "import...". Select the Solarized Light or Dark theme file.

### Download oh-my-zsh theme

Clone the [agnoster](https://github.com/agnoster/agnoster-zsh-theme) into the oh-my-zsh theme folder:

```bash
git clone https://github.com/agnoster/agnoster-zsh-theme.git ~/.oh-my-zsh/custom/themes/agnoster
```
Then, activate the theme by editing the `ZSH_THEME` env var in `~/.zshrc` to have the following content:

```bash
ZSH_THEME="agnoster/agnoster"
```

Close iTerm2 and open it again.

### Install font

Suggested font is [SourceCodePro Medium for Powerline](https://github.com/powerline/fonts/blob/master/SourceCodePro/Source%20Code%20Pro%20Medium%20for%20Powerline.otf). Download and activate it.

Open iTerm 2, open Preferences, click on the "Profiles" icon in the preferences toolbar, then select the "test" tab. Click on the "change font" button and select the `SourceCodePro Medium for Powerline` font and change the size to 14px.

### Set default user

To gain a little space in the terminal, you can set the `DEFAULT_USER` in the `~/.zshrc` file to your default user.
