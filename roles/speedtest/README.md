# Speedtest (ROLE: speedtest)

## Prerequisites

1. This role currently only supports Linux
2. A Datadog account
3. A Dockerhub repo hosting a speedtest-cli container

## Purpose

This role installs a cron job that runs the speedtest Docker container on an hourly basis and reports the information directly to Datadog for reporting purposes.

## Installation

The following variables need to be configured as host_vars for the applicable server(s).

```
---
# Speedtest parameters
#speedtest_ddip: "localhost"
speedtest_site: "home"
speedtest_isp: "aol"
...
```

### speedtest_ddip

If changed, this could allow data to be passed to a specific Datadog / logging instance

### speedtest_site

Tag used to notate site.

### speedtest_isp

Tag used to notate ISP.

