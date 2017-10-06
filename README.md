# Simple_Line_Bot

This is easy way to implement your first line bot in ruby use `line-bot-sdk-ruby` gem.

# Usage


### 1. Apply Messaging API
[LINE Business Center](https://business.line.me/zh-hant/services/bot)

### 2. Get SECRET & TOKEN
[line developers](https://developers.line.me/ba)

### 3. Install

```ruby
git clone git@github.com:mgleon08/simple_line_bot.git
```

### 4. Deploy

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com)

```ruby
# create new heroku project
heroku create

# push heroku
git push heroku master

# env config setting
heroku config:add LINE_CHANNEL_SECRET=[YOUR_Channel_Secret]
heroku config:add LINE_CHANNEL_TOKEN=[YOUR_Channel_Access_Token]

# env config remove
heroku config:remove LINE_CHANNEL_SECRET
heroku config:remove LINE_CHANNEL_TOKEN

# log
heroku logs --tail

# scale
heroku ps:scale web=2
```

[uptimerobot](http://uptimerobot.com/) To prevent dormancy

### 5. VERIFY Webhook URL

Go [line developers](https://developers.line.me/ba) to edit Webhook URL and verify

```ruby
Webhook URL: https://{YOUR_HEROKU_SERVER_ID}.herokuapp.com/callback
```

# Reference

* [Messaging API](https://devdocs.line.me/en/)
* [line-bot-sdk-ruby](https://github.com/line/line-bot-sdk-ruby)
* [LineBot - Sinatra blog](http://jiunjiun.logdown.com/posts/2016/10/06/linebot-with-sinatra/#disqus_thread)
