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

# Install fira code and set it for terminal's font

        sudo apt update && sudo apt install fonts-firacode




