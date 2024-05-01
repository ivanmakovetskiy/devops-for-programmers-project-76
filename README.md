### Hexlet tests and linter status:
[![Actions Status](https://github.com/ivanmakovetskiy/devops-for-programmers-project-76/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/ivanmakovetskiy/devops-for-programmers-project-76/actions)


## Подготовка к деплою

1. Установите Ansible:
```bash
sudo apt update
sudo apt install ansible
```
2. Установите необходимые роли и коллекции:
```bash
ansible-galaxy install -r requirements.yml
```
3. Подготовьте файл инвентаризации inventory.ini, пример уже предоставлен в проекте.




## Запуск проекта

Можно выполнить основной плейбук для деплоя:
```bash
ansible-playbook -i inventory.ini playbook.yml
```

Еще можно запускать конфигурацию одной командой:
```bash
make setup
```
