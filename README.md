Local provisioning for a new ubuntu machine
====================


Steps:

On your new machine, you first need ansible.  Best way to install on the mac is:

```
easy_install --user pip
pip install --user ansible
```

You also need to generate a keypair and add it to your github, as this script clones my [dotfiles repo](https://www.github.com/dgliwa/dotfiles)

After cloning this repo:

```
cd ./local-provisioning
ansible-playbook playbook.yml
```

You will need to do a restart for you changes to the shell to take place, then come back to this directory and run:

```
ansible-playbook finish-playbook.yml
```
