# Отчёт по лабораторной работе
## «Система контроля версий Git и GitHub»

**Выполнил:** Вдовин Родион Максимович, группа 1ИТ9.25  
**Дата:** 03.11.2026  

---

## 1. Цель работы
Освоить базовые команды Git и научиться публиковать веб-проекты на GitHub.

## 2. Ход выполнения

### Задание 1. Настройка Git
Выполнены команды:
```bash
git config --global user.name "ayowhites"
git config --global user.email "vdovinrm25@kem.ithub.ru"

### Задание 2. Создание лок.репозитория и README
Выполнены команды:
```bash
cd Desktop/git-lab-vdovin
git init
echo > README.md
echo > index.html
echo > script.js
echo > style.css
git status
git add .
git commit -m Первый коммит: добавлены README, index.html, style.css, script.js"
git log --oneline

### Задание 3. Коммиты и .gitignore
Выполнены команды:
```bash
git diff
git add .
git commit -m "Добавлена новая секция на страницу"
echo > .gitignore
git status
git add .gitignore
git commit -m "Добавлен .gitignore для веб-проекта"
Отредактировано:
index.html
.gitignore

### Задание 4. Ветки
Выполнены команды:
git checkout -b feature.
Изменено index.html
git add .
git commit -m "Изменения в ветке feature"
git checkout main
git branch -d feature
git log --oneline --graph
git merge feature

### Задание 5. Пулл на GitHub
Создан аккаунт GitHub

Выполнены команды:
```bash
git remote add origin https://github.com/ayowhites/git-lab-vdovin.git
git branch -M main
git push -u origin main
git remote -v


### Задание 6. pull и report.md
Выполнены команды: 
git pull
Коммит на github
git add REPORT.md screenshots/
git commit -m "Добавлен отчёт REPORT.md со скриншотами
git push
mkdir screenshots
Создана папка screenshots со скриншотами работы


### Задание 7. Оформление
Выполнено:
git tag 1.0
git push --tags
оформлен README и REPORT

## Ответы на вопросы(1-7)
1.git add заносит файл в индексы git а commit сохраняет и комментирует изменения
2.ветка это изолированная линия разработки которая позволяет указывать на определенные коммиты
3.fetch скачивает новые коммиты а pull скачивает и сливает ветки
4.показывает текущее состояние рабочей директории
5.git выдаст ошибку т.к сначала нужно сделать pull для объединения изменений
6.указывает git какие файлы и папки нужно игнорировать и не добавлять в репозиторий
7.merge объединяет ветки но сохраняет ветвистую историю проекта а rebase переписывает коммиты поверх коммитов другой ветки вместе со слиянием истории