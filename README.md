# zabbix-nginx

Configure Zabbix agent to monitor Nginx.

Role Variables
--------------


### zbx\_ngx\_conf\_d

Nginx configuration definition directory. Default: `/etc/nginx/conf.d`.

### zbx\_ngx\_script\_dir

Directory for Nginx querying script. Default: `/usr/local/bin`.

### zbx\_ngx\_userparams\_dir

Zabbix agent configuration definition directory. Default: `/etc/zabbix/zabbix_agentd.d`.

### zbx\_ngx\_port

Port (on IPv4/IPv6 loopback interface) on which Nginx will listen for stub\_status requests. Default: 10000.

### zbx\_ngx\_status\_uri

Location, at which Nginx will serve status info. Default: `/`.

Dependencies
------------

* zabbix-agent

Example Playbook
----------------

		- hosts:
				- foo
			roles:
				- zabbix-nginx

License
-------

GPLv3+

Author Information
------------------

Ansible role by Development Gateway. [Scripts and configuration](https://github.com/jizhang/zabbix-templates) by [Ji Zhang](https://github.com/jizhang).
