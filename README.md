Blog-Ghost
=========

Configures a Ghost server on Digital Ocean with the proper hostname info. References: https://www.digitalocean.com/community/tutorials/how-to-use-the-digitalocean-ghost-application?utm_source=Customerio&utm_medium=Email_Internal&utm_campaign=Email_GhostWelcome

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
