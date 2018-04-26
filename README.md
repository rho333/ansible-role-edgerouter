EdgeOS_Router
=========

This role configures an EdgeOS router, generating configuration entries for firewall rulesets and rules, network interfaces (LAN), network services (DHCP, DNS), and PPPoE WAN. It uses the `edgeos_config` module, introduced in Ansible 2.5, to apply the
configuration to a target EdgeOS appliance.

Requirements
------------

N/A

Role Variables
--------------

Configuration is generated from a dictionary containing different sections for various aspects of the EdgeOS feature set. An example dictionary is defined in the `vars/` directory.

The configuration must always be passed to the role as the `config` variable.

Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, config: edgerouter_config }

License
-------

MIT

Author Information
------------------

Richard Hofman (richard@hofman.co.nz // @rho_nz // [rho.nz](https://rho.nz))