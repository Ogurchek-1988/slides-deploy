# Настройка системы для выполнения данного задания: #


#### Дистрибутив: 

- ubuntu server 20.04

#### Сгенерировать ssh ключи: 

 `ssh-keygen`

#### Установить сертификаты: 

 `sudo apt-get install ca-certificates`

#### Установить pip: 

 `sudo apt -y install python3-pip`

#### Установка ansible: 

 `sudo apt install ansible`

#### Настройка ansible.yml:


>  name: Clone repository, copy fig and slides to csa/fp/se-am, and launch docker-compose

>  hosts: localhost

>  become: true

>  vars:

>    git_csa_repo_url: https://gitlab.se.ifmo.ru/Ivan_Ostapenko/csa-rolling.git  <-- помнять ссылку на https://gitlab.se.ifmo.ru/computer-systems/csa-rolling.git

>    git_fp_repo_url: https://gitlab.se.ifmo.ru/Ivan_Ostapenko/main.git  <-- помнять ссылку на https://gitlab.se.ifmo.ru/functional-programming/main.git

>    git_se_am_repo_url: https://gitlab.se.ifmo.ru/Ivan_Ostapenko/architectural-modeling.git  <-- помнять ссылку на https://gitlab.se.ifmo.ru/system-enginering/architectural-modeling.git

>    git_bot_repo_url: https://github.com/ryukzak/course-bot.git

#### Запуск ansible-playbook: 

 `ansible-playbook ansible.yml`

