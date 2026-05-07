# GitKraken-i18n

GitKraken Desktopの非公式日本語化プロジェクトです。  

**動作確認済み:** GitKraken 12.1.1  

> [!NOTE]
> [megos/gitkraken-i18n](https://github.com/megos/gitkraken-i18n) の翻訳は更新が止まっているため、  
> 本プロジェクトで新たに日本語翻訳を構築・メンテナンスしています。  

## 言語の変更方法

> [!WARNING]  
> 自己責任で行ってください。  
> GitKrakenのアップデート時にファイルが上書きされる場合があります。  

以下の説明では、GitKraken のインストールディレクトリを `<GitKraken>` と表記します。  

| OS | `<GitKraken>` のパス |
|---|---|
| Windows | `%LOCALAPPDATA%\gitkraken\app-x.x.x` |
| Mac | `/Applications/GitKraken.app/Contents/Resources` |
| Linux | `/usr/share/gitkraken/resources` |

※Windowsの `x.x.x` はGitKrakenのバージョン番号に置き換えてください。  

### 1. 元の `strings.json` をバックアップする

元のファイルを `en-us` ディレクトリに移動して保管します。  

```bash
mkdir -p <GitKraken>/app.asar.unpacked/src/en-us
mv <GitKraken>/app.asar.unpacked/src/strings.json <GitKraken>/app.asar.unpacked/src/en-us/strings.json
```

### 2. 本プロジェクトの `strings.json` を配置する

本リポジトリの `strings.json` を元のファイルと同じ場所にコピーします。  

```bash
cp strings.json <GitKraken>/app.asar.unpacked/src/strings.json
```

### 3. GitKraken を再起動する

### 4. 言語を選択する

**Preferences** > **UI Customization** を開き、Language のドロップダウンから **Japanese (JP)** を選択してください。  

## 翻訳に貢献する

1. このリポジトリをフォークする  
2. `strings.json` を編集して翻訳を追加・修正する  
3. 上記の手順で動作確認を行う  
4. Pull Requestを作成する  

## License

[MIT](LICENSE)  
