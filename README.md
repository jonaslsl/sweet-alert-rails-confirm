sweet-alert-rails-confirm
=========================

A Rails confirm replacement with SweetAlert

## Requirements
Rails >= 3.1

## Usage

Add it to your Gemfile:
```ruby
gem 'sweet-alert-confirm', github: 'marcelobarreto/sweet-alert-confirm'

source 'https://rails-assets.org' do
  gem 'rails-assets-sweetalert'
end

```

Add the following to application.js:

```javascript
//= require sweetalert
//= require sweet-alert-confirm
```
Add the following to application.css:

```css
/*
 *= require sweetalert
 */
```

OR

```scss
@import "sweetalert";
```

### Custom options


You can pass options in `data:`
```Ruby
 data: {
  sweet_alert_confirm: 'Are you ready?'
  confirm_button_text: 'Im ready',
  cancel_button_text: 'No way',
  confirm_button_color: '#66CD00',
  sweet_alert_type: 'info',
  text: 'This is a subtitle',
  image_url: '/pic.png'
}
```

![Custom confirm](https://cloud.githubusercontent.com/assets/5833678/4653700/14389916-54b0-11e4-9850-14ee970e9345.png)

Default options that will be used application wide so it is not nessecary to set the option on each link. Put this object inside your app to override default options with `sweetAlertConfirmConfig` object.

```Javascript
var sweetAlertConfirmConfig = {
  title: 'Are you sure?',
  type: 'warning',
  showCancelButton: true,
  confirmButtonColor: '#DD6B55',
  confirmButtonText: 'Ok'
};
```

## Contribute

Fork the repo & pull request you fix/feature

append `RAILS_VERSION=4.1.2` or whichever you target before your `bundle` command ex: `RAILS_VERSION=4.1.2 bundle install`

please add/modify test examples on fix or features
