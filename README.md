# Лабораторная работа №6
### Цель лабораторной работы
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием. 
### Ход работы
1) Создал аккаунт на GitHub ([рис. 1](https://github.com/dalucker/LR6/blob/new_branch/Photo/1.png)).
2)	Сделал копию (fork) в личное хранилище из [репозитория](https://github.com/Kurtyanik/LR6/) ([рис. 2](https://github.com/dalucker/LR6/blob/new_branch/Photo/2.png)).
3)	Установил Git.
4)	После установки настроил клиент git, введя имя пользователя (4217 Makarov N.S.) и email ([рис. 3](https://github.com/dalucker/LR6/blob/new_branch/Photo/3.png)).
```sh
git config --global user.email "agiosnikita@gmail.com"
git config --global user.name "4217 Makarov N.S."

```
5)	Клонировал свой личный удалённый репозиторий на компьютер ([рис. 4](https://github.com/dalucker/LR6/blob/new_branch/Photo/4.png)).
```sh
git clone https://github.com/dalucker/LR6
```
6)	Добавил файл `text.txt` через интерфейс GitHub. Подтянул изменения в локальный репозиторий ([рис. 5](https://github.com/dalucker/LR6/blob/new_branch/Photo/5.png)).
```sh
git pull
```
7) Получил историю операций для ветки `master` ([рис. 6](https://github.com/dalucker/LR6/blob/new_branch/Photo/6.png)) и `branch1` ([рис. 7](https://github.com/dalucker/LR6/blob/new_branch/Photo/7.png)).
```sh
git log
git log origin/branch1
```
8)  Посмотрел последние изменения ([рис. 8](https://github.com/dalucker/LR6/blob/new_branch/Photo/8.png)).
```sh
git branch -v
```
9) Выполнил слияние в ветку `master`, разрешив конфликт ([рис. 9](https://github.com/dalucker/LR6/blob/new_branch/Photo/9.png), [рис. 10](https://github.com/dalucker/LR6/blob/new_branch/Photo/10.png)).
```sh
git merge origin/branch1
```
10) Удалил побочную ветку после успешного слияния ([рис. 11](https://github.com/dalucker/LR6/blob/new_branch/Photo/11.png)).
```sh
git branch -d branch1
```
11) Сделал изменения и зафиксировал их, оставляя комментарии несколько раз ([рис. 12](https://github.com/dalucker/LR6/blob/new_branch/Photo/12.png)).
```sh
git add .
git status
git commit -m "comment"
```
12) Сделал откат коммита ([рис. 13](https://github.com/dalucker/LR6/blob/new_branch/Photo/13.png))
```sh
git reset --haard HEAD~
```
13) Создал ветку для отчета ([рис. 14](https://github.com/dalucker/LR6/blob/new_branch/Photo/14.png)).
```sh
git branch new_branch
```
14) Оформил отчет в файле `README.md`
15) Получил историю операций в форматированном виде ([рис. 15]()).
```sh
git log --pretty=format:'%h - %cd - %an - %s' --date=format:'%F %R'
```
### Вывод
Изучил базовые возможности системы управления версиями, получил опыт работы с Git Api, опыт работы с локальным и удаленным репозиториями. 
