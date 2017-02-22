# ruby-rails-sample

This is a simple Ruby app using the [Rails](http://rubyonrails.org) framework.

## Versions

- [Admin version](https://github.com/kefiriaus/ruby-rails-sample/tree/master)
- [Landing page with external auth API](https://github.com/kefiriaus/ruby-rails-sample/tree/external-api-auth)

## Admin version

Added gems:
```ruby
# Add compatibility with jquery
gem 'jquery-turbolinks', '~> 2.1'

# ActiveAdmin
gem 'activeadmin', git: 'https://github.com/activeadmin/activeadmin'
gem 'inherited_resources', git: 'https://github.com/activeadmin/inherited_resources'
gem 'devise'
gem 'devise-i18n'
gem "active_material", github: "vigetlabs/active_material" # , branch: 'nh-responsive-redesign'

# WYSIWYG for activeadmin
gem 'ckeditor'

gem 'carrierwave', '>= 1.0.0.rc', '< 2.0'
gem "mini_magick"

# Menu DSL
gem "navigator"

# Email validator
gem 'validates_email_format_of'

# Meta tags
gem 'meta-tags'

# Error pages
gem 'gaffe'
````

Added gems for development:
```ruby
gem "better_errors"
gem "binding_of_caller"

gem 'rubocop' # to check Ruby code
gem 'scss-lint' # to check SCSS code

gem 'phare' # check for coding style errors
```

## Running Locally

Make sure you have [Ruby](https://www.ruby-lang.org) and [Bundler](http://bundler.io) installed.

```sh
git clone git@github.com:kefiriaus/ruby-rails-sample.git
cd ruby-rails-sample
bundle install
rails db:migrate && rails db:seed
rails s
```

Your app should now be running on [localhost:3000](http://localhost:3000/).

