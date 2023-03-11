Role Name
=========

Start the iperf3 container as a server.

Requirements
------------

Docker

Role Variables
--------------

```yaml
# Docker vars
iperf_log_driver: "json-file"
iperf_log_maxsize: '1g'
iperf_log_maxfile: '7'
iperf_image: privaterepo/iperf3
iperf_image_tag: latest
```

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---
- hosts: network-utility
  become: yes
  roles:
    - iperf
...

