# snakehack-ruby

A simple SnakeHack AI written in Ruby with [Sinatra](http://www.sinatrarb.com/).

This is loosely based on Heroku's official [Getting Started with Ruby App](https://github.com/heroku/ruby-getting-started).

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

### App Overview

- `web.rb` is where the three actions must be implemented: `start`, `move`, `end`

- Each handler is already set up to parse and render JSON.

### Running the AI locally

Fork and clone this repo:

```
git clone git@github.com:stair-ch/snakehack-ruby.git
cd snakehack-ruby
```

Install dependencies:

```
bundle install
```

Run the server:

```
foreman start web
```

Test the client in your browser: [http://localhost:5000](http://localhost:5000)


### Deploying to Heroku

Click the Deploy to Heroku button at the top or use the command line commands below.

Create a new Heroku app:

```
heroku create [APP_NAME] --region eu
```

Push code to Heroku servers:

```
git push heroku master
```

Open Heroku app in browser:

```
heroku open
```

Or go directly via http://APP_NAME.herokuapp.com

View/stream server logs:

```
heroku logs --tail
```
