# Тестовое задание

Используемый дистрибутив Ubuntu 22.04
Для теста используется vagrant.

Для запуска необходимо выполнить:
1. Установить vagrant
2. Запустить vagrant в директории ./vagrant командой vagrant up
3. Получить адрес приватного ключа для доступа к VM командой vagrant ssh-config | grep IdentityFile
4. Прописать адрес ключа в файле ./ansible/ansible.cfg ключ  private_key_file =
5. Запустить playbook из директории ./ansible командой ansible-playbook  playbook.yml
6. Проверить результат выполнив команду curl localhost:8080
7. По завершению теста удаляем тестовую машину, выполнив команду vagrant destroy -f в каталоге ./vagrant