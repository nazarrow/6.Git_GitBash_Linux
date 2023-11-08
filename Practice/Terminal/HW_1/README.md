# HW_1 Linux terminal (GitBash) commands

*Задание 1. Посмотреть где я.*  

`Решение`⮯
   + `pwd`
   
*Задание 2. Создать папку.*

`Решение`⮯
   + `mkdir folder`
 
*Задание 3. Зайти в папку.*

`Решение`⮯
   + `cd folder`
   
*Задание 4. Создать 3 папки.*

`Решение`⮯
   + `mkdir folder1 folder2 folder3`

   + `mkdir folder{1..3}`
  
*Задание 5. Зайти в любоую папку.*

`Решение`⮯
   + `cd folder1`
  
*Задание 6. Создать 5 файлов (3 txt, 2 json).*

`Решение`⮯
   + `touch file1.txt file2.txt file3.txt file1.json file2.json`
  
   + `touch file{1..3}.txt file{1..2}.json`
  
*Задание 7. Создать 3 папки.*

`Решение`⮯
   + `mkdir folder_1 folder_2 folder_3`

   + `mkdir folder{1..3}`
  
*Задание 8. Вывести список содержимого папки.*

`Решение`⮯
   + `ls -la` (вывод всех данных, в т.ч. скрытых)

*Задание 9. Открыть любой txt файл(для редактирования).*

`Решение`⮯
   + `vim file1.txt`

*Задание 10. Написать туда что-нибудь, любой текст.*

`Решение`⮯
   + нажать `"i"` (режим редактирования)

   + `ввести текст`

   + нажать `"esc"`
  
*Задание 11. Сохранить и выйти.*

`Решение`⮯
   + `:wq`
  
*Задание 12. Выйти из папки на уровень выше.*

`Решение`⮯
   + `cd ..`

   + `cd ../..` (выйти на 2 уровня выше)
  
*Задание 13. Переместить любые 2 файла, которые вы создали, в любую другую папку.*

`Решение`⮯
   + `mv folder1/{file2.txt,file1.json} folder1/folder_1`
    
*Задание 14. Скопировать любые 2 файла, которые вы создали, в любую другую папку.*

`Решение`⮯
   + `cp folder1/{file3.txt,file2.json} folder1/folder_2`
  
*Задание 15. Найти файл по имени.*

`Решение`⮯
   + `find . -name "file1*"`
  
*Задание 16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает.*

`Решение`⮯
   + `tail -f file1.txt | grep pattern` (редактируем, сохраняем и смотрим в текстовом редакторе)

   + `tail -f file1.txt | grep --line-buffered pattern >> 1_log.txt | tail -f 1_log.txt` (запись в файл с отображением в терминале)

*Задание 17. Вывести несколько первых строк из текстового файла.*

`Решение`⮯
   + `head -3 file1.txt`

*Задание 18. Вывести несколько последних строк из текстового файла.*

`Решение`⮯
   + `tail -3 file1.txt`
  
*Задание 19. Просмотреть содержимое длинного файла (команда less) изучите как она работает.*

`Решение`⮯
   + `less file1.txt`

   + нажать `"q"`

*Задание 20. Вывести дату и время.*

`Решение`⮯
   + `date`

## 🔖 Дополнительные задания ∗ 🤔

*Задание 1. Отправить http запрос на сервер. `<http://162.55.220.72:5005/terminal-hw-request>`.*

`Решение`⮯
   + `curl <http://162.55.220.72:5005/terminal-hw-request>`

Ответ:

```json
  {"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: `<http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number>)","result":["Your_String","Your_number"]`}} 
```

выполняем Task1:

   + `curl "<http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number>)"`

   + `(set_your_String) --> "Aleksei", (set_your_number) --> 29`
  
Ответ:

   + `["Aleksei","29"]`

*Задание 2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13.*

`Решение`⮯
   + `cat > script.sh`

   + `vim script.sh`
  
   + нажать `"i"`

```bash
# !/bin/bash

pwd

mkdir folder_script

cd folder_script

mkdir folder1 folder2 folder3

cd folder3

touch {f1.txt,f2.txt,f3.txt,f4.json,f5.json}

mkdir script_folder1 script_folder2 script_folder3

ls -la

mv f1.txt f4.json script_folder2

./script.sh
```
