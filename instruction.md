# Инструкция по работе с Git, используя Markdown

## Установка и настройка Git и Visual Studio Code

1. **Для установки ПО необходимо скачать и затем установить его:**
    - Установка Git для Windows, Mac, Linux: <https://git-scm.com/downloads>
    - Установка VSCode для Windows, Mac, Linux: <https://code.visualstudio.com/download>

2. **Настройка ПО:**

- В терминале необходимо прописать:

    *git --version*

- Если всё установлено правильно, должно быть что-то вроде: 

    *git version 2.34.1.windows*

    ![Git_version](/Skrin/Git_version.JPG)

- После этого нужно представиться GITу введя команды:

    *git config --global user.email "ВАШ email"*

    *git config --global user.name "ВАШЕ Имя"*

**Установка и настройка ПО завершены!**

## Работа с GIT

1. Cоздаем папку, в которой мы будем работать, например ***Git_HW_1***, запускаем VSC и открываем эту папку:
![Git_version](/Skrin/VSC_open.JPG)

2. Нажимаем пункт меню ***Терминал - Создать терминал (Cntr+Shift+`)***. Открывется окно терминала:
![Git_version](/Skrin/VSC_terminal.JPG)

3. В терминале вводим команду ***git init*** (команда инициализирует директорию в новый репозиторий Git) и получаем следующее сообщение:
![Git_version](/Skrin/VSC_Git_init.JPG)

4. Команда ***git status*** отображает состояние рабочего каталога и раздела проиндексированных файлов:
![Git_version](/Skrin/Git_status.JPG)

5. Создаем файл ***instruction.md*** в нашей папке и снова выполняем команду ***git status*** и видим, что у нас был создан файл и от нас требуются действия:
![Git_version](/Skrin/Git_status_1.JPG)

6. Вводим команду ***git add .\instruction.md*** (команда добавляет изменение из рабочего каталога в раздел проиндексированных файлов), после этого снова вводим ***git status*** и получаем следующее:
![Git_version](Skrin/Git_add.JPG)
Также можно использовать команду ***git add --all*** (добавляет все измененные и неотслеживаемые файлы в репозиторий и обновляет дерево изменений репозитория).

7. Далее вводим команду ***git commit -m "Create file instruction.md"*** (комментируем коммит прямо из командной строки вместо текстового редактора):
![Git_version](/Skrin/Git_commit.JPG)
Снова проверям состояние ***git status***:
![Git_version](/Skrin/Git_status_commit.JPG)