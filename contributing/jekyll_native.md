# Install Jekyll natively on your local machine

## Prerequisites

* Ruby has to be installed on your machine
* (Bundler)[https://bundler.io] has to be installed on your machine

Windows user should check out this step-by-step guide to setting up Jekyll on Windows: http://jekyll-windows.juthilo.com/

A compact guide to setting up Jekyll on Mac OS can be found below:

## Step 1: Install Jekyll

Run `bundle install` in the root directory of your local Git repository directory. This will install all of the requirements for running the site locally. 

## Step 2. Run the Jekyll server

You can run the Jekyll service locally with `bundle exec jekyll serve --baseurl=""`. This will compile the site and start serving the content locally. Since compiling can take a while, you can add the option `-V` to get a more verbose output and information about the running compilation steps. Once it's ready, you can open your browser and visit `http://localhost:4000` to see your local version of the site.