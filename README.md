# ansible-network-troubleshooting

## Background
This repository should be considered a template only. My typical setup is orchestrated with Jenkins with a number of
environmental variables being passed to an ephemeral Ansible container. I also use AWS SSM for secret management.

## Roles

### network-test
This role has a number of functions that can be run, either on demand or in sequence.

### iperf
This role installs an iperf container as a server. There's an example Dockerfile in the role folder.

### speedtest
This role installs a scheduled speedtest (runs in a container). There's an example Dockerfile in the role folder.

