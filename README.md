Install Xcode

Accept license:

```
sudo xcodebuild -license
```

Install Ansible

```
sudo easy_install pip
sudo pip install --ignore-installed ansible
```

Get community.general collection:

```
ansible-galaxy install -r requirements.yml
```

To run playbook:

```
ansible-playbook -i "localhost," -c local ansible_osx.yml --ask-become-pass
```

You can run a role directly with:

```
ansible localhost -m include_role -a name=dnsmasq --ask-become-pass
```

## Structure

- 


