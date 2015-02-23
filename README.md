# Author-Level Metrics

This script generates the following author-level metrics based on ".bib" files:
* h-Index
* Normalized h-Index
* m-Index
* Normalized m-Index
* Average Citation Count
* Normalized Average Citation Count
* Date of Second Publication

## Installation

Before you can run the script, you will need to install some dependencies.

First, make sure you have a Ruby programming environment. Most Unix-based OSes come with a pre-installed version of Ruby, but I highly recommend a dedicated Ruby version management tool, such as [chruby](https://github.com/postmodern/chruby), [rbenv](https://github.com/sstephenson/rbenv), or [rvm](https://rvm.io/).

Second, make sure that the Ruby gem `bundle` is installed:
```
  gem install bundle
```

Now you can install the other required Ruby gems by running:
```
  bundle install
```

## Running the Script

Make sure that your ".bib" files are located in the "data/" subdirectory, and then run:
```
  ruby ap.rb
```
That should output a ".csv" file in the "results/" subdirectory.

## Cleaning the Data

Add the "BibTeX_Export_Impact" style to your EndNote library, and export the EndNote library using this style.

More coming soon ...