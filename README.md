# Ad-hoc commands on Ansible

### `File Transfer`
```
ansible atlanta -m copy -a "src=/etc/hosts dest=/tmp/hosts"
ansible webservers -m file -a "dest=/srv/foo/a.txt mode=600"
```
