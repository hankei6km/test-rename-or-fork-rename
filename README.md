# test-rename-or-fork-rename
リポジトリ名のリネームとフォークの違いを試す。これはリネームした

https://docs.github.com/ja/free-pro-team@latest/github/administering-a-repository/renaming-a-repository

の手順でリネームした。

> Web トラフィックのリダイレクトに加え、前の場所をターゲットにしたすべての git clone、git fetch、または git push 操作は、引き続き新しい場所に対して行われているように機能します。 ただし、混乱を低減するため、既存のローカルクローンが新しいリポジトリ URL を指すよう更新することを強く推奨します。 これを行うには、コマンドラインで git remote を使用します。

古い名前の URL でアクセスした場合、リダイレクトされることは確認できた(いつまでリダイレクトされる?)

ウェブの clone のアドレスは `git@github.com:hankei6km/test-rename-or-fork-rename-1.git` で変更されている。


ローカルの remote はそのままで push してみる

```
$ git remote -v
origin	git@github.com:hankei6km/test-rename-or-fork-rename.git (fetch)
origin	git@github.com:hankei6km/test-rename-or-fork-rename.git (push)
```

これがプッシュできれば push もリダイレクトされる


