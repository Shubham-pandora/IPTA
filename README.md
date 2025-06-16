ansible-playbook deploy.yml -i HOSTFILE  --limit "192.168.0.104" -e "IPTABLES='NO' IPTABLESAUDIT='YES'" -k -v

ansible-playbook deploy.yml -i INV  --limit "192.168.0.104" -e "IPTABLES='NO' IPTABLESAUDIT='YES'" -k -v

ansible-playbook deploy.yml -i inventory/hosts.ini -i inventory/groups.ini -u root --limit "192.168.0.104" -e "IPTABLES='YES' IPTABLESAUDIT='YES' NAGIOS='YES'" -k -v