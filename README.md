# VPN-приложение

Простой VPN-шелл между двумя устройствами

Для функционирования необходимо на обоих устройствах иметь файл с 16-байтовым ключом.
При подключении устройства согласуют 16-байтовый сессионный ключ алгоритмом EKE, после этого передают друг другу сообщения, зашифрованные AES-CBC.

## Запуск сервера
`python3 main.py -l -p <port> -f <secret file>`

## Запуск клиента
`python3 main.py <host> <port> -f <secret file>`