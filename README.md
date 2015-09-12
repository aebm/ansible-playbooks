# ansible-playbooks
Playbooks to provision machines

## Steps
* Install python and virtualenv
  ```bash
  $ sudo apt-get update
  
  $ sudo apt-get install --no-install-recommends python virtualenv build-essential python-dev
  ```
* Install Ansible in a virtualenv
  ```bash
  $ virtualenv --clear --always-copy ansible
  
  $ source ansible/bin/activate
  
  $ pip install -U ansible
  ```
* Create inventory file

  ```bash
  $ echo "localhost ansible_connection=local ansible_become=true" > inventory
  ```
* Test Ansible

  ```bash
  $ ansible all -i inventory --ask-become-pass -m setup
  ```
