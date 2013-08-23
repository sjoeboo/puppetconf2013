Razor

started by EMC/VMware

1 year old

unlike other tools, you don't have to treat everyhign as pets. no need to enter mac adresses etc. 

razor lets you treat them all as cattl.e 

ipxe. (http)
hardware discovery and inventory (facter)
tagging and policies

handoff to puppet.

microkernel -> runs facter, sends to server.
then you can classify systems based on the discovered facts. 

postgres +sinatra + tourquebox

components:
 * server
 * cli
 * mircokernel agent
 * microkernel image
 * UI

microkernel:
	agent = seperate
	build on EL / fedora
	~150MB
	
server api:
	json
	rest
	async

cli

tags, a rule w/ a name. (group mac addresses, any facts, booleanlogic).

policy ~ cobbler profile...ish

installers = yaml +erb, could be kickstarts etc. API for node to get info from server. 

systems pxe everytime, but, you define how many times to boot into the installer, or local (ie, boot the installer, then default to booting local). These are all ipxe files. 

release soon (~2 weeks)

demo


