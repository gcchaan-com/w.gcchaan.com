---
title: "Mac"
linkTitle: "Mac"
weight: 1
description: >
  Mac の設定と便利ツール

---

### macセットアップ備忘録
- バッテリーの割合を表示
- 日付表示
- トラックパッドのジェスチャを設定
- キーボード設定; リピートを早くする
- アイコンドックの整理・左側に変更
- Finderの設定
  - よく使う項目の設定、ユーザーディレクトリ、格納先、iTunesに自動で追加フォルダも追加
  - 隠しファイル表示
    1. `defaults write com.apple.finder AppleShowAllFiles TRUE`
    1. `killall Finder`
- NightShift常時稼働設定
- 背景変更
- 英語に変更
- フォームのあるアプリでファンクションキーをタッチバーに表示
- Xcodeとhomebrew設定
- Karabinar 設定
- zshに変更(oh-my-zshインストールで可能)
  - /usr/sbin にパスを通す
- SSH鍵コピー
- 壁紙設定



### Brewfile

```.Brewfile
tap 'burntsushi/ripgrep', 'https://github.com/BurntSushi/ripgrep.git'
tap 'caskroom/cask'
tap 'caskroom/versions'
tap 'homebrew/bundle'
tap 'homebrew/core'
tap 'homebrew/science'
tap 'homebrew/versions'
tap 'phinze/cask'
cask 'java'
brew 'bash-completion'
brew 'coreutils'
brew 'curl'
brew 'direnv'
brew 'gawk'
brew 'git'
brew 'python'
brew 'gradle'
brew 'hr'
brew 'httpie'
brew 'jq'
brew 'jsonpp'
brew 'mysql-client'
brew 'nkf'
brew 'node'
brew 'pipenv'
brew 'pyenv'
brew 'ruby-build'
brew 'rbenv'
brew 'ruby'
brew 'sbt'
brew 'scala'
brew 'sl'
brew 'tmux'
brew 'tree'
brew 'vim'
brew 'wget'
brew 'yarn'
brew 'youtube-dl'
brew 'zsh'
brew 'zsh-completions'
brew 'burntsushi/ripgrep/ripgrep-bin'
cask 'dropbox'
cask 'evernote'
cask 'google-chrome'
cask 'google-japanese-ime'
cask 'hyperswitch'
cask 'imageoptim'
cask 'iterm2'
cask 'karabiner'
cask 'kindlegen'
cask 'postico'
cask 'screenflow'
cask 'sequel-pro'
cask 'slack'
cask 'sourcetree'
cask 'visual-studio-code'
cask 'wireshark'
mas "LINE", id: 539883307
mas "Xcode", id: 497799835
```

- sbt -> 先に `brew cask install java` が必要
- rbenv ruby-build -> install 後 `rbenv init`


### CLI 設定の備忘録

- aws
  - profile設定
- git
  - `git config --global user.name "USERNAME"`
  - `git config --global user.email "USERNAME@users.noreply.github.com"`
- sbt
  - /usr/local/etc/sbtopts の `mem` を4096とか
- nvm, pyenv, rbenv
