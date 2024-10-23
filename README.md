# ansible -i <inventory.yml> -m shell -a 'ls' lxc - used to run shell commands, cam be done to evalutate post ansible deployments

to run ansible and authenticate using password = install sshpass on controlnode and then mention this --ask-pass in ansible command.

setup module = ansible gather facts

ansible-doc ansible.builtin.setup

ansible-galaxy collection init --init-path collections/ansible_collections ansible.tutorial ansible=namespace, tutorail= collection


run playbook in collections : first set the right path of collections using either export ANSIBLE_COLLECTIONS_PATH=./collections or add path in ansible.cfg : ansible-playbook ansible.tutorial.ping 


always login to the managed node using nonroot user, refer user role and non_root_user playbook for this. 