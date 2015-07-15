# FluentLoggerSinatra

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'fluent-logger-sinatra'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install fluent-logger-sinatra

## Usage

Initalize an instance of the logger
The first argument is the tag prefix, the second argument is an option tag suffix, the third is the host IP, and the fourth is the port number

```ruby
logger = FluentLoggerSinatra::Logger.new('myapp', 'delayed_job', '127.0.0.1', 24224)
logger.info("Delayed Job running on port ###")
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake rspec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/sliuu/fluent-logger-sinatra. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
