#!/bin/sh
xcode-select --install
sudo xcodebuild -license
/usr/sbin/softwareupdate --install-rosetta
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python3 get-pip.py
sudo pip3 install --ignore-installed ansible
ansible-galaxy install -r requirements.yml

ansible-playbook -i "localhost," -c local ansible_osx.yml --ask-become-pass
