1. Check all disks you having
    
    sudo fdisk -l

2. Mount HDD into a specific folder

    sudo mount /dev/sda1 /hdd

3. Run mounting.... 
Stop the server: 

        sudo systemctl stop docker

Create/edit the configuration at /etc/docker/daemon.json, for example: 

        {
        "data-root": "/new/path/docker-data-root"
        }
   
Copy your data there:

        sudo cp -axT /var/lib/docker /new/path/docker-data-root

(if the target docker-data-root directory already exists, make sure you don’t accidentally copy into a docker subdirectory).

Start the server:

        sudo systemctl start docker

Check everything works:

        sudo docker images
