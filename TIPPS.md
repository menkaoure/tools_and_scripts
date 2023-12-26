## TIPPS
#### Docker / Docker-compose
Problem: "windows max virtual memory areas vm.max_map_count [65530] is too low"  
Solution:
```shell
# Linux
sysctl -w vm.max_map_count=262144

# Windows
## Open powershell, run
wsl -d docker-desktop
## then
sysctl -w vm.max_map_count=262144
```

#### Nginx configure virtual hosts
https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-server-blocks-virtual-hosts-on-ubuntu-16-04#step-2-creating-sample-pages-for-each-site
