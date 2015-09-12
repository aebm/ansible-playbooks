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
