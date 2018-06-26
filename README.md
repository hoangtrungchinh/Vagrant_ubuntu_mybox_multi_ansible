# Vagrant_ubuntu_mybox_multi_ansible

===============================
ansible-doc apt
ansible-doc -l | grep become
ansible-doc setup

===============================
vagrant up

vagrant global-status

ansible -i inventory.ini all -m ping
ansible -i inventory.ini all -a "hostname"
ansible -i inventory.ini all -a "df -h"
ansible -i inventory.ini all -a "du -hs /home"
ansible -i inventory.ini all -a "free -m"
ansible -i inventory.ini all -a "python --version"

ansible -i inventory.ini all -b -m apt -a "upgrade=yes"


#INSTALL PYDF
ansible -i inventory.ini all -b -m pip -a "name=pydf state=present"
ansible -i inventory.ini all -a "pydf"
