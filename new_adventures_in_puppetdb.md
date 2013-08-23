puppet generates LOTS of data. 

agent collects facts about self. sends to master.
master takes facts, generates a catalog. (compiled puppet code/graph)
send catalog to agent (master discards it), 
agent runs catalog, discards it.
agent generates report, which is the result of the catalog (catalog is what was supposed to happen, report is what DID)
agent send report to master, master does something w/ the report. 

w/ puppetdb
master sends facts received to pupeptdb
master sends catalog to puppetdb
master sends report to puppetdb
nothing tossed out. 

Command 
Query
Responsabiliy
Seperation

async,paralell, mq-based(internal).

since writes are async, commands are queued. just like smtp. litterally. exponential backoff, for like 9 hours. 
dead letter office = bit for bit copy, great for support. 

puppetdb expects failure. 

JVM

can ship an uberjar, jar w/ all deps. 

puppet-puppetdbquery
(use this to make nagios way faster!)
hiera backend to yank data from puppetdb
plugin for mcollective!

single instance resource storage (de-dup)
same for catalogs

in the field, resource/catalog duplication rates are mostly 85% +
so puppetdb doesnt need to WORK 85% of the time. 

2 nagios plugins! 
puppetdb-external-naginator

on by default in PE3 

automatic MQ corruption fixes
compression od DLO
purge inactive node data
db connection recycling. 
backup and restore. 

complex queries (all the ndoes running httpd, give me their IP addresses). 

can store reports. 

streaming queries coming. 
replication coming
more flexible routing, softfailures, etc


