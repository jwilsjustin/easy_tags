[![Maintainability](https://api.codeclimate.com/v1/badges/5c35fe854f8cbd3f1209/maintainability)](https://codeclimate.com/github/iiwo/easy_tags/maintainability)
[![Build Status](https://travis-ci.org/iiwo/easy_tags.svg?branch=master)](https://travis-ci.org/iiwo/easy_tags)

# EasyTags

Easy tagging for Rails

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'easy_tags'
```

And then execute:

    $ bundle


## Usage

generate migration with:
```
rails g easy_tags:migration
```

in your model add:

```
include EasyTags::Taggable
easy_tags_on :highlights, :birds
easy_tags_on :bees
```

## Testing
```
bundle exec appraisal install
bundle exec appraisal spec
```

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/easy_tags. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
