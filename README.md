# chef-data_bags
My public Chef data bags for experimentation.

Creating the users data bag on the chef server from an existing users directory.
1) First, you need to create the data bag using knife
  $ knife data bag create users

2) Next, upload the databag to the chef server:
  $ knife data bag from file {bag} {item1} {item2} ...
  $ knife data bag from file users data_bags/users/jason.json data_bags/users/doug.json

$ knife data bag list
$ knife data bag show users
$ knife data bag show users/jason
