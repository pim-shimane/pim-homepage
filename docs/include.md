# css,jsの編集と読み込み方法

## css
### 編集
`_includes/css/`の中に`.css`ファイルを作成、編集します。
### 読み込み
`_layouts/style.css`に追加します。 
(例)
```
{% include css/bootstrap.min.css %}
```

## js
### 編集
`js/`の中に`.js`ファイルを作成、編集します。
### 読み込み
`_includes/js.html`に追加します。
(例) 
```
<script src="{{ "/js/jquery-1.11.0.js" | prepend: site.baseurl }}"></script>
```
