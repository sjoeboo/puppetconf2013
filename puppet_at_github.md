Puppet @ github

@wfarr

operations

boxen: 240 modules, github, puppet 3.latest hiera, for building OSX systems. Linux support in progress.

github/puppet = used to manage infrastructure/office/etc

~5 years old. still on 2.7. 121 modules ~280K lines of code

15.5K commits to master, all employees can commit. 

Single Master, bare metal.

Install w/ ruby gems. 1.8.7
Unicorn. ~600 Nodes, some bare metal, some virt. 
run hourly via cron, no agent.
puppetdb
nagiosdb - does api calls to build configs, WAY faster than running puppet, but uses the collected resources.
filtergendb

gPanel - internal version of puppetdb/puppet-dash/foreman/etc

puppetdb:
inventory

pupppet-lint religiously. can fix things for you. 
rspec-puppet

augeas

how github ships puppet
jenkings test suite. 
test-queue


branch deploy everything. 181 environments. 

ChatOps, 202 eployess, all w/ puppet access. 
all puppet runs go to chat, all output. 


