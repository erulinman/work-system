# Ansible role for installing arch-linux based user software
## Role list (main)
---
* alacritty
* android-studio
* applications
* aur-user
* dunst
* i3wm
* idea
* firefox
* fonts
* greenclip
* java
* kotlin
* neovim
* nvidia
* pacman
* picom
* polybar
* python
* rofi
* sound
* thunar
* time
* xorg

## Run playbook
---
### Over ansible
```bash
ansible-playbook -i inventory main.yml -K --connect=local
```
### Over bash script
```bash
bash install.sh
```
## Check only one role
---
```bash
ansible  localhost -m include_role -a name=$ROLE -e home=$home -e user=$USER
```
## Some cool
---
```bash
fc-list|grep Awesome -- check fonts name
```
## TODO
---
- [ ] set dunst config
- [ ] aliases /etc/bash.bashrc
- [ ] anky app install
- [ ] nvidia role: dont know how work + xorg.conf copy
