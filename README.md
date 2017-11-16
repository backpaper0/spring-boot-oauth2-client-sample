# Spring SecurityのOAuth 2クライアントでログインする

プロバイダはGitHubを使う。

## 準備

### GitHubでOAuth Appを作る

https://github.com/settings/developers を開く。

"Register a new application"をクリック。
（すでに1つ以上OAuth Appがある場合は"New OAuth App"をクリック）

次のように入力。

|項目|値|
|---|---|
|Application name|`helloworld`|
|Homepage URL|`http://localhost:8080`|
|Authorization callback URL|`http://localhost:8080`|

"Register application"をクリック。

### application.propertiesを編集する

生成された"Client ID"と"Client Secret"を`application.properties`に書く。

## 試す

アプリケーションを起動して http://localhost:8080 をブラウザで開く。

