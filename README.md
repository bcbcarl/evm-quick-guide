# evm - Emacs Version Manager

https://github.com/rejeep/evm

## 目標對象

* 需要安裝 Emacs
    * 提供另一種安裝 Emacs 的方式。
* 需要多個版本的 Emacs
    * evm 允許 Emacs 23.4 和 Emacs 24.5 共存。
    * 透過快速切換版本，驗證設定檔是否相容。
    * 套件開發者和維護者可以從中受益。
* 需要執行自動化測試
    * evm 提供編譯好的 Emacs，環境搭建更容易。
    * 跟 Travis-CI 很容易做整合。

## 平台支援

* Travis-CI
* Mac OS X
* Linux

## 使用方式

* `evm`
    * `list` - 列出可用和已安裝的版本
    * `install` - 安裝選定的版本
    * `use` - 使用選定的版本
    * `uninstall` - 解除安裝選定的版本
    * `bin` - evm Emacs 執行檔完整路徑
* `evm-emacs` - 執行 evm 選到的 Emacs 版本

## 安裝方式

### Travis-CI

可參考 [.travis.yml](https://github.com/bcbcarl/emacs-wttrin/blob/master/.travis.yml)。

### 本地安裝

1. 以 Debian/Ubuntu 為例，先安裝下列套件:

    * build-essential
    * libncurses-dev
    * autoconf
    * automake
    * autogen
    * git
    * texinfo
    * libtool

2. 安裝 Ruby。

3. 若要必要，更新 `.ruby-version` 版本號。

4. 參照最新文件[手動安裝](https://github.com/rejeep/evm#manual)。

5. `evm install <version>`

6. `evm use <version>`

7. `evm list`

8. `emacs --version`

## 延伸閱讀

* [Emacs Lisp Unit Testing](https://www.emacswiki.org/emacs/UnitTesting)
