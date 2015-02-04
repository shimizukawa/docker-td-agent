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

