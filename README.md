# Russian
# English
# Демонстрационный телеграм-бот для нужд транспортной компании
#### Цель проекта
Реализация простейшего телеграм-бота на языке программирование **python** с использованием библиотеки **pyTelegramBotAPI**
#### Цель программы
Информировать клиента вымышленной транспортной компании Che-logistic о месте нахождения отправления (посылки) клиента в конкретный момент времени.
## Как начать
1. Скачать и установить [python](https://www.python.org/downloads/) версии 3.9.7;
2. Установить библиотеку [pandas](https://pypi.org/project/pandas/);
3. Установить библиотеку [pyTelegramBotAPI](https://pypi.org/project/pyTelegramBotAPI/) (тестирование проводилось на версии 3.8.2);
4. Установить библиотеку [telebot](https://pypi.org/project/telebot/) (тестирование проводилось на версии 0.0.4);
5. Создать телеграм-бота с помощью [BotFather](https://telegram.im/BotFather) и получить API-key;
6. Скачать с репозитория файлы *Che_inform.py* и *base_cargo.csv* (проверить в скрипте *Che_inform.py* правильность пути к файлу *base_cargo.csv*, путь указан в переменной *BASE_FILE_NAME*);
7. Создать файл с именем *auth_info.txt* (или указать свое имя файла и путь в скрипте *Che_inform.py* в переменной *AUTH_FILE_NAME*) и записать в него полученный API-key (использовать кодировку файла UTF-8);
8. Запустить на исполнение файл *Che_inform.py*.
## О проекте
Данный проект был разработан как демонстрационное пособие по созданию телеграм-бота для нужд Компьютерной Академии ШАГ. Бот информирует любого спросившего о месте нахождения отправления (посылки) с определенным номером. Данные об отправлениях находятся в файле *base_cargo.csv*. Номера отправлений сгенерированы автоматически и имеют ключ (4-я цифра номера). 

Задача бота:
- получить номер отправления от пользователя;
- проверить с помощью регулярного выражения, что пользователь отправил именно цифры;
- проверить значение ключа номера отправления с контрольной суммой;
- проверить наличие номера отправления в базе;
- по результатам проверки вернуть пользователю сообщение об ошибке или место нахождение отправления.
