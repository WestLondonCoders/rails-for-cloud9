# Setting up Cloud9

Once you've created an account and started a blank project that clones this repository, do the following:

Install Ruby 2.4.2 by typing the following into the terminal at the bottom:

`rvm install ruby-2.4.2`

Then use that version by typing:

`rvm use 2.4.2`

Install bundler:

`gem install bundler`

Install the gems this Rails app depends on:

`bundle install`

### Setup the database

Start Postgres on your virtual server by typing into the terminal:

`sudo service postgresql start`

Then to create the database, where Rails will store your data, type:

`bundle exec rails db:create`

### Running the server

Type the following into the terminal to run Rails on Cloud9:

`rails server -b $IP -p $PORT`

Visit `projectname-username.c9users.io` to see your new web app for the first time.
