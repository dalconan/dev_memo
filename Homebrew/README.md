# Homebrew


Mac套件軟體管理用

Homebrew安裝方式

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
安裝caskroom（安裝GUI程式用）
```
brew install caskroom/cask/brew-cask
brew tap caskroom/cask
```

將cask安裝目錄從個人目錄的Application目錄改成「應用程式」目錄，
在 .bash_profile裡面加上。

 [官網說明](https://github.com/caskroom/homebrew-cask/blob/master/USAGE.md)

```
export HOMEBREW_CASK_OPTS="--appdir=/Applications"     
```
