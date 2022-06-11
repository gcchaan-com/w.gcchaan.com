---
title: "Mac"
linkTitle: "Mac"
weight: 1
description: >
  Mac の設定と便利ツール

---

# macセットアップ備忘録

### Launchpad

- 既存アプリケーションをグループに押し込める


### Dock & Menu Bar

システム設定(Dock & Menu Bar)
- バッテリーの割合を表示
- 日付表示
- アイコンドックの整理・右側に変更


### Trackpad

システム設定(Trackpad)
- トラックパッドのジェスチャを設定


### Keyboard

システム設定(Keyboard)
- リピート最速・ディレイ最短設定
- 連続入力の有効化
    - `defaults write -g ApplePressAndHoldEnabled -bool TRUE`
    - ログアウトか再起動が必要
- FnキーでのF1〜F12入力の標準設定
- 自動キャピタライズ無効化
- ダブルスペースでのピリオド挿入無効化
- スマートクオート無効化
- 入力ソース追加
    - `google-japanese-ime` をインストールしておく

Karabinar 設定


### Finder

設定
  - サイドバー項目の表示非表示設定
  - 拡張子表示
  - 隠しファイル表示
    1. `defaults write com.apple.finder AppleShowAllFiles TRUE`
    1. `killall Finder`


### ターミナル・シェル設定

- iTerm2インストール
- Homebrewインストール


### その他

- NightShift常時稼働設定
- 英語に変更
- フォームのあるアプリでファンクションキーをタッチバーに表示
- SSH鍵コピー
- 壁紙設定


### Brewfile

```.Brewfile
brew 'coreutils'
brew 'direnv'
brew 'gawk'
brew 'git'
brew 'hr'
brew 'httpie'
brew 'jq'
brew 'jsonpp'
brew 'mysql-client'
brew 'nkf'
brew 'ripgrep'
brew 'tmux'
brew 'tree'
brew 'wget'
brew 'yarn'
brew 'zsh-completions'
cask 'altair-graphql-client'
cask 'amazon-music'
cask 'authy'
cask 'bitwarden'
cask 'discord'
cask 'docker'
cask 'evernote'
cask 'figma'
cask 'firealpaca'
cask 'google-chrome'
cask 'google-japanese-ime'
cask 'hyperswitch'
cask 'imageoptim'
cask 'intellij-idea-ce'
cask 'insomnia'
cask 'iterm2'
cask 'karabiner-elements'
cask 'keycastr'
cask 'kindle'
cask 'kindle-previewer'
cask 'postico'
cask 'screenflow'
cask 'skype'
cask 'slack'
cask 'spotify'
cask 'sourcetree'
cask 'tableplus'
cask 'visual-studio-code'
cask 'zoom'
mas "Gifski", id: 1351639930
mas "LINE", id: 539883307
mas "Xcode", id: 497799835
```


### CLI 設定の備忘録

- aws
  - profile設定
- git
  - `git config --global user.name "USERNAME"`
  - `git config --global user.email "USERNAME@users.noreply.github.com"`


### Go

[https://golang.org/](https://golang.org/)


### Node.js

[fnm](https://github.com/Schniz/fnm)


### Python

```.Brewfile
brew 'pipenv'
brew 'pyenv'
```


### Ruby

```.Brewfile
brew 'ruby-build'
brew 'rbenv'
brew 'ruby'
```


### Java（JVM）

- [sdkman](https://sdkman.io/)
-  `brew install --cask java`


### Scala

先にjavaが必要

```.Brewfile
brew 'sbt'
brew 'scala'
```

/usr/local/etc/sbtopts の `mem` を4096とか


### AWS

SAM
```bash
brew tap aws/tap
brew install aws-sam-cli
```


### Hugo

```.Brewfile
brew hugo
```
