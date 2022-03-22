# Bulk Discounts 

![languages](https://img.shields.io/github/languages/top/JCNapier/bulk_discounts?color=red)
![rspec](https://img.shields.io/gem/v/rspec?color=blue&label=rspec)
![simplecov](https://img.shields.io/gem/v/simplecov?color=blue&label=simplecov)
[![All Contributors](https://img.shields.io/badge/contributors-1-orange.svg?style=flat)](#contributors-)


## Description 

Bulk Discounts is a solo project that is an extension of the Little Esty Shop group project. Added functionality for merchants to create bulk discounts for their items. A “bulk discount” is a discount based on the quantity of items the customer is buying, for example “20% off orders of 10 or more items”. Little esty shop is a group project that has a total of 8 contributors. Little Esty emulates an online store with different admins, merchants, items, invoices, invoice items, etc. It has full functionailty of a real application(within the scope of the application) using dummy data to populate the website with items, merchants, and invoices. 

## APIs Used 

- [Public Holiday API](https://date.nager.at/api)

## Learning Goals 
- Write migrations to create tables and relationships between tables
- Implement CRUD functionality for a resource using forms (form_tag or form_with), buttons, and links
- Use MVC to organize code effectively, limiting the amount of logic included in views and controllers
- Use built-in ActiveRecord methods to join multiple tables of data, make calculations, and group data based on one or more attributes
- Write model tests that fully cover the data logic of the application
- Write feature tests that fully cover the functionality of the application
- Correctly test and implement the consumption of an API. 
- Incorporate API returned JSON data into functionality of bulk discounts. 
- Successfully implement a facade pattern into the API consumption. 

## Versions
- Ruby 2.7.2
- Rails 5.2.6

## Gems
```ruby 
  #Global Scope Gems 
  gem 'bootstrap'
  gem 'faraday'
  
  #group :development, :test
  gem 'capybara'
  gem 'factory_bot_rails'
  gem 'faker'
  gem 'launchy'
  gem 'pry'
  gem 'orderly'
  gem 'rspec-rails'
  gem 'shoulda-matchers'
  gem 'simplecov'
  
  #group :test 
  gem 'vcr'
  gem 'webmock'
```
- [VCR Docs](https://github.com/vcr/vcr)
- [WebMock Docs](https://github.com/bblimke/webmock)
- [Faraday Docs](https://lostisland.github.io/faraday/)
- [SimpleCov Docs](https://github.com/simplecov-ruby/simplecov)
- [Capybara Docs](https://github.com/teamcapybara/capybara)
- [ShouldMatchers Docs](https://github.com/thoughtbot/shoulda-matchers)
- [Factory Bot Rails Docs](https://github.com/thoughtbot/factory_bot_rails)
- [Faker Docs](https://github.com/faker-ruby/faker)
- [Bootstrap Docs](https://github.com/twbs/bootstrap-rubygem)
- [Orderly Docs](https://github.com/jmondo/orderly)


## Local Setup 

1. Fork & Clone the repo 
```shell
$ git clone git@github.com:JCNapier/bulk_discounts.git
```
2. Navigate to the directory 
```shell 
$ cd bulk_discounts
```
3. Install gem packages:
```shell
$ bundle install
```
4. Update gem packages: 
```shell
$ bundle update
```
5. SRun the migrations: 
```shell
$ rake db:{drop,create,migrate,seed}
```

## Test Suite 

To properly run the test suite you will need to follow these instructions, and run the following commands in terminal: 

1. Once you are in the bulk_discounts directory run the following command in your terminal: ```bundle exec rspec```
2. There 140 tests in total. This command will run the *entire* test suite. All tests should be passing. 
3. You will notice the VCR gem is being used in conjunction with webmock. In the instance there are failing tests, try deleting the fixtures folder located in the path ```spec/fixtures```. 
4. Once you delete the fixtures re-run the *entire* test suite again and *vcr* will automatically create a new fixtures folder and repopulate new vcr cassetes with new test data from the API in use for the test suite to run on. 

## Schema 
![Screen Shot 2022-01-19 at 10 30 59 AM](https://user-images.githubusercontent.com/81737385/150183387-7d9a224b-0193-4bad-af65-28e748789ac5.png)

## Project Contributors

<a href="https://github.com/JCNapier/bulk_discounts/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=JCNapier/bulk_discounts" />
</a>


