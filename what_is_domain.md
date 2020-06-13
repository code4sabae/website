# じぶんだけのドメインで公開しよう

## 独自ドメインとは？

URLの https:// の後に続き、最初の / までの間をドメインといいます。  
github.com は、リポジトリ管理サービス、github.io は、GitHub Pagesとして公開されるサービスなど、世界中、さまざまなドメインがあります。  
このドメインを自分で購入することで、自分だけのドメインを使うことができます。これを独自ドメインと呼びます。  

## 独自ドメインを設定しよう

1. ドメインを用意する（購入したり、既存のドメインのサブドメインなど）
2. [Settings]のGitHub Pagesの Custom domain に、設定したいドメイン名を書き[Save]する
3. 管理するドメインのサービスの設定画面へ行き、下記のようにDNSを設定する （4つのIPアドレスがGitHub Pagesを指しています [詳細](https://help.github.com/ja/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site))
```
A	@	185.199.108.153
A	@	185.199.109.153
A	@	185.199.110.153
A	@	185.199.111.153
```
4. DNSの設定が伝搬し有効になるまで待つ
5. 独自ドメインでアクセスしてみる

## わからないこと？

こちらのIssuesに分からないことをどうぞ！  
https://github.com/code4sabae/website/issues  
