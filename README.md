# Zabbix-alerts-in-Yandex-Messenger
Данный скрипт позволяет получать оповещения о проблемах из Zabbix в Яндекс Мессенджере 


Для работы вам понадобиться:
1. Развернутый Zabbix
2. API ключ Яндекс Бота
3. id групового чата:
    - можно получить открыв в браузере созданный групповой чат Яндекс.Месенджера
    - Взять часть URL c конца заменив символы 0%2F0%2F на 0/0/
    - https://yandex.ru/chat#/chats/0%2F0%2FXXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    - Итоговый id группы  0/0/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX

Старт

1. Войдите в заббиск и создайте новую систему оповещения
2. Добавьте переменные
   
   ![image](https://github.com/user-attachments/assets/dc8fa3d4-3dd4-4eb4-9ae9-736e2aa9b6e3)

   Message  =  {ALERT.MESSAGE}

   Subject  =  {ALERT.SUBJECT}

   To       =  {ALERT.SENDTO}

   Token    =  ваш токен бота 

   URL      =  адрес отправки сообщений https://botapi.messenger.yandex.net/bot/v1/messages/sendText/

3. В строку скрипт впишите скрипт лежащий в файле main.js. 

4. Настройте оповещения на каком либо оповещательном пользователе
   
   ![image](https://github.com/user-attachments/assets/dcb46e06-a6e2-4891-9a33-7518ed03e892)
   
В отправть на, требуется написать id чата куда слать сообщения

На этом все) 
