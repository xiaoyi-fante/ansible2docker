# ansible2docker
Through Ansible playbook to install docker 19.03.1

```[root@localhost docker]# ansible-playbook docker_install.yaml

PLAY [docker] ************************************************************************************************************

TASK [Gathering Facts] ***************************************************************************************************
ok: [10.211.55.8]

TASK [docker install] ****************************************************************************************************
[WARNING]: Consider using 'become', 'become_method', and 'become_user' rather than running sudo
changed: [10.211.55.8]

TASK [shell] *************************************************************************************************************
changed: [10.211.55.8]

TASK [shell] *************************************************************************************************************
changed: [10.211.55.8]

TASK [shell] *************************************************************************************************************
changed: [10.211.55.8]

TASK [docker config dir] *************************************************************************************************
changed: [10.211.55.8]

TASK [file transfer] *****************************************************************************************************
ok: [10.211.55.8]

PLAY RECAP ***************************************************************************************************************
10.211.55.8                : ok=7    changed=5    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0```

On the remote server
```[root@8 Dockerfile]# docker info
Client:
 Debug Mode: false

Server:
  ...
 Server Version: 19.03.1
 Storage Driver: overlay
  Backing Filesystem: extfs
  Supports d_type: true
 Logging Driver: json-file
 Cgroup Driver: cgroupfs
  ...
 Docker Root Dir: /data/docker
  ...```
