# Создай свой первый вебсайт за 2 часа

## Записи вебинаров
- [Обираємо ІТ спеціальність](https://www.youtube.com/watch?v=Jy8vUkQavk0&feature=youtu.be&list=PL7FuXFaDeEX0ovUeVROcfrren_M1z5LgY&t=205)
- [Frontend чи Backend? Що це? І яка взагалі різниця?](https://www.youtube.com/watch?v=GvL9Cj7VCM8&list=PL7FuXFaDeEX0ovUeVROcfrren_M1z5LgY&index=2)
- [Створи першу веб-сторінку за 2 години повністю з нуля](https://www.youtube.com/watch?v=725Xg0rw-ZI&feature=youtu.be&list=PL7FuXFaDeEX0bTyQhptYAD1lt01nI7UYt&t=1183)
- [Front end розробник. Покроковий план освоєння професії](https://youtu.be/aY5y0tc2ObU)

## Устанавливаем программы
1. Скачай и установи [Google Chrome](https://www.google.com/chrome/) если у тебя его ещё нет
1. Скачай и установи [VSCode](https://code.visualstudio.com/)
    ![vscode-setup](img/vscode-setup.png)

1. Скачай и установи [GIT](https://git-scm.com/)
    ![git-setup-1](img/git-setup-1.png)
    
    ![git-setup-2](img/git-setup-2.png)
    
## Настраиваем GIT
1. Создай пустую директорию `my-first-page` и открой её в проводнике
1. Нажми правой клавишей и выбери `Git Bash Here`
1. Набери в терминале `git config --global user.name "Your Name"`
    - Напиши своё имя, а не `Your Name` :-)
    - Не забудь нажать `Enter`
1. Запусти в терминале `git config --global user.email "Your@Email"`
    - тут твоя почта, а не `Your@Email`

## Создаём сайт 
1. В терминале запусти команду `code .` - после неё откроется VSCode
1. Создай новый файл с названием `index.html`
    ![create-index-html](img/create-index-html.png)

1. Нажми `Ctrl + ,` чтобы открыть настройки `VSCode`
    - Если не сработало можно открыть через меню `Code` -> `Preferences` -> `Settings`
1. Включи автосохранение (`Auto Save`)
    ![vscode-enable-autosave](img/vscode-enable-autosave.png)
1. В первой строке файла `index.html` набери `!` и нажми табуляцию. У тебя появится такой текст:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
    </head>
    <body>
      
    </body>
    </html>
    ```
1. Набери в пустой строке между `<body>` и `</body>` текст `Привет! Я - Твоё Имя`
    - Если ты не настроил автосохранение, то сохрани нажав `ctrl + S` (`cmd + S` если у тебя MacOS)
1. Открой в проводнике директорию `my-first-page` и нажми правой кнопкой на файле `index.html`
1. В меню выбери пункт `Открыть с помощью` и выбери программу `Google Chrome`.
1. У тебя должна открыться твоя страница со словами `Привет! Я - Твоё Имя`

**Поздравляю! - Вы создали первую WEB-страницу.**

## Создаём аккаунт на Github
1. Зарегистрируйся на [Github](https://github.com/join) если у вас ещё нет аккаунта
    - Введи `Username`, `Email address` и `Password`
    - Нажми кнопку `Проверить` (`Check`) и реши задачки 
    - Нажми `Create account`
1. Заполни анкету 
    - What kind of work do you do, mainly? (например `Software Engineer`)
    - How much programming experience do you have? (например `A little`)
    - What do you plan to use GitHub for? (Например `Learn to code` и `Host a project`)
    - Нажми `Complete setup`
1. Открой свой почтовый ящик указанный при регистрации 
    - в письме `[GitHub] Please verify your email address.` нажмите ссылку `Verify email address`

## Пора показать ваш сайт миру!
1. Создай новый репозиторий на Github
    ![create-repo](img/create-repo.png)

1. Введи основные данные репозитория
    - введи название
    - Проверь что выбран `Public`
    - Поставь галочку `Add a README file`
    - Нажми кнопку `Create repository`
    
    ![img/new-repo-params](img/new-repo-params.png)

1. Найди ссылку для скачивания  
    - Нажми зелёную кнопку `Code`
    - Проверь что выбран `HTTPS`
    - Скопируй ссылку

1. Открой терминал в папке `my-first-page` (Правой клавишей внутри и `Git Bash Here`)
1. В терминале выполни команду `git clone сюда-вставь-скопированную-ссылку`.
1. Внутри папки `my-first-page` появится папка `my-first-website`
1. Перенеси файл `index.html` в папку `my-first-website`. 
    - Это можно сделать вручную через проводник или в терминале командой
        ```
        mv index.html my-first-website/index.html
        ```
1. Открой терминал во внутренней папке `my-first-website`
1. Запусти поочереди следующие команды
    ```
    git add index.html
    git commit -m 'My first page'
    git push
    ```
    - Последняя команда попросит вас ввести `username` (то что вы ввели при регистрации на Github) и нажать `Enter`
    - Дальше вводим пароль (символы отображаться не будут) и снова `Enter`
    - Если ошиблись, запускаем `git push` ещё раз и вводим опять имя и пароль
1. Если всё ок, то открывай свой репозиторий на `Github`
    ![my-github-repos](img/my-github-repos.png)
1. Там должно быть 2 файла `README.md` и `index.html`
    - Если `index.html` - значит `git push` не сработал (запускайте ещё раз и читайте ошибку)
1. Перейди на закладку `Settings`
    ![open-repo-settings](img/open-repo-settings.png)
1. Пролистай до раздела `GitHub Pages`
1. Выбери в выпадающем списке `main`
    ![gh-pages-settins](img/gh-pages-settins.png)
1. И нажми `Save`
    ![gh-pages-main-save](img/gh-pages-main-save.png)
1. Дождись пока ссылка на GH-Pages станет зелёной (примерно минуту)
    ![gh-pages-active-state](img/gh-pages-active-state.png)
1. Открой её, чтобы увидеть свою страницу
1. Теперь можно поделиться с друзьями :-)

## Сделаем наш сайт прекраснее!
1. Замени содержимое своего файла `index.html` на код с сайт [Bulma](https://bulma.io/documentation/overview/start/#starter-template)
1. Замени текст `Hello World` на своё приветствие!
1. Выполни в термале команды
    ```
    git commit -am 'my Bulma page'
    git push
    ```
