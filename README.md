# P4D

P4D デザイナー向けプログラム部 の meetup 用 Web アプリケーションになる予定です。

実際に meetup のときにデザイナ / エンジニアで協力しながら作り上げていきましょう！


## 開発に必要なもの

- Ruby 2.0.0-p0
- Rails 4.0.0.beta1


## 動かし方

```
$ git clone git@github.com:prog4designer/p4d.git
$ cd p4d
$ bundle install --path vendor/bundle
$ rake db:migrate
$ rails s
```

* GitHubキー設定

https://github.com/settings/applications

```
Name : [ Local Development ](※何でもよい)

URL : [ http://0.0.0.0:3000/ ](※自分のローカル環境用URL)

Callback URL : [ http://0.0.0.0:3000/ ](※自分のローカル環境用URL)
```

config/settings.local.yml (settings.local.yml.sample をコピーして使ってください)

```yaml
# GitHub OAuth Setting
github_client_id: "Client ID"
github_secret:    "Client Secret"
```

```
rails s
```

http://0.0.0.0:3000/
