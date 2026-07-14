# Rails Association Task

Active Recordの関連付けを学ぶための課題用Railsアプリケーションです。

## 動作環境

- Ruby 4.0.5
- Ruby on Rails 8.1.3
- PostgreSQL 18.4
- Node.js 24.18.0 LTS (Krypton)

## セットアップ

PostgreSQLを起動した状態で、次のコマンドを実行します。

```sh
bundle install
bundle exec rails db:prepare
```

ローカルのPostgreSQL接続にユーザー名やパスワードが必要な場合は、`DATABASE_URL`を設定してください。

```sh
export DATABASE_URL=postgresql://USER:PASSWORD@localhost/rails_association_task_development
```

## 起動

```sh
bundle exec rails server
```

ブラウザで `http://localhost:3000/exercises/exercise1` を開きます。

## テスト

評価用の`spec`ディレクトリが配置された環境で、次のコマンドを実行します。GitHub Actionsでは評価コードを自動的に取得します。

```sh
RAILS_ENV=test bundle exec rails db:prepare
bundle exec rspec
```

このアプリケーション固有の必須環境変数はありません。本番環境では、`DATABASE_URL`、`SECRET_KEY_BASE`、または既存の`config/database.yml`に対応する`rails_association_task_DATABASE_PASSWORD`を設定してください。
