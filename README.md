# vagrant-ansible-lab-virtualbox
### Credits: [ginigangadharan](https://github.com/ginigangadharan)

### Forked From: [vagrant-iac-usecases](https://github.com/ginigangadharan/vagrant-iac-usecases/tree/master/virtualbox-ansible-lab)
#
## This Vagrantfile creates 2 ansible nodes & 1 ansible engine. However, this script will not work in WSL/WSL2

#
## Steps to Run:
#
1. Clone the github repo
2. Make sure [Virtualbox](https://www.virtualbox.org/) is installed

3. Make sure [Vagrant](https://www.vagrantup.com/downloads) is installed

4. Make sure you have ssh keys present in ~/home/user/.ssh/ Follow this [Guide](https://www.digitalocean.com/community/tutorials/how-to-create-ssh-keys-with-openssh-on-macos-or-linux) to generate ssh keys

5. Navigate to the location of the repository

6. Run this command: ``vagrant up``

7. List status of running machines using: ``vagrant status``

8. Login to ansible-engine: ``vagrant ssh ansible-engine``

9. Check if you can ping ansible nodes: ``ping ansible-node-1``
#
### Congrats! You can now work on Ansible. Want to code in vs-code?
#
1. You can open SSH into the remote container from vs-code using [remote-ssh](https://marketplace.visualstudio.com/items?temName=ms-vscode-remote.remote-ssh).

2. To get the ssh config file for ansible-engine type ``vagrant ssh-config`` & copy the configuration for ansible-engine

3. Copy the output your SSH config file — I added it to my default SSH config at ~/.ssh/config

4. You can use this info to SSH into container through vs-code & write scripts easily

### To shut down the machines run: ``vagrant halt``
