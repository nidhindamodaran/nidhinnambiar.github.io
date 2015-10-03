---
layout: post
---

####1.Initializing heroku application
Change directory into project folder eg.
```bash
cd railsapp
```
Now initialize heroku app

```bash
heroku create
```

This will create a new application in heroku.

####2.Update Gemfile
Next step is updating your gemfile

First replace

```ruby
gem 'sqlite3'
```
with

```ruby
group :development, :test do
  gem 'sqlite3'
end

group :production do
  gem 'pg'
  gem 'rails_12factor'
end
```
Here specifies the gem required for production in heroku, and now apply the changes

```bash
bundle install --without production
```

####3.Commit changes

```bash
git add .
git commit -m "Gemfile changed"
```

####4.Pushing to Heroku
After creating each changes in project you had add  and commit then

```bash
git push heroku master
```
