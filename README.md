# Настройка клиента WireGuard, подключение SSH, создание пользователей и базовая работа с директориями/файлами в Linux
## Wire Guard
WireGuard можно назвать VPN подключением. Для создания самого простого клиентского конфига, нужно прописать всего пять параметров:

[Inteface]
+ PrivateKey = (генерируется при создании пустого тунеля)
+ Address = (IP адрес в тунеле)

[Peer]
- PublickKey = (публичный ключ, который использует сервер)
- AllowedIps = (разрешённые IP сети)
- Endpoint = (внешний IP адрес сервера)

После создания конфига в строке Publick key: генерируется ключ, который нужен серваку
## SSH
SSH - это шифрованное подключение к компам.

Команда: ***ssh -p (порт) (пользователь)@(адрес_компьютера)***

После этого у вас запросят пароль от пользователя
## Создание пользователей
Для создания пользователей в Linux используется команда adduser.
Синтаксис: ***adduser -d (директория) (имя пользователя)***

После он спросит несколько параметров, в том числе пароль.
ssh [имя пользователя]@[адрес]
[пароль]

adduser [имя пользователя]
[пароль]
[еще раз пароль]

mkdir [путь к дериктории в которой вы хотите создать саму директорию]

touch [путь к директории, в которой создается файл]

ls [кооманда для просмотра содержимого дериктории]
