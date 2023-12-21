# Scaffoldとcssbundling-railsを使った簡単なToDo
プログラムを一切書かずに綺麗なアプリが作れる．

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
# スクリーンショット
<img width="1920" alt="スクリーンショット 2023-12-21 19 28 34" src="https://github.com/tkkwa01/cssbundler/assets/130450932/d2b0ef0b-4165-4287-b60a-6207893751b1">
<img width="1920" alt="スクリーンショット 2023-12-21 19 27 06" src="https://github.com/tkkwa01/cssbundler/assets/130450932/111797e3-d18d-498f-86de-bb3a6ddeb85b">
<img width="1920" alt="スクリーンショット 2023-12-21 19 27 20" src="https://github.com/tkkwa01/cssbundler/assets/130450932/43548267-a1c0-486b-a029-2d5b42882d86">
<img width="1920" alt="スクリーンショット 2023-12-21 19 28 56" src="https://github.com/tkkwa01/cssbundler/assets/130450932/31b559b3-1452-47cf-bf3b-4da72ac67724">
