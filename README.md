### Проект домашнего задания Ansible SkillFactory

В проекте переконфигурирован _**ansible.cfg**_
```
[defaults]
inventory = /home/ansible/homework_proj/hosts
roles_path = /home/ansible/homework_proj/roles
sudo_user = ansible
```
**roles** и **hosts** находятся в папке проекта.

Задайте адреса управляемых хостов в **_hosts_**
```commandline
# все управляемые машины
[all]
10.0.0.22
10.0.0.32

# хост, на котором будет hginx
[http]
10.0.0.32

# хост, на котором будет php-fpm
[web]
10.0.0.22
```
playbook `add_controller_user.yaml` для выполнения **Задания 1**.

Файлы для проекта переданы в папке **_files_**, перенесите их в `/opt/files` или создайте
символическую ссылку в `/opt`

Рабочая версия сайта: http://158.160.31.162/
