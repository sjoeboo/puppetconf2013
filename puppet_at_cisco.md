Cisco's Saas Offerings, connect, webex, cisco social.

millions of meetings, 10's of millilions of users. 

no scheduled downtimes. 

7K hosts, 8 data centers, iPops,private backbone

how do you evolve the system w/o turning it off? 

easy to be overwhlemed by the scale and complexity. but when broken down into component parts...
assembled into the systems. 

never run 1 of anything. clusters.

upgrade by dc/cluster, by node?

cluster managment requires a later of definition and controler above puppet. 

TOSCA/HEAT

salt/mcollective/fabric for orcestration

puppet for config. mgmt. 

masterless? sometimes. 
robust packaging systems.

webex uses everything. multiple masters, masterless, multiple orcestration tools.
heterogenious application stacks and mgmt of those stacks. no  "one solution"

how do you eat an elephant? one bite at a time. 

bundle modules together.
 
role profile modules

puppet librarian puppetfile

cooperitive modules: loosly coupled modules, work together IF installed together, but can stand alone..

push as much as possible out of rpm deps. put deps in puppet, more transparent. 4am proofing. 

 
