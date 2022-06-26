# <p align="justify"> Это тестовый репозиторий, выполненный в рамках учебного курса Вадима Ксендзова по тестированию программного обеспечения. Здесь мои  первые шаги по изучению Git и GitHub. Ниже, собственно, одна из "домашек" и мой вариант ее решения. С целью закрепления изученного материала и практических навыков, инструментарием служили: Visual Studio Code; Git Bash; Markdown.</p>

## __1. Создать внешний репозиторий c названием json:__

 [Ссылка на репозиторий](https://github.com/gadaborshev/gr29_github_json.git)

## __2. Клонировать репозиторий json на локальный компьютер:__

```  
$ git clone git@github.com:gadaborshev/gr29_github_json.git
Cloning into 'gr29_github_json'...
The authenticity of host 'github.com (140.82.121.3)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? y
Please type 'yes', 'no' or the fingerprint: yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
Enter passphrase for key '/c/Users/director/.ssh/id_rsa':
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done. 
```

## __3. Внутри локального json создать файл “new.json”:__
```
 touch new.json
```  

## __4. Добавить файл под гит:__
 ```
 $ git add new.json
 warning: LF will be replaced by CRLF in new.json.
 The file will have its original line endings in your working directory
```
## __5. Закоммитить файл:__
```
 $ git commit -m "created file new.json"
 [main 9b70499] created file new.json
 1 file changed, 8 insertions(+)
 create mode 100644 new.json
```
## __6. Отправить файл на внешний GitHub репозиторий:__
```
 $ git push
 Enter passphrase for key '/c/Users/director/.ssh/id_rsa':
 Enumerating objects: 4, done.
 Counting objects: 100% (4/4), done.
 Delta compression using up to 12 threads
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (3/3), 419 bytes | 419.00 KiB/s, done.
 Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 To github.com:gadaborshev/gr29_github_json.git
 922fa85..9b70499  main -> main
```
## __7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате json:__
```
 vim new.json 
{
 "Identity":"Gadaborshev Ruslan Tarkhanovich",
 "Age":"41",
 "Pets":"I don't have pets, but I have three children :-)",
 "Desired Salary":"Let's start with $1000"
}
```

## __8. Отправить изменения на внешний репозиторий:__
```
 $ git add new.json
 warning: LF will be replaced by CRLF in new.json.
 The file will have its original line endings in your working directory
 
 $ git commit -m "added some info about me"
 [main 67b5d6c] added some info about me
 1 file changed, 1 insertion(+), 1 deletion(-)
 
 $ git push
 Enter passphrase for key '/c/Users/director/.ssh/id_rsa':
 Enumerating objects: 5, done.
 Counting objects: 100% (5/5), done.
 Delta compression using up to 12 threads
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (3/3), 325 bytes | 325.00 KiB/s, done.
 Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
 remote: Resolving deltas: 100% (1/1), completed with 1 local object.
 To github.com:gadaborshev/gr29_github_json.git
    9b70499..67b5d6c  main -> main
```

## __9. Создать файл preferences.json:__

```
 vim preferences.json
```

## __10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате json:__
```
{
 "Favorite movie":"There are a lot of them",
 "Favorite series":"Silicon Valley",
 "Favorite food":"Seafood",
 "Country I would like to visit":"USA"
} 
```
## __11. Создать файл sklls.json добавить информацию о скиллах, которые будут изучены на курсе в формате json:__
```
 vim sklls.json
{
 "Skill":"Basic theory (What is testing, bug reports, documentation, types, methods, areas of testing, etc.) SDLC, STLC",
 "Skill":"What is a client-server architecture",
 "Skill":"HTTP Methods of requests to the server",
 "Skill":"HTTP server response codes",
 "Skill":"Structures of HTTP requests and responses",
 "Skill":"What is JSON, XML. Their structure",
 "Skill":"API testing via Postman (JS, API autotests)",
 "Skill":"Removing and reading logs from an external server",
 "Skill":"Sniffing http web traffic via Charles and Fiddler",
 "Skill":"Dev Tools of web browsers (Google Chrome, FireFox)",
 "Skill":"VPN. (How it works, why you need it, how to use it, tool options)",
 "Skill":"Mobile testing",
 "Skill":"Feature iOS, Android, guidelines",
 "Skill":"Building iOS applications on XCode. (Those who do not have a Mac computer, just look)",
 "Skill":"Building Android applications on Android Studio",
 "Skill":"ADB (android device management)",
 "Skill":"Setting up proxy and vpn on iOS and Android",
 "Skill":"Interception (sniffing) of mobile traffic via Charles and Fiddler on iOS and Android",
 "Skill":"Command line (terminal) Linux (copying, creating, viewing, moving files on servers without a graphical interface)",
 "Skill":"Basics of bash scripting, automation of routine tasks on the server",
 "Skill":"Access to remote servers",
 "Skill":"SQL basics (Create, Delete, Drop, Insert Into, Select, From, Where, Join)",
 "Skill":"Postgres database (installation, configuration and use)",
 "Skill":"Non-relational database Redis (installation, configuration and use)",
 "Skill":"Load testing in Jmeter",
 "Skill":"Scrum development methodology",
 "Skill":"Python. (Learning the basics. Creating a client-server application)"
 } 
```

## __12. Отправить сразу 2 файла на внешний репозиторий:__
```
 $ git add .
 warning: LF will be replaced by CRLF in preferences.json.
 The file will have its original line endings in your working directory
 warning: LF will be replaced by CRLF in skills.json.
 The file will have its original line endings in your working directory
 
 $ git commit -am "added some new info about me"
 [main bf3ef72] added some new info about me
 2 files changed, 35 insertions(+)
 create mode 100644 preferences.json
 create mode 100644 skills.json

 $ git push
 Enter passphrase for key '/c/Users/director/.ssh/id_rsa':
 Enumerating objects: 5, done.
 Counting objects: 100% (5/5), done.
 Delta compression using up to 12 threads
 Compressing objects: 100% (4/4), done.
 Writing objects: 100% (4/4), 1.24 KiB | 1.24 MiB/s, done.
 Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
 To github.com:gadaborshev/gr29_github_json.git
 67b5d6c..bf3ef72  main -> main
```
## __13. На веб интерфейсе создать файл bug_report.json:__

[Ссылка](https://github.com/gadaborshev/gr29_github_json/blob/main/bug_report.json)

## __14. Сделать Commit changes (сохранить) изменения на веб интерфейсе:__

[Скриншот_1](https://github.com/gadaborshev/gr29_github_json/blob/main/screenshot_1.png)
 
## __15.На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате json, сделать Commit changes (сохранить) изменения на веб интерфейсе :__

[Скриншот_2](https://github.com/gadaborshev/gr29_github_json/blob/main/screenshot_2.png)

## __16. Синхронизировать внешний и локальный репозиторий json:__
```
 $ git fetch
 Enter passphrase for key '/c/Users/director/.ssh/id_rsa':
 remote: Enumerating objects: 7, done.
 remote: Counting objects: 100% (7/7), done.
 remote: Compressing objects: 100% (5/5), done.
 remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
 Unpacking objects: 100% (6/6), 1.46 KiB | 4.00 KiB/s, done.
 From github.com:gadaborshev/gr29_github_json
 bf3ef72..857d158  main       -> origin/main


 $ git pull
 Enter passphrase for key '/c/Users/director/.ssh/id_rsa':
 Updating bf3ef72..857d158
 Fast-forward
 bug_report.json | 7 +++++++
 1 file changed, 7 insertions(+)
 create mode 100644 bug_report.json
```