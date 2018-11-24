[![GoKEV](http://gokev.com/GoKEV200.png)](http://GoKEV.com/)

<div style="position: absolute; top: 40px; left: 200px;">

# GoKEV-AnsibleTower-Backup

This project uses Ansible Tower's RESTful API to backup specific pieces of the configuration.
  - The end result is a sanitized file (you will need to re-add passwords and keys to the credentials)


## Example Playbook
Here's an example of how you could launch this

<pre>
---
---
- hosts: localhost
  gather_facts: no

  vars:
    tower_server: inventory-recognzed-tower-server-name.whatever
    tower_user: admin
    tower_pass: mytowerpassword
    tower_action: backup
#    tower_action: restore


  roles:
    - "GoKEV-tower-{{ tower_action }}"


</pre>


## Troubleshooting & Improvements

- Not enough testing yet

## Notes

  - Not enough testing yet

## Author

This project was created in 2018 by [Kevin Holmes](http://GoKEV.com/).


