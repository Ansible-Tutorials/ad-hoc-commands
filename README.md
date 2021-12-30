# Ad-hoc commands on Ansible

### `File Transfer`
```
$ ansible atlanta -m copy -a "src=/etc/hosts dest=/tmp/hosts"
$ ansible webservers -m file -a "dest=/srv/foo/a.txt mode=600"
$ ansible webservers -m file -a "dest=/srv/foo/b.txt mode=600 owner=mdehaan group=mdehaan"
$ ansible webservers -m file -a "dest=/path/to/c mode=755 owner=mdehaan group=mdehaan state=directory" (The file module can also create directories, similar to mkdir -p)
$ ansible webservers -m file -a "dest=/path/to/c state=absent" (As well as delete directories (recursively) and delete files:)
```




