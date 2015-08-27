# Rails setup on OSX

An excellent reference an be found here: http://railsapps.github.io/installrubyonrails-mac.html

## Global settings

Do not install gem documentation
`$ echo "gem: --no-document" >> ~/.gemrc`

## Starting a new Rails app

Create a folder for the app
`
$ mkdir newapp
$ cd newapp
`

Assuming RVM is used for ruby and gem version management
`
$ rvm use ruby-2.2.2@newapp --ruby-version --create
`

The `--ruby-version` option creates .ruby-version and .ruby-gemset so RVM loads correct version of rails and gemset.

Install latest version of Rails
`
$ gem install rails
`

Create the new rails app in the directory we're currently in
`$ rails new .`