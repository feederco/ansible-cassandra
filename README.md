# ansible-cassandra
Ansible provisioning/maintenance tasks for Cassandra

Usage:
1) Create the servers for Cassandra and Datastax OpsCenter
2) Define an Ansible inventory (see inventory/example.hosts) for your environment
3) Run the playbook to install Cassandra + Datastax OpsCenter

Inventory configuration:
1) cassandra_nodes
   a) seed=[true, false] (is the node a seed)
   b) repair_weekday=[MON,TUE,WED,THU,FRI,SAT,SUN] (which day(s) to run repair)

Requirements:
- Ansible 1.8 or later
- Ansible general configuration: "jinja2_extensions = jinja2.ext.do"
- Nodes running Ubuntu 14.04 or later
