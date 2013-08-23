intro to system orchesrations w/ mcollective. 

what is orchestration? 

the automated coordination of multiple systems.

server = mcollective daemon runnong on all nodes. 
middleware = pub/sub middlewear, things talk to this. 
client = where cms are run, talks to middleware, which sends to clients. 

mcollective is a framework. to leverage, you need to add plugins. 

plugins:
agents : tasks
secrutiy: auth etc
connector: middleware
data: more advance ways to filter/group nodes. 

agents:
	package agent, leverages puppets pacakge type. 
	mco package rsync status (gets the status of the rsync pacakge on all systems)
	
	service agent, leverages puppet serice type.
	mco service http status/start/stop etc. 

	puppet agent lets you run puppet. can run X at a time. 
	mco puppet count
	mco puppet summary

	mco filemgr status --file/tmp/devon.txt
	mco puppet resource file /etc/devon.txt content="blah"
	
	agents are NOT just chipping shell code out
	so if you want an exec, do
	mco puppet resource exec something cmd="rm -rf /tmp/matt"

			
filtering:
	by id
	classes
	facts
	collectives

	collectives, the most basic node grouping in mcollective.
	nodes can be in multiple collectives. (compute, storage, cluster, access, service, global, holyoke/campus)
		
