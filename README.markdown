# Foundation Icons for Rails

An easy way to use [ZURB's](http://zurb.com) fantastic [Foundation Icons](http://www.zurb.com/playground/foundation-icons) set in a Rails 3 application.

## Installation

1\. Add this line to your application's Gemfile:

```ruby
gem 'foundation-icons-rails'
```

2\. Add this line to your stylesheet

```css
*= require foundation-icons
```

3\. (Optional) Add something like this to your routes.rb file

```ruby
mount Foundation::Icons::Rails::Engine => '/fi'
```


And then, as with most gems, execute:

    $ bundle

Or install it yourself as:

    $ gem install foundation-icons-rails
    


## Usage

### Icons
To use an icon, simply create a some HTML element with some special CSS classes

```html
    <span class="glyph general">l</span>
```
and you'll see something like this ![Globe](https://github.com/TrueNorth/foundation-icons-rails/raw/master/public/img/l.png)

To use the 'enclosed', or 'social' fonts, simply use```<span class="glyph enclosed">l</span>``` or ```<span class="glyph socia">l</span>```, respectively.

Obviously, you need to know exactly which icon corresponds with each letter in the three fonts (general, enclosed, social), so you may be interested in folowing the optional step 3 above, and make use of the handy....

### Directory
If you've followed the optional step 3 above, you can go to the page

    http://localhost:3000/fi/directory

To see a nice list of which icon corresponds to various letters, for each of the three foundation icons fonts (general, enclosed, social)
![Directory](https://github.com/TrueNorth/foundation-icons-rails/raw/master/public/img/directory.png)
In some situations, this may be better than looking at a reference on some other website, because it shows you how the icons will look with all of the other CSS in your web application. The directory will be rendered using your default layout (usually ```application.html.erb``` or ```application.html.haml``` or something).

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
