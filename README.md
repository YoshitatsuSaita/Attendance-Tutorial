# 勤怠システムを開発しよう！

これはセレブエンジニアサロンの教材で作られたサンプルアプリケーションです。

## 開発環境

- AWS Cloud9
- Ruby
- Rails
- Git

# サンプルアプリケーション（Docker 版手順）

### 1) dockerコンテナ起動(Rails Server起動)

```bash
$ docker-compose up -d
$ docker attach attendance_app-web-1
```

# gemfile変更後の docker-compose run --rm web bundle install も必要

## 権限がなく実行できないときは　docker compose build

### 9) rails c やrails db コマンド実行時

```bash
$ docker compose run --rm web bin/rails c
$ docker compose run --rm web bin/rails db:(各種コマンド)
```

# docker compose run --rm web bin/ を前に書く
