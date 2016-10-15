README [![Build Status](https://travis-ci.org/simplonco/rails-scraping-mechanize.svg?branch=master)](https://travis-ci.org/simplonco/rails-scraping-mechanize)
======

## [Ruby on Rails App with Mechanize](https://rubygems.org/gems/mechanize)

### Steps to get the application up and running:
* Create an app for webscraping
```
rails new scraper
cd scraper
```
* Generate a controller
```
rails generate controller welcome_index
```
* Edit your index in `app/views/welcome/index.html.erb`
* Edit `config/routes.rb`: 
```
root 'welcome#index'
```
* Launch the app
```
rails server
```

## Setup your app for webscraping

### Web Scraping - What is it?

an application that processes the HTML of a Web page to extract data for manipulation such as converting the Web page to another format (i.e. HTML to WML). Web Scraping scripts and applications will simulate a person viewing a Web site with a browser. With these scripts you can connect to a Web page and request a page, exactly as a browser would do. The Web server will send back the page which you can then manipulate or extract specific information from.

### [Web-scraping technologies](https://en.wikipedia.org/wiki/Web_scraping)

Sometimes you might need to create an account and login to access the information you need. If you have a good HTTP library that handles logins and automatically sending session cookies (did I mention how awesome Requests is?), then you just need your scraper login before it gets to work.
