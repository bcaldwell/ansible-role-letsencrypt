Role Name
=========

This role gets SSL/TLS certificate from let's encrypt and sets up a cron job to renew the certificate. 

Requirements
------------

This role currently only supports ubuntu.

Role Variables
--------------

email: email to give to letsencrypt as your contact info
domains: domain names to get certificate for (comma separated)
CF_email: cloudflare email
CF_key: CLOUDFLARE KEY

Dependencies
------------

This role does not have any dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
---
- vars:
    email: user@example.com
    domains: hello.example.com
    CF_email: user@example.com
    CF_key: CLOUDFLARE KEY

  hosts: localhost

  roles:
    - letsencrypt
```

License
-------

MIT
