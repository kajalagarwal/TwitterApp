#Ruby and rails version
  * Ruby=2.0.0 
  * Rails=4.2.2
  
#Application URL on Heroku
 * Running live at 
    * https://kajalagarwal-rails.herokuapp.com/
  
# Running app locally
  * `bundle install`
  * `rails server`
  *  `bundle exec rake db:migrate`
  
#Deployment instructions on Heroku
 
  * Push all the assets on the clouds first
    * `RAILS_ENV=production bundle exec rake assets:precompile`
  * First Get the heroku login and create an app.
  * Git add and commit
  * Login to heroku using 
    * `heroku login`
  *  Create the heroku name
    * `heroku create`
  *  push to heroku
    * `git push heroku master`
  *  migrate your db
    * `heroku run rake db:migrate`
 
# Run Test cases
     * `bundle exec rake test:models` to run the test cases of models created
     * `bundle exec rake test` to run all the test cases related to app (model, view, controller).
 
# Special Gem includes
  * `gem 'faker'`
  * `gem 'will_paginate'`
  * `gem 'rspec-rails'`


# Code Documentation
  * Based on the theme of social website like twitter where you log in as an individual and either read or tweet the post.
  * This app also contains a Rails Faker gem for randomly generating the fake data.
  * Paginated gem for paginate the micropost pages.
  * For unit testing it is using rspe.
