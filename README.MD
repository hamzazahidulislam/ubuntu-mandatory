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
