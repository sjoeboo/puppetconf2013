puppet dashboard 2.0

~1 year ago, dashboard was depricated, turned over to community, Aaron Stone picked it up. 

updated to rails 3.2
bundler oriented rail app, gem updates
runs on ruby 1.8.7 and 1.9.3
better rest api
lots of bug fixes and UI tweaks

moving to github under sodabrew

ENC and report processing
Groups

variables form ENC are available as top-level variables in manifests $$::thing_from_enc

classes can be parameterized

groups are internal to the dashboard. inheritance, overridding.

reports. 

key db tuning
innodb_file_per_table
frequent pruning of old reports

upgrading is easy from 1.2 (normal rake db:migrate etc)

node classification is moving to hirea

report processing is moving to puppetdb, has an api etc. 

start using puppetdb as report backend. not there yet.

aiming for ruby 2.0, migration tools to get data out.

updated sharable urls.
