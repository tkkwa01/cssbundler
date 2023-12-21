# Scaffoldとcssbundling-railsを使った簡単なToDo

## プロジェクトを作成
```bash
rails new myapp --css tailwind
```

## Gemfileに追加
```ruby
gem 'cssbundling-rails'
```

## bundleでインストール
```bash
bundle install
rails css:install:tailwind
```

## scaffoldでCRUDを作成
```bash
rails g scaffold todo name:string limit:date
```

## DBをマイグレート
```bash
rails db:migrate
```

## tailwindをビルド
```bash
rails tailwindcss:build
```