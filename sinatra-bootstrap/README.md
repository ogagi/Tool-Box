# sinatra-bootstrap

Generate a simple [sinatra][1] application with some template files.

* `app.rb` 
* `config.ru`
* `Gemfile`
* `views` folder with an `index.haml`
* `public` folder with an `application.css` file

Run `script/bootstrap` set the _PATH_ for the app and the _NAME_. It will generate the following structure:

```
APP_NAME/
  public/
    public/css
	  public/css/application.css
    public/images
    public/javascript
  views/
    views/index.haml
  app.rb
  models.rb
  Gemfile
  config.ru
```

After this run `bundle install` to install the required gems and run `rackup`.
Something like this should appear:

```
[2013-08-28 17:12:01] INFO  WEBrick 1.3.1
[2013-08-28 17:12:01] INFO  ruby 1.9.3 (2012-11-10) [x86_64-darwin12.4.0]
[2013-08-28 17:12:01] INFO  WEBrick::HTTPServer#start: pid=56062 port=9292
```

And start doing things with sinatra!

[1]: http://sinatrarb.com/intro.html
