# Tapestry

[TAP](http://testanything.org/) tools and its wrapper testing framework in Ruby.

Tapestry API is inspired by [tape](https://github.com/substack/tape).

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'tapestry'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install tapestry

## Usage

```ruby
require 'tapestry'

# @params [Integer] number of tests.
tapestry = Tapestry::Test.new(1)

expected = 2
actual = 1 + 1
msg = 'test1'
test_num = 1

tapestry.equal(expected, actual, msg, test_num)
```

## API

### tapestry.equal(a, b, msg, num)

Assert that `a == b` with an optional msg and test number.

Aliases: `tapestry.equals()`, `tapestry.is()`, `tapestry.is_equal_to()`, `tapestry.is_equal_in()`

### tapestry.not_equal(a, b, msg, num)

Assert that `a != b` with an optional msg and test number.

Aliases: `tapestry.is_not()`, `tapestry.is_not_equal_to()`, `tapestry.is_not_equal_in()`

### tapestry.description(msg)

Print `msg`.

Aliases: `tapestry.message()`, `tapestry.echo()`
## Contributing

1. Fork it ( https://github.com/[my-github-username]/tapestry/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
