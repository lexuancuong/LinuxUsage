# Preparing

        sudo apt-get update


# Install tweak for ubuntu to swap ESC and Casplock
1. Install `universe` repository
        
        sudo add-apt-repository universe

2. Install Tweaks
        
        sudo apt-get install gnome-tweaks
        
3. Start Gnome Tweak
        
        gnome-tweaks
        
Then swap ESC and Caplocks in tweak's UI

# Generate SSH key and add it to github
- Open Terminal.
- Generate ssh key

        ssh-keygen -t ed25519 -C "your_email@example.com"
    
- Add ssh key to ssh-keygent
    
        eval "$(ssh-agent -s)"
        ssh-add ~/.ssh/id_rsa

- Open Github UI and add that ssh-key into your Github Account

# Generate GCP key then add it into Github account
Follow this guideline
        https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key


# Install fira code and set it for terminal's font

        sudo apt update && sudo apt install fonts-firacode

# Install base environment
Firstly, install git cli

        sudo apt install git
        
You must to press enter when it requires.

        git clone git@github.com:lexuancuong/dotfiles.git
        ./install.sh --ubuntu
        
# Insall Pip3 

        sudo apt install python3-pip

       
# Install YCM
Do after this guideline
        
        https://github.com/ycm-core/YouCompleteMe#linux-64-bit
        
# If you are a vietnamease, you could love ibambo (Vietnamese typing tool)
Work around after this guidline
        https://github.com/BambooEngine/ibus-bamboo

# Install docker
- For ubuntu 21.04. Maybe it be different in other ubuntu versions

        apt install docker.io
        systemctl enable --now docker
        systemctl status docker
        sudo groupadd docker
        sudo usermod -aG docker $USER
        docker --version

# Install docker-compose

        apt -y install docker-compose

# Set up VPN for ubuntu
        https://askubuntu.com/questions/920352/vpn-l2tp-ipsec-client-on-ubuntu-16-04-vpn-service-failed-to-start/1144964#1144964
