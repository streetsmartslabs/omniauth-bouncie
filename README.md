# Omniauth::Bouncie

This is the unofficial OmniAuth strategy for authenticating to Bouncie. Register your app and see official documentation at [https://docs.bouncie.dev](https://docs.bouncie.dev).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'omniauth-bouncie'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install omniauth-bouncie

## Usage

```ruby
use OmniAuth::Builder do
  provider :bouncie,
           ENV['BOUNCIE_CLIENT_ID'],
           ENV['BOUNCIE_CLIENT_SECRET'],
           token_params: {
             redirect_uri: 'http://localhost:3000/auth/bouncie/callback'
           }
end
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/omniauth-bouncie.

## License
Copyright (c) 2020 StreetSmarts Labs, LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
