# Помошник по Git

[Скачть Git](https://git-scm.com/download/win)
Запускать Git Bash

## Команлы Git Bash

- **mkdir**  создать директорию
- **mkdir -p dir1/dir-inside/dir-deeper-inside** создать структуру директорий
- **cd ~**  перейти в свою домашнюю директорию
- с помощью **Tab** bash подставит окончание
- **pwd** данные о текущем каталоге
= **ls** просмотр содержимого каталога
- **ls -a** расширенный просмотр, со скрытыми файлама
- **touch имя_файла** создать текстовый файла
- **cp что_копируем что_копируем что_копируем куда_копируем** копирование файла
- **mv table.csv ./very-important-files** переместить файл 
- **cat myfile.txt** чтение файла
- **rm example.txt** удаление файла
- **rmdir images** удаление директории
- **rm -r images** удаление директории со всем содержимым
- ** mkdir second-project && cd second-project && touch index.html style.css** выполнение нескольких команд. Записыааются через **&&**
- На Windows (в Git Bash) и Linux для этого используется сочетание Ctrl+Shift+V

## Git и команды

- **git init** сделать папку репозиторием
- **rm -rf .git** удалить .git, перестать считать папку репозиторием
- **git config use.name "Имя"** имя для конфига
- **git config use.email "adress@emial.com"** email для конфига
- **git.status** статус git: состояние репозитория
- **git add --all** добавить все измененные файлы
- **git add имя_файла** добавить файл 
- **git commit -m"текст коммита"** закомиттить изменения Если ввести git commit без флага -m, откроется редактор Vim. Чтобы выйти из него, нажмите клавишу Esc, наберите последовательность символов :q! и нажмите Enter.
- **git push** отправить изменения в git-hub
- **git log** история коммитов

## Работа с Git-Hub

### SSH

Проверить наличие ключей SSH
- **ls -la .ssh/** проперять надо в домашней директории
- **ssh-keygen -t ed25519 -C "электронная почта, к которой привязан ваш аккаунт на GitHub"** создать ключи с алгоритмом ed25519
- **ssh-keygen -t rsa -b 4096 -C "электронная почта, к которой привязан ваш аккаунт на GitHub"** создать кдючи с алгоритмом rsa
- **clip < ~/.ssh/id_rsa.pub** скопировать ключ
- Перейдите на GitHub и выберите пункт Settings (англ. «настройки») в меню аккаунта.
- В меню слева нажмите на пункт SSH and GPG keys.
- В открывшейся вкладке выберите New SSH key (англ. «новый SSH-ключ»).
- **ssh -T git@github.com** проверить ключ

### Работа с удаленным репозиторием

- **git remote add origin git@github.com:%ИМЯ_АККАУНТА%/first-project.git** свзять локальный с Git Hub origin - имя. Нужно создать репозиторий на git-hub и взять там ссылку
- **git remote -v** проверить связь
- **git clone https://github.com/yandex-praktikum/git-clone-lesson** клонирование к себе
- fork позволяет скопировать к себе без связи с оригинальным проектом 


