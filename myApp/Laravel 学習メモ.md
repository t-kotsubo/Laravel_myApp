## Laravel 学習メモ



### Laravel インストール

```
$ composer global require laravel/installer
```

### Laravel バージョン確認

```
$ laravel help --version
```

### Laravel アプリ作成

```
$ laravel new アプリ名
```

### Laravel ディレクトリ構成

![image-20230916154856463](C:\Users\t_kot\AppData\Roaming\Typora\typora-user-images\image-20230916154856463.png)



### コントローラーの作成

```
$ php artisan make:controller コントローラー名(*Controllerという名称が一般的)
```

※コントローラーの作成に成功すると/app/Http/Controllersフォルダ配下に`コントローラー名.php`のファイルが生成される

### ルーティング

ルーティング設定は`/routes/web.php`に定義する

#### ◎getメソッド

```
Route::get(path, action)
path: リクエストパス
action: 実行すべきアクション
```

※引数actionは呼び出すアクションを`コントローラー名@アクション名`で指定する



