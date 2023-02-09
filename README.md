when setting up wireguard on my ubuntu server, I noticed every restart would get rid of my interfaces so I wrote a script to automatically configure the interface on boot up

1. get the script
2. make the config files in /etc/wireguard
3. make the scripts runnable
4. add to your sudo crontab with "sudo crontab -e" and choose the editor of your choice
5. at the bottom of the crontab, enter "@reboot /path_to_script.sh"
6. verify the crontab was added to the root user with "sudo crontab -l"
7. reboot and see if it worked


this configures one interface of whatever name and pairs it to some IP
