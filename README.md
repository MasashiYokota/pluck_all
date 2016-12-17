[![Gem Version](https://badge.fury.io/rb/pluck_all.svg)](http://badge.fury.io/rb/pluck_all)
[![Build Status](https://travis-ci.org/khiav223577/pluck_all.svg?branch=master)](https://travis-ci.org/khiav223577/pluck_all)

# PluckAll

Plucking Multiple Columns in Rails 3. Also support in Rails 4, and Rails 5

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'pluck_all'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install pluck_all

## Usage

```rb
User.where(:id => [1,2]).pluck_all(:id, :account)
# => [{"id"=>1, "account"=>"account1"}, {"id"=>2, "account"=>"account2"}] 
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake test` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/khiav223577/pluck_all. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

