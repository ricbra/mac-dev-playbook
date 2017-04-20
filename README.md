# Mac Development Ansible Playbook

This repository is a fork of Jeff Geerlings excellent repository: https://github.com/geerlingguy/mac-dev-playbook
It is a stripped version suited to my needs.

For installation:
 
    $ xcode-select --install
    $ sudo easy_install pip
    $ sudo pip install ansible
    $ mkdir projects && cd projects
    $ git clone git@github.com:ricbra/mac-dev-playbook.git
    $ cd mac-dev-playbook
    $ ansible-galaxy install -r requirements.yml
    
    For Ansible < 2.0
    $ ansible-playbook -i inventory --ask-sudo-password main.yml 
    For Ansible >= 2.0 use 
    $ ansible-playbook -i inventory --ask-become-pass main.yml 
    
    $ cd ~/dotfiles
    $ bin/install
    $ bin/setup_osx
