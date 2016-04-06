# Chargebee Ruby Client Library - API V1

The ruby library for integrating with Chargebee Recurring Billing and Subscription Management solution.

Chargebee now supports two API versions - [V1](https://apidocs.chargebee.com/docs/api/v1) and [V2](https://apidocs.chargebee.com/docs/api). This library is for our <b>older API version V1</b>. The library for V2 can be found in the [master branch](https://github.com/chargebee/chargebee-ruby). 

You'd want to upgrade to V2 to benefit from the new functionality. Click here for the [API V2 Upgradation Guide](https://apidocs.chargebee.com/docs/api/v1#api-v2-upgradation-guide).


## Installation

Install the latest version of the gem with the following command...
	
	$ sudo gem install chargebee -v '~>1'

## Documentation

For API reference see <a href="https://apidocs.chargebee.com/docs/api/v1/?lang=ruby"  target="_blank">here</a>

## Usage

To create a new subscription:
	
	ChargeBee.configure({:api_key => "your_api_key"}, {:site => "your_site"})
	result = ChargeBee::Subscription.create({
		:id => "sub_KyVqDh__dev__NTn4VZZ1", 
		:plan_id => "basic", 
	})
	subscription = result.subscription
	puts "created subscription is #{subscription}"

## License

See the LICENSE file.
