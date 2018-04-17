# Emojis: Configuring a more fun development environment in the Terminal
![Expected result](/expected-result.png)
## 1. Install oh-my-zsh
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## 2. Install Bullet Train
(https://github.com/caiogondim/bullet-train.zsh#for-oh-my-zsh-users)

1. Download the theme [here](http://raw.github.com/caiogondim/bullet-train-oh-my-zsh-theme/master/bullet-train.zsh-theme)

2. Put the file **bullet-train.zsh-theme** in **$ZSH_CUSTOM/themes/**

  Usuallly the themes folder is under this directory:

  /Users/{CURRENT_USER}/.oh-my-zsh/themes

3. Configure the theme, colors and emojis in your **~/.zshrc** :
```bash
# PERSONAL CUSTOM
ZSH_THEME="bullet-train"
export TERM="xterm-256color"
BULLETTRAIN_PROMPT_ORDER=(
  nvm
  git
  dir
)
BULLETTRAIN_NVM_BG="030"
BULLETTRAIN_NVM_PREFIX="🤖  "
BULLETTRAIN_DIR_BG="031"
BULLETTRAIN_DIR_FG="255"
BULLETTRAIN_DIR_EXTENDED="0"
BULLETTRAIN_GIT_DIRTY="🤔 - "
BULLETTRAIN_GIT_UNTRACKED="🥑"
BULLETTRAIN_GIT_DELETED="🔥"
BULLETTRAIN_GIT_MODIFIED="🍺"
BULLETTRAIN_GIT_CLEAN=" 😎"
BULLETTRAIN_GIT_ADDED="🚜"
```

## 3. Install Powerline Fonts
(https://github.com/powerline/fonts#quick-installation)
```
# clone
git clone https://github.com/powerline/fonts.git --depth=1
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts
```

## 4. Create a new Profile in the Terminal (oh-my-zsh) and set the colors as follow:
![Expected result](/profile2.png)

## 5. Select the new Profile created in the General tab
## 6. Restart the Terminal
## 7. Result
![Result](/result2.png)
