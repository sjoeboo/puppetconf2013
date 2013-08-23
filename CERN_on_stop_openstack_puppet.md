
* 270 oepnstack hypervisors
* 4K vms
* 300 users
* 14 puppet masters
* 6 foreman backend nodes

Goals:
ramp ups to 15K hypervisors
multi-site

git workflows:
	manifests/module/heirdata = git version controlled. 
	puppetmasters syc w/ git on thier own.
	wasn't scaling

	So
	
	"Jens"
	PuppetFiles
	Each module has its own repo, prod and dev branch. 
	

Foreman for provisioning, ON openstack. hooks into puppet.

koji for repo mgmt	
