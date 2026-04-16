
```sh
sudo apt update && sudo apt install -y git ansible
```
```sh
ansible-pull -U https://github.com/nanoenjoyer/ansible.git -K
```
> This looks for local.yml in root of repo directory.

> -U is short for URL, -K is short for --ask-become-pass (When you run this, the first thing it will do is prompt you: BECOME password:) if the server doesn't have root password just hit `enter` and it should work.

> You can safely ignore the warnings about hostnames, ansible is used to using hostnames for configuration but since we're just using pull on localhost there will be no host names and thats normal, the pull will still work and tasks will be run.

- only get config files
```sh
ansible-pull -U https://github.com/nanoenjoyer/ansible.git -K --tags config
```
- only get pictures
```sh
ansible-pull -U https://github.com/nanoenjoyer/ansible.git -K --tags pics
```
```sh
source ~/.bash_aliases
```
