# pushkey
push ssh ansible host key to another host

If you are managing multiple nodes and don't want to enter a password each time a playbook is run or manually push keys to each host one by one this script will let you run a playbook to automatically push keys to each host.

Requirements:

1. Generate you public keys on your ansible host.
2. Set "host_key_checking = false" in ansible.cfg file
3. Run the playbook using the following variables:
   ansible-playbook -i /etc/ansible/hosts pushkey.yml --ask-pass
   
