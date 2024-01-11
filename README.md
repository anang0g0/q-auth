# q-auth
PKPを用いたブラインド電子署名を使って、SSH認証のようにアカウント認証するための方法について。

まずアカウントを作るときにSSH鍵を登録する。

秘密鍵はエラーベクトル。

公開鍵を使って確率的電子署名を作ることができれば一見別のように見えるパスナンバーを使ってすべてのアカウントをにアクセスすることができるというもの。
公開鍵は各ウェブサービス内で管理されるだけでいいのでPKIのような管理システムは必要ない。

ただしPKIなど個人の存在を保証するためにはそのシステムが必要になる。
今までのSNSなどは個人の特定ができる余地を残したものだった。
しかしSSH方式は鍵の真正性のみを保証していればいい。
ユーザーはサービスのアカウント作成時にSSHの公開鍵だけを登録すればいい。
