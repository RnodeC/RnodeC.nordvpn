rnodec.nordvpn
=========

This ansible role sets up nordvpn, which configures a server to use the vpn for all it's network traffic.  

Requirements
------------

None

Role Variables
--------------

* `nordvpn_server`: the specific server to connect to.  default = let nordvpn choose
* `nordvpn_token`: (PRIVATE) access token


Dependencies
------------

None

Example Playbook
----------------

```bash
- hosts: all

  vars: 
    nordvpn_server: true 
    nordvpn_token: thisshouldbeinansiblevault

  roles:
  - RnodeC.nordvpn
```

Author Information
------------------

RnodeC - rnodec.io
