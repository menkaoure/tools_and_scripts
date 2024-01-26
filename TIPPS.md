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
