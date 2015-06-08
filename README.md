# Lightbox for Bootstrap 3

This gem was built for the use of 'Lightbox for Bootstrap 3' as Rails assets pipeline and you can look for the detailed documents at http://ashleydw.github.io/lightbox/

[![Gem Version](https://badge.fury.io/rb/lightbox-bootstrap-rails.svg)](http://badge.fury.io/rb/lightbox-bootstrap-rails)

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'lightbox-bootstrap-rails'
```

And then execute:

```bash
$ bundle
```

Or install it yourself as:

```bash
$ gem install lightbox-bootstrap-rails
```

## Usage

in assets/javascripts/application.js

``` javascript
//= ...
//= require lightbox-bootstrap
//= ...
```

in assets/stylesheets/application.scss

``` css
...
@import "bootstrap-sprockets";
@import "bootstrap";
@import "lightbox-bootstrap/rails"
...
```

Finally, you should add `assets/stylesheets/lightbox_bootstraped.coffee` as follows:

``` coffee
$(document).delegate '*[data-toggle="lightbox"]', 'click', (event) ->
  event.preventDefault()
  $(this).ekkoLightbox()
  return
```

## Test Application

Among the gem sources, a test application is provided and there you can find how to code in the wild.

# Changelog

  - v 3.3.0.0 : initially created.
  - v 3.3.0.1 : deployed to Rubygems.org


## Contributing

1. Fork it ( https://github.com/[my-github-username]/lightbox-bootstrap-rails/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
