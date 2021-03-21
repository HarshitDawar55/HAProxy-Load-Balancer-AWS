<img src = "https://img.shields.io/badge/version-1.1.0-brightgreen" />

HAProxy-Load-Balancer-AWS
=========

This role is designed to install & configure the HAProxy Load Balancer specifically for AWS, although it can be used anywhere else, then only firewall rules has to be taken into consideration!

Requirements
------------

* boto package(because EC2 Module is used).
* ec2-scripts which will fetch the IP of the EC2 instances dynamically(if dynamic inventory of Ansible is used!).
    * [ec2.py](https://github.com/HarshitDawar55/Ansible/blob/master/Dynamic-Inventory/ec2.py)
    * [ec2.ini](https://github.com/HarshitDawar55/Ansible/blob/master/Dynamic-Inventory/ec2.in)
* If the dynamic Inventory is used, hosts should be assigned using the tags given to the instances! 

Role Variables
--------------

No Variable is used in this role, although there are some points to be noted:
<br />
<b>Note:  All the instances launched to act as Webservers, should be launched having a key as "Type" & value as "Webservers". <i>(It is case-sensitive)</i> </b>

Dependencies
------------

Nil

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: tag_Type_LB
      roles:
         - HAProxy-LB-AWS

License
-------

[MIT](https://github.com/HarshitDawar55/HAProxy-Load-Balancer-AWS/blob/master/LICENSE)

Author Information
------------------

Developed by Harshit Dawar, also known as Technologist, a public speaker, extrovert, & optimist.

**LinkedIn:** https://www.linkedin.com/in/harshitdawar

**PortFolio:** https://harshitdawar55.github.io

**Twitter:** https://www.twitter.com/harshitdawar55

**Medium:** https://harshitdawar.medium.com

**GitHub:** https://www.github.com/harshitdawar55
