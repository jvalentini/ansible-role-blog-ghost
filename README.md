Blog-Ghost
=========

Configures a Ghost server on Digital Ocean with the proper hostname info.

References [How To Use the DigitalOcean Ghost Application](https://www.digitalocean.com/community/tutorials/how-to-use-the-digitalocean-ghost-application)

Requirements
------------

- An existing Digital Ocean droplet with Ghost installed.

Role Variables
--------------

`hostname: blog.example.com`

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
