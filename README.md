В корневой папке проекта выполнить следующие команды
1.	$ git init - инициализация(создание) репозитория
2.	Создаем .gitignore - прописывая в него файлы и папки, которые не должны попасть в репозиторий.
3.	Минимальные настройки git’а: 
$ git config --global user.name "username"
$ git config --global user.email "you@mail.ru"
4.	$ git add . - добавляем все файлы проекта(кроме тех, что в .gitignore). Подготавливаем файлы к коммиту(сохранению)
5.	$ git commit -m “комментарий к коммиту”  - делаем коммит(сохраняем текущее состояние файлов в репозитории)
Каждый раз, когда вам нужно сохранить изменения в локальном репозитории выполните:
$ git add .
$ git commit -m “комментарий к коммиту” 

При создании репозитория из командной строки делаем так:
echo "# Docker" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin git@github.com:kvepyt/Docker.git
git push -u origin master

При наличии существующего репозитория - так:
git remote add origin git@github.com:kvepyt/Docker.git
git branch -M master
git push -u origin master
