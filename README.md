# :package_description

[![Latest Version on Packagist](https://img.shields.io/packagist/v/:vendor_slug/:package_slug.svg?style=flat-square)](https://packagist.org/packages/:vendor_slug/:package_slug)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/:vendor_slug/:package_slug/run-tests?label=tests)](https://github.com/:vendor_slug/:package_slug/actions?query=workflow%3Arun-tests+branch%3Amain)
[![GitHub Code Style Action Status](https://img.shields.io/github/workflow/status/:vendor_slug/:package_slug/Fix%20PHP%20code%20style%20issues?label=code%20style)](https://github.com/:vendor_slug/:package_slug/actions?query=workflow%3A"Fix+PHP+code+style+issues"+branch%3Amain)
[![Total Downloads](https://img.shields.io/packagist/dt/:vendor_slug/:package_slug.svg?style=flat-square)](https://packagist.org/packages/:vendor_slug/:package_slug)
<!--delete-->
---
これはSpatie製のLaravel用パッケージの雛形生成機能を日本語化したものです。利用するには下記の手順に従いましょう:

1. このリポジトリのトップにある"Use this template"ボタンをクリックして、このスケルトンの中身そのままに新規リポを作成します
2. それを自分の環境に`git clone`コマンドでダウンロードし、その中に移動して"php ./configure.php"を実行します。
3. パッケージ生成用に幾つかの質問が出てくるので回答を入力すると、最後にこのスケルトンのプレースホルダを入力された内容で書き換えてすべてのファイルを準備してくれます
4. 準備ができたのでパッケージの制作を楽しみましょう
---
<!--/delete-->
ここにはパッケージの概要が入ります。1〜2パラグラフ程度の内容に留め、簡単な例を記載しましょう

## Spatieをサポートしてね

Spatieでは多くの労力を注力して[最高レベルのオープンソースパッケージ](https://spatie.be/open-source)を作ってるので、サポートしてくれるなら[有償版の製品を何個か買ってくれると助かります](https://spatie.be/open-source/support-us).

それと、あなたの住んでる地元のポストカード使って、僕らの作ったパッケージの中から、あなたのお気に入りを書いて送ってくれると嬉しいです。住所は[ここに書いてあるよ](https://spatie.be/about-us). We publish all received postcards on [our virtual postcard wall](https://spatie.be/open-source/postcards).

## インストール

composerを使ってインストールしてください:

```bash
composer require :vendor_slug/:package_slug
```

下記のコマンドで必要なマイグレーションファイルの出力とマイグレーションを実行します:

```bash
php artisan vendor:publish --tag=":package_slug-migrations"
php artisan migrate
```

Configファイルは下記のコマンドで出力可能です:

```bash
php artisan vendor:publish --tag=":package_slug-config"
```

出力されたConfigファイルの中身は次のような感じです:

```php
return [
];
```

オプションとして次のコマンドを実行すとでViewファイルも出力可能です:

```bash
php artisan vendor:publish --tag=":package_slug-views"
```

## 使い方

```php
$variable = new VendorName\Skeleton();
echo $variable->echoPhrase('Hello, VendorName!');
```

## テスト方法

```bash
composer test
```

## 変更履歴

最近の変更履歴については[CHANGELOG](CHANGELOG.md)を参照してください

## 貢献について

このパッケージに貢献したい人は[CONTRIBUTING](CONTRIBUTING.md)を参考にしてください

## セキュリティや脆弱性について

[セキュリティポリシー](../../security/policy)を見て、必要な情報を送ってくれると助かります

## 貢献者

- [:author_name](https://github.com/:author_username)
- [All Contributors](../../contributors)

## ライセンス

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
