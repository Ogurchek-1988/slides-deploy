task: https://gitlab.se.ifmo.ru/computer-systems/csa-rolling/-/issues/15

При необходимости могу переделать работу с гитом на ssh


Настройка системы для выполнения данного задания:


Дистрибутив: ubuntu server 20.04

Сгенерировать ssh ключи: ssh-keygen

Установить сертификаты: sudo apt-get install ca-certificates

Установить pip: sudo apt -y install python3-pip

Установка ansible: sudo apt install ansible

Установка docker:
sudo apt install docker.io 
sudo pip install docker
sudo pip install docker-compose
sudo gpasswd -a $USER docker


Запуск ansible-playbook: ansible-playbook ansible.yml

