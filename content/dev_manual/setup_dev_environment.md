---
title: Setup a Loomio development environment
description: A step by step guide for people wanting to install Loomio on their personal computer so they can fix bugs and write features.
weight: 20
---

There are 3 parts to this document: MacOS X system setup, Ubuntu system setup, and Application setup. You'll need to complete one of the system setups, and then the application setup after that.

## MacOS X system setup

First install [homebrew](http://brew.sh)

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

You then need to install __Command Line Tools for XCode__ from https://developer.apple.com/downloads.

With that done, use Homebrew to install Git and PostgreSQL

```
brew install git postgresql pkgconfig
brew install ImageMagick --with-perl
brew services start postgresql
```

And that's it. You can jump to 'Install ruby'

## Ubuntu system setup

```
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib build-essential \
                     libssl-dev libreadline-dev zlib1g-dev \
                     libpq-dev libffi-dev libmagickwand-dev \
                     imagemagick python
```

## Install ruby

I recommend that you install ruby via rbenv, this gives you the flexiblity required to install and switch between various versions of ruby.

Follow the installation steps for rbenv from  [https://github.com/sstephenson/rbenv#installation](https://github.com/sstephenson/rbenv#installation).

Then install [ruby-build](https://github.com/sstephenson/ruby-build#readme) like so:

```
mkdir -p "$(rbenv root)"/plugins
git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build
```

When a new version of ruby is released, you can update ruby-build with
```
cd "$(rbenv root)"/plugins/ruby-build && git pull
```

At the time of writing 2.5.1 is the version of ruby that Loomio uses. To check what the current version required is, see [.ruby-version](https://github.com/loomio/loomio/blob/master/.ruby-version)

```
rbenv install 2.5.1
rbenv global 2.5.1
gem install bundler
```

## Install node

You'll need Node.js and I recommend you use [nvm](https://github.com/creationix/nvm) to install it. Just run:

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```

You'll need to restart your terminal, then run:

```
nvm install 8.12.0
nvm alias default 8.12.0
```

## Install two packages required for this project

```
npm install -g gulp
```

## Fork and clone the Loomio git repo

I recommend you visit https://github.com/loomio/loomio then click "Fork" to create your own loomio repository to work from.

In my case my forked repo is available at https://github.com/robguthrie/loomio and I use the SSH based url to clone the repo to my computer:

```
cd ~/projects # or wherever you like to keep your code
git clone git@github.com:robguthrie/loomio.git && cd loomio
```

## Install ruby and node dependencies

From you freshly checked out Loomio repo:

```
bundle install
cd client; npm install && cd ..
```

## Create database.yml

```
cp config/database.example.yml config/database.yml
```

On Linux you'll need to create a postgres user with the same name as your Linux user account. This is not required on MacOS as it's automatic.

```
sudo postgres -c 'createuser -P --superuser <username>'
```

## Setup the Loomio database and schema

```
rake db:setup
```

## Launch rails and gulp
Rails run the Loomio server, gulp builds the javascript client, and automatically rebuilds it when you make changes

```
rails s
```

And in a new terminal instance
```
cd client; gulp dev
```

You can view Loomio in your browser by visiting http://localhost:3000, however, you will not be able to move past the initial authentication without navigating through the /dev/ route. To view Loomio's features and changes to your source code, visit any of the dev routes listed at http://localhost:3000/dev/ (be sure to include the trailing slash).  A good place to start might be http://localhost:3000/dev/setup_group.  


## Other things to know
Rails stuff

- sometimes `rails s` and similar commands will fail. Try with `bundle exec rails s` and that can help.
- `rails c` will bring up a rails console
- 'rspec' will run the rails tests

Gulp stuff (run from the client folder)

- `gulp nightwatch`: Run the automated frontend tests
- `npm rebuild node-sass` has been known to be very useful
- if you ever get into problems with node libraries: `rm -rf node_modules && npm install`

### Having trouble?
Let us know in the [product development](https://www.loomio.org/g/GN7EFQTK/loomio-community-product-development) group on Loomio.
