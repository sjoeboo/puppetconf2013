
recent deployment

lots of inovation

$5,200 payment volume/second

build a new system for deploying system and application software.
across datacenters

4000+ pacakges, 100GB of code to deploy.

12-20 masters, depending on how you count. redundancy+load. 
yum for pkg storage. 
heira = mongodb
REST api to integrate w/ other tools, like openstack heat, etc. 

dev put requst into portal, openstack heat deploys vms, registes w/ heira, agents run, deployment happens. 

project velocity ^^

ninja engine, takes list of apps you want to install, assemble the list of pkgs, autodiscover deps, generate puppet resoureces, execture. 

roles and labels

role = set of pkgs to insall
label = set of versioned packages, backed by yum repo.

system hierarchy

env -> geo -> dc -> pool -> host

sclaing activemq,removed load balancer, to activemq cluster. 

mcollective is huge for paypal
