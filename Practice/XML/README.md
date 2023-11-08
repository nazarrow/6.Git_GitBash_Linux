# XML + Git

*Задание 1. Создать внешний репозиторий c названием XML.*

`Решение`⮯

1. Перейти по [ссылке](https://github.com/nazarrow?tab=repositories)
2. Нажать "New"
3. Ввести "XML" в поле "Repository name" 
4. Выбрать "Public" и "Add a README file"
5. Нажать "Create repository"
---

*Задание 2. Клонировать репозиторий XML на локальный компьютер.*

`Решение`⮯

1. Нажать "Code"
2. Выбрать "HTTPS"
3. Нажать "Скопировать ссылку на репозиторий"
4. В GitBash зайти в папку (в которой будет размещен репозиторий)
5. Клонировать репозиторий на локальный компьютер:

```bash
git clone <https://github.com/nazarrow/XML.git>
```

6. Войти в папку "Xml folder":

```bash
cd Xml folder
```
---

*Задание 3. Внутри локального "XML" (папки "Xml folder") создать файл “new.xml.*

`Решение`⮯

1. Создать файл:

```bash
touch new.xml
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
git add new.xml
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
git commit -m "add new.xml"
``` 
---

*Задание 6. Отправить файл на внешний GitHub репозиторий.*

`Решение`⮯

1. Выгрузить содержимое локального репозитория в удаленный:

```bash
git push
```
---

*Задание 7. Отредактировать содержание файла “new.xml - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.*

`Решение`⮯

1. Открыть текстовый редактор Vim:

```bash
vim new.xml
```

2. Нажать " i "
3. Ввести информацию:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<aboutMe>
 <fullName>Nazarov Aleksei Olegovich</fullName>
 <age>29</age>
 <pets>I don`t have any pets</pets>
 <desiredSalary>1000$</desiredSalary>
</aboutMe>
```

4. Нажать "Esc"
5. Нажать ":wq"
---

*Задание 8. Отправить изменения на внешний репозиторий.*

`Решение`⮯

```bash
git add new.xml

git commit -m "modified new.xml"

git push
```
---

*Задание 9. Создать файл preferences.xml.*

`Решение`⮯

```bash
cat > preferences.xml
```
---

*Задание 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм,сериал, еда, время года, страна которую хотели бы посетить) в формате XML.*

`Решение`⮯

1. Ввести информацию:
   
```xml
<?xml version="1.0" encoding="UTF-8"?>
<myPreferences>
 <movie>The Social Network</movie>
 <series>Silicon Valley</series>
 <food>Meat</food>
 <season>Summer</season>
 <country>Switzerland</country>
</myPreferences>
```

2. Нажать "Enter"
3. Нажать "Ctrl + D"
---

*Задание 11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML.*

`Решение`⮯

1. Ввести:

```bash
cat > skills.xml
```

2. Ввести информацию:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<skills>
 <one>software testing theory</one>
 <two>client-server architecture</two>
 <three>HTTP Server Request Methods</three>
 <four>HTTP server Response codes</four>
 <five>Structures of HTTP requests and responses</five>
 <six>What is JSON, XML. Their structure</six>
 <seven>API testing via Postman JS, API autotests</seven>
 <eight>Removing and reading logs from an external server</eight>
 <nine>Sniffing http web traffic through Charles and Fiddler</nine>
 <ten>Dev Tools of web browsers Google Chrome, FireFox</ten>
 <eleven>VPN. How it works, why you need it, how to use it, tool options</eleven>
 <twelve>Mobile testing</twelve>
 <thirteen>Feature of iOS, Android, guidelines</thirteen>
 <fourteen>Build iOS applications on Xcode</fourteen>
 <fifteen>Build Android applications on Android Studio</fifteen>
 <sixteen>ADB management of android devices</sixteen>
 <seventeen>Setting up proxy and vpn on iOS and Android</seventeen>
 <eighteen>Interception (sniffing) of mobile traffic through Charles and Fiddler on iOS and Android</eighteen>
 <nineteen>Command line (terminal) Linux copy, create, view, move files on servers without a graphical interface</nineteen>
 <twenty>Basics of bash scripting, automation of routine tasks on the server</twenty>
 <twentyOne>Access to remote servers</twentyOne>
 <twentyTwo>Basics of SQL Create, Delete, Drop, Insert Into, Select, From, Where, Join</twentyTwo>
 <twentyThree>Postgres database installation, configuration and use</twentyThree>
 <twentyFour>Non-relational database Redis installation, configuration and use</twentyFour>
 <twentyFive>Load testing in Jmeter</twentyFive>
 <twentySix>Scrum development methodology</twentySix>
 <twentySeven>Python. Learning the basics. Building a client-server application</twentySeven>
</skills>
```

3. Нажать "Enter"
4. Нажать "Ctrl + D"
---

*Задание 12. Отправить сразу 2 файла на внешний репозиторий.*

`Решение`⮯

```bash
git add .

git commit -m "add preferences.xml and skills.xml"

git push
```
---

*Задание 13. На веб интерфейсе создать файл bug_report.xml.*

`Решение`⮯

1. Зайти в репозиторий "XML"(папка Xml folder)
2. Нажать кнопку "Add file"
3. Нажать кнопку "Create new file"
4. В поле "Name your file" ввести "bug_report.xml"
---

*Задание 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.*

`Решение`⮯

1. Нажать кнопку "Commit new file"
---

*Задание 15. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.*

`Решение`⮯

1. Открыть файл "bug_report.xml"
2. Нажать кнопку "Редактировать" 
3. Ввести информацию:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<bugReport>
   <summary>Information dosn't provide if have more than 7 characters from WS</summary> 
   <descriprion>WS dosen't provide information if response containes more than 8 characters.</descriprion>
   <actualResult>information gets</actualResult>
   <expectedResult>information doesen't get</expectedResult>
   <requirementId>requirement</requirementId>
   <reproducedOn>Win 10</reproducedOn>
   <reproducibility>always</reproducibility>
   <workaround>no</workaround>
   <stepsTOreproduce>
        <one>1. Open FireFox browser</one>
        <two>2. Click [RESTClient] icon</two>
        <three>3. Request method: POST</three>
        <four>4. URL: http://178.124.206.52/app/ws/</four>
        <five>5. type in Body: {"user":"rangarad", "strict":false}</five>
   </stepsTOreproduce>
   <severity>minor</severity>
   <priority>low</priority>
</bugReport>
```
---

*Задание 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.*

`Решение`⮯

1. Нажать кнопку "Commit changes"
---

*Задание 17. Синхронизировать внешний и локальный репозиторий XML.*

`Решение`⮯

```bash
git pull
```
