# zabbix-mastodon-sidekiq
Zabbix template for monitoring sidekiq of mastodon.

## dependencies
- zabbix
- zabbix-agent
- redis-cli

## setup

clone this repository.

```
# git clone https://github.com/kedamaDQ/zabbix-mastodon-sidekiq.git
```

copy or link zabbix-userparameter-sidekiq.conf to zabbix_agentd.d.

on ubuntu:

```
ln -s /path/to/zabbix-userparameter-sidekiq.conf /etc/zabbix/zabbix_agentd.conf.d/userparameter-sidekiq.conf
```

restart zabbix_agentd

```
# systemctl restart zabbix_agentd
```

import zabbix-template.xml to zabbix server and attach template to host.

