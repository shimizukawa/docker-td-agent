# Docker td-agent

Docker image with:

- [td-agent](http://www.fluentd.org/)
- fluent-plugin-elasticsearch
- fluent-plugin-record-modifier
- fluent-plugin-exclude-filter

which do nothing by default.

Fluentd config is `/etc/fluentd/fluent.conf` could be easily override by volume.

`-v /path/to/fluentdconfdir:/etc/fluentd`


# Simple usage

`docker run -d -v /path/to/fluentdconfdir:/etc/fluentd shimizukawa/td-agent`

# settings

PATH

- `/etc/fluentd/fluent.conf`: td-agent config file
- `/var/log/td-agent/`: td-agent log directory

default fluent.conf

- see: [fluent.conf](https://github.com/shimizukawa/docker-td-agent/blob/master/etc/fluentd/fluent.conf)

