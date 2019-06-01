# Homebrew

## Mac套件軟體管理用，可以使用指令安裝套件或是GUI程式

Homebrew安裝方式

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

新版homebrew會自動裝上cask，所以不需要特別執行下列指令了

~~安裝caskroom（安裝GUI程式用~~
```
brew install caskroom/cask/brew-cask
brew tap caskroom/cask
```

~~將cask安裝目錄從個人目錄的Application目錄改成「應用程式」目錄，
在 .(bash_profile裡面加上。
 [官網說明](https://github.com/caskroom/homebrew-cask/blob/master/USAGE.md)
~~
```
export HOMEBREW_CASK_OPTS="--appdir=/Applications"     
```
~~這樣安裝的程式就會出現在「應用程式」這個目錄~~