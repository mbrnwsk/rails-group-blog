#RAILS GROUP BLOG#
Sample **Ruby on Rails** app for collaborative blogging.


###To run###

    bundle install
    rake db:migrate
    rails server

After registration, account must be approved by other registered users. To activate first account and assign the 'admin' role there is a **rake** task:

    rake users:set_admin[user_login]

For example for account with login admin@admin.com:

    rake users:set_admin[admin@admin.com]
