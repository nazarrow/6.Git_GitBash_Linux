# JSON + Git

*Задание 1. Создать внешний репозиторий c названием JSON.*

`Решение`⮯

1. Перейти по [ссылке](https://github.com/nazarrow?tab=repositories)
2. Нажать "New"
3. Ввести "JSON" в поле "Repository name" 
4. Выбрать "Public" и "Add a README file"
5. Нажать "Create repository"
---

*Задание 2. Клонировать репозиторий JSON на локальный компьютер.*

`Решение`⮯

1. Нажать "Code"
2. Выбрать "HTTPS"
3. Нажать "Скопировать ссылку на репозиторийЭ
4. В GitBash зайти в папку (в которой будет размещен репозиторий)
5. Клонировать репозиторий на локальный компьютер:

```bash
git clone <https://github.com/nazarrow/JSON.git>
```

6. Войти в папку "Json folder":

```bash
cd Json folder
```
---

*Задание 3. Внутри локального "JSON" (папки "Json folder") создать файл “new.json”.*

`Решение`⮯

1. Создать файл:

```bash
touch new.json
```

2. Посмотреть состояние файлов в рабочем каталоге и индексе:

```bash
git status
``` 
---

*Задание 4. Добавить файл под гит.*

`Решение`⮯

1. Добавить содержимое рабочего каталога в индекс (staging area) для последующего коммита:

```bash
git add new.json
```
2. Посмотреть состояние файлов в рабочем каталоге и индексе:

```bash
git status
``` 
---

*Задание 5. Закоммитить файл.*

`Решение`⮯

1. Сделать снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов:

```bash
git commit -m "add new.json"
``` 
---

*Задание 6. Отправить файл на внешний GitHub репозиторий.*

`Решение`⮯

1. Выгрузить содержимое локального репозитория в удаленный:

```bash
git push
```
---

*Задание 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.*

`Решение`⮯

1. Открыть текстовый редактор Vim:

```bash
vim new.json
```

2. Нажать " i "
3. Ввести информацию:

```json
{
 "full_name":"Nazarov_Aleksei_Olegovich",
 "age":29,
 "pets":"I don`t have any pets",
 "desired_salary":"1000$"
}
```

4. Нажать "Esc"
5. Нажать ":wq"
---

*Задание 8. Отправить изменения на внешний репозиторий.*

`Решение`⮯

```bash
git add new.json

git commit -m "modified new.json"

git push
```
---

*Задание 9. Создать файл preferences.json.*

`Решение`⮯

```bash
cat > preferences.json
```
---

*Задание 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм,сериал, еда, время года, страна которую хотели бы посетить) в формате JSON.*

`Решение`⮯

1. Ввести информацию:
   
```json
{
 "favorite_movie":"The Social Network",
 "favorite_series":"Silicon Valley",
 "favorite_food":"Meat",
 "favorite_season":"Summer",
 "country_i_would_like_to_visit":"Switzerland"
}
```

2. Нажать "Enter"
3. Нажать "Ctrl + D"
---

*Задание 11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON.*

`Решение`⮯

1. Ввести:

```bash
cat > skills.json
```

2. Ввести информацию:

```json
{
"skills":[
 "software testing theory",
 "client-server architecture",
 "HTTP Server Request Methods",
 "HTTP server Response codes",
 "Structures of HTTP requests and responses",
 "What is JSON, XML. Their structure",
 "API testing via Postman JS, API autotests",
 "Removing and reading logs from an external server",
 "Sniffing http web traffic through Charles and Fiddler",
 "Dev Tools of web browsers Google Chrome, FireFox",
 "VPN. How it works, why you need it, how to use it, tool options",
 "Mobile testing",
 "Feature of iOS, Android, guidelines",
 "Build iOS applications on Xcode",
 "Build Android applications on Android Studio",
 "ADB management of android devices",
 "Setting up proxy and vpn on iOS and Android",
 "Interception (sniffing) of mobile traffic through Charles and Fiddler on iOS and Android",
 "Command line (terminal) Linux copy, create, view, move files on servers without a graphical interface",
 "Basics of bash scripting, automation of routine tasks on the server",
 "Access to remote servers",
 "Basics of SQL Create, Delete, Drop, Insert Into, Select, From, Where, Join",
 "Postgres database installation, configuration and use",
 "Non-relational database Redis installation, configuration and use",
 "Load testing in Jmeter",
 "Scrum development methodology",
 "Python. Learning the basics. Building a client-server application"
 ]
}
```

3. Нажать "Enter"
4. Нажать "Ctrl + D"
---

*Задание 12. Отправить сразу 2 файла на внешний репозиторий.*

`Решение`⮯

```bash
git add .

git commit -m "add preferences.json and skills.json"

git push
```
---

*Задание 13. На веб интерфейсе создать файл bug_report.json.*

`Решение`⮯

1. Зайти в репозиторий "JSON"(папка Json folder)
2. Нажать кнопку "Add file"
3. Нажать кнопку "Create new file"
4. В поле "Name your file" ввести "bug_report.json"
---

*Задание 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.*

`Решение`⮯

1. Нажать кнопку "Commit new file"
---

*Задание 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.*

`Решение`⮯

1. Открыть файл "bug_report.json"
2. Нажать кнопку "Редактировать" 
3. Ввести информацию:

```json
{
"bugReport":[
   {
   "summary": "Information dosn't provide if have more than 7 characters from WS",
   "descriprion": "WS dosen't provide information if response containes more than 8 characters",
   "actualResult": "information gets",
   "expectedResult": "information doesen't get",
   "requirementId": "requirement",
   "reproducedOn": "Win 10",
   "reproducibility": "always",
   "workaround": "no",
   "stepsTOreproduce":[
        {"one": "1. Open FireFox browser",
        "two": "2. Click [RESTClient] icon",
        "three": "3. Request method: POST",
        "four": "4. URL: <http://178.124.206.52/app/ws/>",
        "five": "5. type in Body: {user:rangarad, strict:false}"
                                }
                                ],
   "severity": "minor",
   "priority": "low"
   }  
   ]
}
```
---

*Задание 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.*

`Решение`⮯

1. Нажать кнопку "Commit changes"
---

*Задание 17. Синхронизировать внешний и локальный репозиторий JSON.*

`Решение`⮯

```bash
git pull
```
