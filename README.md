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
ln -s /path/to/zabbix-userparameter-sidekiq.conf /etc/zabbix/zabbix_agentd.d/userparameter-sidekiq.conf
```

import zabbix-template.xml to zabbix server and attach template to host.

