
```sh
sudo apt update && sudo apt install -y git ansible
```
```sh
ansible-pull -U https://github.com/nanoenjoyer/ansible.git -K
```
- only get config files
```sh
ansible-pull -U https://github.com/nanoenjoyer/ansible.git -K --tags config
```
- only get pictures
```sh
ansible-pull -U https://github.com/nanoenjoyer/ansible.git -K --tags pics
```
> -U is short for URL, -K is short for --ask-become-pass (When you run this, the first thing it will do is prompt you: BECOME password:).
> This looks for local.yml in root of repo directory.
```sh
source ~/.bash_aliases
```
