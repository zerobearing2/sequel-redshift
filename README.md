# Sequel::Redshift

Amazon Redshift adapter for sequel.

## Installation

Add this line to your application's Gemfile:

    gem 'sequel-redshift'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install sequel-redshift

## Usage

connecting to the database

    DB = Sequel.connect('redshift://#{database-url}', options = {})

querying records

    DB[:table].where('created_at > ?', Time.now - 3600)

inserting records

    DB[:table].insert(key: value)

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
