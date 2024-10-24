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

https://hackprogramming.com/blog/how-to-setup-subdomain-or-host-multiple-domains-using-nginx-in-linux-server

#### Postgresql
- Execute sql File from psql
```sql
# specificities of windowns environment (use slash and not backslash)
\i 'C:/temp/test_tables.sql'
```
#### Linux LVM
https://www.linkedin.com/pulse/how-add-discover-new-disk-create-lvm-linux-virtual-machine-khating/

#### Powershell
```ps1
netstat -ano | findstr <str>
taskkill /F /PID <pid>
```

#### VMWare Windows 11 & Server blue Screen (Unsupported Processor)
[ypervisorlaunchtype auto](https://www.deskmodder.de/blog/2022/08/22/vmware-installation-der-windows-11-insider-und-windows-server-2022-werden-mit-unsupported-processor-beendet-workaround/)

```
bcdedit /enum
bcdedit /set hypervisorlaunchtype off
```

#### Mac
Install Minikube on MAC arm64-based systems without any issues
https://devopscube.com/minikube-mac/
