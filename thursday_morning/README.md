README.md - Palo Alto Setup
install collection: github: https://github.com/PaloAltoNetworks/pan-os-ansible galaxy: https://galaxy.ansible.com/ui/repo/published/paloaltonetworks/panos/

to install from galaxy.ansible.com version 2.19.0:

ansible-galaxy collection install paloaltonetworks.panos==2.19.0

to install from github main branch:

ansible-galaxy collection install -r requirements.yml

example requirements.yml:

collections:
   - name: paloaltonetworks.paloaltonetworks
     source: https://github.com/PaloAltoNetworks/pan-os-ansible/
     version: main
vist the collection on github, and get a copy of requirements.txt (alternatively look @ documentation)

install requirements.txt (python requirements):

python3 -m pip install -r requirements.txt

Run the playbook:

ansible-playbook playbook.yml
