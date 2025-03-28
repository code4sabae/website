# GitHub Pages で、じぶんのウェブサイトをつくろう！

## ひとまず作ってみよう！

1. 確認できるメールアドレスを用意して、GitHubアカウントを作る [Sign up for GitHub](https://github.com/)
<img width="582" alt="image" src="https://user-images.githubusercontent.com/1715217/226754875-7f52824c-5452-4858-8eac-794dbae6768c.png">

2. [このリポジトリ](https://github.com/code4sabae/website/)を右上にあるForkを押して自分のリポジトリとしてコピーする （リポジトリ＝貯蔵庫、Git上で扱う1つのプロジェクトのファイル一式を指す）
<img width="440" alt="image" src="https://user-images.githubusercontent.com/1715217/226750933-5a111401-eccc-4e70-b02b-ee4011b6de9b.png">

3. 自分のリポジトリの設定 Settings を開く (ブラウザ幅が短いと「...」で隠れている)
<img width="286" alt="image" src="https://user-images.githubusercontent.com/1715217/226753559-2a412a27-cb94-45de-8b1f-96928c860184.png">

4. 左のメニューから「Pages」をクリック、Brunchを[master brunch]に変更して、Saveを押す
<img width="667" alt="image" src="https://user-images.githubusercontent.com/1715217/226753697-51318b6e-b338-4f4e-aa0b-329d5194af4e.png">

5. 1分くらい待つ
6. そのページをリロードすると、新たに表示される https://...github.io/website/ というリンクを新しいウィンドウで開く　（自分のサイトで動いた！）

7. 自分のリポジトリ、メニューの Code を押し index.html を開く
8. 右上の鉛筆マークで編集モードにする （ブラウザの翻訳機能はOFFにしておきましょう）
9. &lt;h1&gt;たいとる&lt;/h1&gt;と書いてあるところを好きなタイトルに変える
10. 画面下の緑色のボタン「commit changes」を押す
11. 1分くらいまって、さっき開いたウィンドウ　https://...github.io/website/　をリロードすると、編集したタイトルに変わる！ （自分のサイトできた！）
12. 以降、編集、コミット、ちょっと待って反映、この繰り返しでウェブサイトづくりができる

## リンクしよう

1. HTMLの本文のどこかに &lt;a herf="http://github.com/" &gt; GitHub &lt; /a &gt; と書いて「commit changes」
2. GitHubへのリンクができる！

## 複数ページを作って、リンクしよう

1. Code を押して、index.html を開く
2. HTMLの本文のどこかに &lt;a herf="test.html"&gt;GitHub&lt;/a&gt; と書いて「commit changes」
3. Code を押して、Add file、Create new file をクリックする
<img width="279" alt="image" src="https://user-images.githubusercontent.com/1715217/226752316-a49daeac-ee2d-4bb1-8891-efb042559213.png">

3. ファイル名でとりあえず test.html とつける （HTMLは .html で終わる英数字でファイル名を付ける）
<img width="375" alt="image" src="https://user-images.githubusercontent.com/1715217/226752535-8419ec4e-6e03-44a1-832b-20647c823db0.png">

4. 本文にテストと書いて「commite changes」、1分くらい待つと反映
5. いくらでもページを増やせる！

## 画像をつけよう

1. pngかjpg画像を準備する
2. 半角英数字を使った空白を含まないファイル名に変更する （日本語名やトラブルの元になる）
3. [Upload files]を押す
4. 画像ファイルをドロップして、コミットする
5. index.html を編集する
6. &lt;img src="imgfile.jpg"&gt; と、&lt;h1&gt;タイトル&lt;/h1&gt; の前の行に書く (imgfile.jpg はアップロードしたファイル名に）
7. コミットし、しばらく待って、リロードすると表示される！

## プログラムを加えよう

1. ページを開いた時、計算結果がダイアログで出るようにするHTMLを加える
```js
<script type="module">
alert(1 + 1);
</script>
```
2. scriptタグの中身はJavaScriptというプログラミング言語、いろいろ計算してくれます！

## サイトを育てましょう！

- [HTMLはじめのいっぽ](https://github.com/code4sabae/website/blob/master/what_is_html.md)
- [CSSはじめのいっぽ](https://github.com/code4sabae/website/blob/master/what_is_css.md)
- [JSはじめのいっぽ](https://github.com/code4sabae/website/blob/master/what_is_js.md)

## わからないこと？

こちらのIssuesに分からないことをどうぞ！  
https://github.com/code4sabae/website/issues  

→ スマホでもいい感じにみえるようにしたい
先頭に下記を記述するといい感じになります
```html
<meta name="viewport" content="width=device-width"><meta name="viewport" content="width=device-width">
```

## GitHub Desktop を使って効率アップ!

1. [GitHub Desktop](https://desktop.github.com/)をダウンロードする
2. 自分のリポジトリの右側[clone or download]を押し、[Open in Desktop]を押す
3. ダウンロードするフォルダをローカルパスとして指定し[Clone]する
4. ダウンロードしたフォルダの中の index.html をブラウザで開くと表示される
5. [VSCode](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)などのエディタを使って、index.html や index.css を編集し、サイトをつくる
6. GitHub Desktop で、コミットする（更新用のメモは必須、”更新”など、一言でもOK！）
7. [Fetch origin] を押し、サーバーにプッシュする
8. しばらく待つと、反映される

## ドメイン名だけでアクセスできるようにしよう

[Settings]で、リポジトリ名を (自分のGitHubアカウント名).github.io に変更すると、そのアドレスでアクセスできます！短くてかっこいいですね！  

github.io じゃなく、じぶんだけのドメイン（独自ドメイン）を設定したい方はこちら  
https://github.com/code4sabae/website/blob/master/what_is_domain.md  
