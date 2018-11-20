## HerokuのSendGrid Addon を使ってメール送信する設定

- [Herokuのドキュメント](https://devcenter.heroku.com/articles/sendgrid)

## Heroku CLIのインストール(For Mac)
- [Herokuのドキュメント](https://devcenter.heroku.com/articles/heroku-cli)
```
brew install heroku/brew/heroku
```

```
heroku create AppName
heroku addons:create sendgrid:starter --app AppName
```
## Heroku GUI上で設定する内容
SendGrid -> Settings -> API Keys
- Creat API Key

- 取得したAPIを設定する
```
heroku config:set SENDGRID_API_KEY=API_KEY --app AppName
```

## PHPのインストール
```
brew install php71
brew install composer
```

- composer.json 作成後
```
ocmposer install
```

## Heroku へのデプロイ
```
git add .
git commit -m 'commit message'
git push heroku master
```
