# GitBash.HW_1

1) Посмотреть где я:
```
pwd
```

2) Создать папку: 
```
mkdir dz
```

3) Зайти в папку: 
```
cd dz
```

4) Создать 3 папки: 
```
mkdir papka1 papka2 papka3
```

5) Зайти в любую папку:
```
cd papka1
```

6) Создать 5 файлов (3 txt, 2 json):
```
touch 1.txt 2.txt 3.txt 4.json 5.json
```

7) Создать 3 папки: 
```
mkdir p1 p2 p3
```

8) Вывести список содержимого папки: 
```
ls -la
```

9) Открыть любой txt файл: 
```
cat 1.txt
```

10) Написать туда что-нибудь, любой текст: 
```
cat >> 1.txt
qqqqqq
aaaaaa
zzzzzzzzwwwww
sssssss
xxxxxxxxx
```

11) Cохранить и выйти:
```
Esc
:wq 
Enter
```

12) Выйти из папки на уровень выше: 
```
cd ..
```

13) Переместить любые 2 файла, которые вы создали, в любую другую папку: 
```
mv papka1/1.txt papka1/2.txt papka2
```

14) Cкопировать любые 2 файла, которые вы создали, в любую другую папку: 
```
cp papka1/4.json papka1/5.json papka3
```

15) Найти файл по имени: 
```
find papka1/3.txt
```

16) Просмотреть содержимое в реальном времени:
```
tail -f  papka2/1.txt
```

17) Вывести несколько первых строк из текстового файла: 
```
head -2 papka2/1.txt
```

18) Вывести несколько последних строк из текстового файла:
```
tail -3 papka2/1.txt
```

19) Просмотреть содержимое длинного файла (команда `less`), изучите как она работает: 
```
less papka2/1.txt
```

20) Вывести дату и время:
```
date
```

## *
1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request 
```
curl http://162.55.220.72:5005/terminal-hw-request
```

Получен ответ:
```
{"Intro":"Hello!! This is your the first response from server",
"Tasks":{"Task_1":"Send the next URL in terminal: 
http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}

# Отправить повторный запрос
curl "http://162.55.220.72:5005/get_method?name=(Sultan)&age=(30)"
```

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13:
```
# Создать файл
touch script.sh

# Внести изменения в файл
cat >> script.sh
#!/bin/bash
cd dz
mkdir papka1 papka2 papka3
cd papka1
touch 1.txt 2.txt 3.txt 4.json 5.json
mkdir p1 p2 p3
ls -la
cd ..
mv papka1/1.txt papka1/2.txt papka2

# Запустить скрипт
sh script.sh
```
