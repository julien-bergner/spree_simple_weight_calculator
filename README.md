Spree Simple Weight Calculator
==============================

This is a shipping costs calculator for the Ruby on rails e-commerce solution Spree.

It's based on the total weight of the order.
You simply specify a weight/price table in a textarea like this:

```
5:10
10.5:15
100:50.5
```

This means:
- up to 5kg cost is 10$
- up to 10.5kg cost is 15$
- up to 100kg cost is 50.5$
- over 100kg this shipping method doesn't apply

An handling fee may also be added.

Usage
=====

Add to your Gemfile

    # for spree 2.1.0
    gem 'spree_simple_weight_calculator',
      github: 'julien-bergner/spree_simple_weight_calculator',
      branch: '2-1-stable'

    # for spree 2.0.x
    gem 'spree_simple_weight_calculator',
      github: 'freego/spree_simple_weight_calculator',
      branch: '2-0-stable'

    # for spree 1.3.x
    gem 'spree_simple_weight_calculator',
      github: 'freego/spree_simple_weight_calculator',
      branch: '1-3-stable'

Create a shipping method and choose "Simple Weight" as calculator.

Testing
-------

Be sure to bundle your dependencies and then create a dummy test app for the specs to run against.

    $ bundle
    $ bundle exec rake test_app
    $ bundle exec rspec spec

Credits
=======

Inspired by https://github.com/dancinglightning/spree-postal-service .


Copyright (c) 2013 freego http://freegoweb.it - Released under the MIT License
