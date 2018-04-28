# 全域環境設定檔
## git

### ignore(排除檔案設定)

[gitignore_global](gitignore_global)

git ingnore全域檔案，將指定檔案或副檔名排除，可依照需求和常用開發環境將特定檔案加入。

檔案位置

Mac 
```
$HOME/.gitignore_global
```

Windows  
```
C:\Users\[Your_name]\Documents\gitignore_global.txt
```

設定檔

git基本設定檔，路徑或是預設名稱等訊息。

檔案位置

Mac 
```
$HOME/.gitconfig
```

Windows  
```
C:\Users\[Your_name]\.gitconfig
```

## SVN

### ignore(排除檔案設定)

找到設定檔的 [miscellany] 區塊下的 global-ignores ，將要排除的副檔名或檔案加上

EX

```
[miscellany]
global-ignores = *.o *.lo *.la #*# .*.rej *.rej .*~ *~ .#* .DS_Store ._* *.log *.bak node_modules *.idea .project .idea
```

檔案位置


Mac 
```
~/.subversion/config
```

Windows  
```
C:\Users\<username>\AppData\Roaming\Subversion
```

