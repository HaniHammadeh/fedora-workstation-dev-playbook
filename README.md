Fedora WorkStation Ansible Playbook
=========

This playbook installs and configures most of the software I use on my fedora workstation  for systems scripting and  day to day lab practices.

Requirements
------------

This playbook has been tested on Ansible Core 2.12.4 and Fedora 36

Role Variables
--------------

There is a default varibale file ***default.config.yml*** which contains the default software I use, I will create a config file that can still override the default one.

Included Application /Packages
------------
## Applications Installed with Fedora package manager

  - firefox
  - chromium
  - transmission 
  - vagrant
  - podman
  - vlc
  - slack
## Packages installed with dnf
  - bash-completion
  - gettext
  - git
  - httpie
  - iperf
  - vim
  - gedit
  - sqlite
  - wget
  - RPM Fusion (Extra Packages Repository, the free one)
 ## Python Packages installed with pip:
  - pandas
  - rich
  - flask
  - waitress

Example of Running the Playbook
----------------

Testing this playbook can be executed by the below command, enter your account  password once propmted for the 'BECOME' password.

>    ansible-playbook main.yml -b --ask-become
   
License
-------

BSD

Author Information
------------------
This playbook created by [Hani Hammadeh](https://github.com/HaniHammadeh "Hani Hammadeh") (originaly inspired by [geerlingguy/mac-dev-playbook](https://github.com/geerlingguy/mac-dev-playbook "geerlingguy/mac-dev-playbook"))
