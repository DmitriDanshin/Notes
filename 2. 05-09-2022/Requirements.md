## Использование requirements.txt

Если потребуется масштабировать вашу программу, перенести её на другой сервер или развернуть проект из GitHub, не устанавливая каждый пакет PIP, который требуется для запуска, отдельно — всё это можно реализовать с помощью встроенного функционала. Все пакеты можно сохранить в файл `requirements.txt` (такое название необязательно, но является общепринятым стандартом), а затем развернуть их на сервере или в виртуальном окружении VENV. 

Чтобы сохранить информацию о всех установленных пакетах PIP, используем команду:

```
pip3 freeze > requirements.txt
```

Для установки пакетов, которые были сохранены в файл, команда следующая:

```
pip install -r requirements.txt
```