automation-challenge server configuration
=====================

The Ansible playbook in this repo is designed to upload and update a single template file.   
It has been tested using vagrant and the current source (a37a84243b968087668a3c2e73b5032b6d3ceeee) of Ansible.  

To run this playbook:
- Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- Install [Vagrant](http://docs.vagrantup.com/v2/installation/)
- git clone the [Ansible Source](https://github.com/ansible/ansible)
- Follow Ansible [instructions for running from source](http://docs.ansible.com/intro_installation.html#id12)

#### Example
```
<ansible source path>/ansible-playbook -i <path_to_playbook>/hosts.ini --private-key=~/.vagrant.d/insecure_private_key -u vagrant <path_to_playbook>/site.yml -vv
```

#### Output
```
PLAY RECAP ******************************************************************** 
localvm                    : ok=4    changed=2    unreachable=0    failed=0   

```

#### Additional hosts

You can add hosts to update by editing the hosts.ini file. 


Reference
[Automation Challenges](https://github.com/meconlin/automation-challenges/tree/master/log%20scraper)
