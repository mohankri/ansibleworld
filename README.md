# ansibleworld
'''

Preparation on new client

sudo adduser ubuntu
sudo apt-get install openssh-server

/etc/sudoers

ubuntu ALL=(ALL) NOPASSWD: ALL

From Development Machine
ssh ubuntu@IPADDRESS mkdir -p .ssh

cat .ssh/id_rsa.pub | ssh ubuntu@IPADDRESS 'cat >> .ssh/authorized_keys'

You have password less login as root and ubuntu user


On Development Machine

Add /etc/ansible/hosts

[ansible-client]
192.168.1.8

Test
ansible-playbook -i /etc/ansible/hosts playbooks/ping.yml

To checkout private repo
ssh-keygen -t rsa -b 4096 -C "name@github.com"
cat ~/.ssh/id_rsa.pub

# Add the key to your github account settings/SSH Keys



'''
