# Heroku

## 準備

- Heroku Toolbelt
- git

## 認証から

```
> heroku login
> heroku create [hogehoge]
> git init
> heroku git:remote -a [hogehoge]
```

heroku git:remoteで紐付け

```
> git add .
> git commit -m "first commit"
> git push heroku master
```

## DBの使用

menu>data から追加  
menu>data>postgresql-hogehoge>Setttig>DatabaseCredentials View  
でURIを指定することでnode.jpのpgからアクセス可能

### postgreSQL

#### JSON

postgreSQL 9.2からJSONのサポートがされている。2018-05-04時点でv10がdefaultなので使えるはず。



####

##

heroku login: Herokuにログインします。
heroku logout: Herokuをログアウトします。
heroku create: Herokuにappを作成する。
heroku apps: Herokuに上がっているdyno(アプリ)一覧を表示する。
heroku run: Herokuに実行させたいコマンドをrunの後ろに続けて打つ。
heroku config: Herokuの環境変数を確認できる。
heroku open: Herokuにアップしたアプリをブラウザで開いてくれる。
git push heroku master: Herokuにdeployする。
