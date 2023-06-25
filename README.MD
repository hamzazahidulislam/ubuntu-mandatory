# Ubuntu Installation and Disk Partition

### partition image

![1](./assets/1.jpg)

![2](./assets/2.jpg)

### After installation

### Please make sure display font size and setting appearance make it up to you

### And if you install chrome then please make sure you sue **GTK** Them for better UI & UX

### some linux wildcards

### ls document\_\* , ls \*.txt

     ls file.?.csv

     cat files/*.csv

     cp files/* .

     rm *.csv

     rm document_*

     touch file_10.txt

     rm file_?.txt

     ls -l *.xml

![2](./assets/1.png)

### Important tool for networking

     sudo apt install net-tools

### Holding "Backspace" deletes only one character

     gsettings set org.gnome.desktop.peripherals.keyboard repeat true

### Font size increase

     sudo apt install gnome-tweaks

### For update system

     sudo apt-get update

# SSH Key Agent Setup

### Generating ssh key

     ssh-keygen -t ed25519 -C test@gmail.com

### Set ssh key in ssh-agent

     eval "$(ssh-agent -s)"

## Make ssh config file for store our .peb file or private key

     touch ~/.ssh/config

### Open the file

     nano ~/.ssh/config

### Writing the following value

     Host *
     AddKeysToAgent yes
     IdentityFile ~/.ssh/id_ed25519

### Add into SHH

     ssh-add ~/.ssh/id_ed25519

### Copy the public key

     cat ~/.ssh/id_ed25519.pub

### check your SSH connection

     ssh -T git@github.com

     ssh -T git@gitlab.com

     ssh -T git@bitbucket.org

# Install multi-media code & VLC Player

     sudo apt install ubuntu-restricted-extras && sudo apt install vlc

### unzip file

     unzip /path/to/file.zip -d temp_for_zip_extract

## Enable minimise on click

     gsettings set org.gnome.shell.extensions.dash-to-dock click-action "minimize"

## Enable Firewall

     sudo systemctl status ufw

     sudo systemctl enable ufw

     sudo ufw enable

     sudo ufw disable

     sudo ufw status

     sudo ufw allow 22/tcp

     sudo ufw deny 22/tcp

## Use FlatPak Instead of Snap

     sudo apt install flatpak

### flatpak.org search in brower

- Please make sure first add flat repository
- Also add flatpak plugin
- after restart pc

### Speed up app launch time Preload

     sudo apt install preload

# Live Patch

     uname -ar
     uname -a

- You have to create Ubuntu account use this future
- Free to use up to 30 machines
- Go to software update and active live patch
- Token you get from UBuntu website

### If you want you use keboard shortcuts please. Go setting inside keyboard shortcuts and set as you need

## If you need system backup

- then use timeshift tool

## Use Windows app

- Then use the Bottles tool
- Or you can use wine for small app like lighshot tools

## If you use Ubuntu then you lapto bettery very fast decrease the charge then you should try this app instad

` sudo apt install tlp tlp-rdw`

`sudo systemctl enable tlp`

` sudo systemctl start tlp`

## clean you junk file

     sudo apt install bleachbit
