24 million monthly active users

using puppet for 3 years. 
450 changes per month
220 commiters to git
325 puppet modules

reviews w/ gerrit

run puppet via cron
masters do 1 compile per worker process, then die. 
5 minute mod_memcache in apache for file(source) resources

dynamic environemtns git branch = env
code review manditory to make it to production

debian shop, through and through.

storage in cassandra, postgresql, and tokyocabinet

custom module, dalen-dnsquery to look up dns IN a manifest, most for SRV records. 

different ENC's in each puppet deployment, plan onmoving to heira for all of them

https://github.com/dalen/puppet-puppetdbquery

https://github.com/dalen/dm-puppetdb-adapter

future
split the repo out
vagrant testing
building images using masterless puppet apply
