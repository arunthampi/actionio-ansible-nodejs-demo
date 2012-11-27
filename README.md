# Ansible Demo on Action.IO

This is a demo of ansible, used to install node.js on an Action.IO
python box. This was demo'ed during the Singapore DevOps Meetup on 28th
November, 2012.

* Bring up a Python-based box on action.io
* Create a virtualenv called ansible, using `virtualenv ansible`
* Run `source ~/ansible/bin/activate`
* Install the dependencies for ansible with this command `pip install pyyaml jinja2
  paramiko`
* Clone the ansible repository `git clone
  git://github.com/ansible/ansible.git`
* Install ansible `cd ansible && python setup.py install`

# Running the playbook

Once you have cloned this repository, `cd` into it and run this command
to install node:

`ansible-playbook install_nodejs_via_nvm.yml -i hosts`
