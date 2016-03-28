[![Build Status](https://travis-ci.org/jvalentini/ansible-role-blog-ghost.svg?branch=master)](https://travis-ci.org/jvalentini/ansible-role-blog-ghost)

Blog-Ghost
=========

Configures a Ghost server on Digital Ocean with the proper hostname info.

References [How To Use the DigitalOcean Ghost Application](https://www.digitalocean.com/community/tutorials/how-to-use-the-digitalocean-ghost-application)

Requirements
------------

- An existing Digital Ocean droplet with Ghost installed.

Role Variables
--------------

Required:

```
hostname: blog.example.com
mail_user: postmaster@blog.example.com
mail_pass: 4j6f0f65893054e2ada96a5babj23l1234
```

Defaults:

```
nginx_ghost_conf: /etc/nginx/sites-available/ghost
ghost_conf: /var/www/ghost/config.js
url: http://{{ hostname }}
mail_service: Mailgun
```

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: blog
      roles:
         - { role: jvalentini.blog-ghost, hostname: blog.example.com }

License
-------

MIT

Author Information
------------------

Justin Valentini
