Tm
================

Ruby on Rails
-------------

This application requires:

- Ruby 2.2.2
- Rails 4.2.5

Learn more about [Installing Rails](http://railsapps.github.io/installing-rails.html) or use [pre-configured Vagrant container](https://github.com/ro31337/just-ror).

Getting Started
---------------

Before you start make sure you did initial project setup:

```bash
$ bundle install
$ rake db:migrate
```

Basic commands are:

Kicks off local development server on port 3000:

```bash
$ rails s
```

Open `http://localhost:3000` in your browser. Please note: if you use vagrant/docker you may need to tell Rails to listen on all ip addresses:

```bash
$ rails s -b 0.0.0.0
```

Run entire tests suite:

```bash
$ rspec
```

or

```bash
$ rspec ./spec/path/to/file.rb
```

to run tests from specified file.

Debugging
---------

[pry](https://github.com/pry/pry) gem, [pry-byebug](https://github.com/deivid-rodriguez/byebug), and [pry-stack_explorer](https://github.com/pry/pry-stack_explorer) are enabled for test and production environment.

Paste `binding.pry` wherever you need a breakpoint. Run app the standard way (`rails s` or `rspec`).

Few commands inside pry (aliases are defined in `.pryrc`):

Command      | Description
-------------|-------------
`exit`       | Exit from pry (go to the next breakpoint)
`show stack` | Shows the stack
`c`          | Continue
`s`          | Step
`n`          | Next

Documentation and Support
-------------------------

Issues
-------------


Contributing
------------

TODO: add ruby lint and code analyzer (rubycop).

Credits
-------

License
-------

(c) 2015-2016 TM team.
