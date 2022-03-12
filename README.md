# The Command Line and Terminal

### Часто используемые команды в терминале Mac

### Горячие клавиши

| Команда | Описание |
| ----------- | ----------- |
| Ctrl + A   | Переместиться в начало набранной строки.  Это также работает практически для всех полей ввода в системе, за исключением IDE Netbeans.|
| Ctrl + E   | Переместиться в конец выбранной строки.  Это также работает практически для всех полей ввода в системе, за исключением IDE Netbeans. |
| Ctrl + Q   | Очистить текущую строку |
| Ctrl + L   | Очистить экран |
| Cmd + K    | Очистить экран |
| Ctrl + U   | Вырезать все символы с начала строки и до текущего положения курсора |
| Ctrl + K   | Вырезать все символы, начиная от текущего положения курсора и до конца строки |
| Ctrl + W   | Вырезать одно слово слева до первого пробела |
| Ctrl + Y   | Вставить то, что было вырезано последней командой "Вырезать" |
| Ctrl + H   | То же самое, что клавиша Backspace |
| Ctrl + C   | Прервать исполнение запущенной программы |
| Ctrl + D   | Выход из консоли если в консоли нет запущенных процессов или послать EOF запущенному процессу |
| Ctrl + Z   | Переместить запущенный процесс в фоновый процесс и приостановить его. Команда `fg` восстанавливает прежнее состояние процесса. |
| Ctrl + _   | Отменить последнюю выполненную команду. (Это знак подчеркивания, т.е. Ctrl + Shift + minus) |
| Ctrl + T   | Поменять местами символ справа от курсора с символом слева от курсора. Если курсор находится в конце строки, то поменять последние два символа местами.|
| Ctrl + F   | Переместить курсор на один символ вперед |
| Ctrl + B   | Переместить курсор на один символ назад |
| Option + →  | Переместить курсор на одно слово вперед |
| Option + ←  | Переместить курсор на одно слово назад |
| Esc + T  | Поменять местами слово слева от курсора со словом справа от курсора. Если курсор стоит в конце строки, то поменять последние два слова местами.|
| Tab  | Автодополнение строки именами файлов или папок, которые совпадают с началом строки |

## КЛЮЧЕВЫЕ КОМАНДЫ

| Команда | Описание |
| ----------- | ----------- |
| cd [folder] | Сменить директорию. Например `cd Documents` |
| cd |  Переместиться в домашнюю директорию |
| cd ~ |  Переместиться в домашнюю директорию |
| cd /  | Переместиться в корневую папку диска |
| cd -  | Переместиться в предыдущую директорию |
| ls | Список файлов и папок в текущей директории |
| ls -l | Список файлов и папок в текущей директории. Название каждого файла/папки печатается на отдельно строке |
| ls -a | Список файлов и папок в текущей директории с учётом скрытых файлов и папок|
| ls -lh| Список файлов и папок с размером объектов в Кб, Мб и т.д. |
| ls -R | Отобразить рекурсивно список всех файлов и папок в директории |
| sudo [command] | Выполнить команду с правами суперпользователя (Super User DO) |
| open [file] | Открыть файл (равносильно открытию файла двойным щелчком мыши) |
| top | Отобразить активные процессы. Нажмите `q` для выхода |
| nano [file] | Открыть файл в редакторе `nano` |
| vim [file] | Открыть файл в редакторе `vim` |
| clear |  Очистить экран |
| reset |  Сбросить дисплей терминала |

## ОБЪЕДИНЕНИЕ КОМАНД В ЦЕПОЧКИ

| Команда | Описание |
| ----------- | ----------- |
| [command-a]; [command-b] | Выполнить команду `a`, а затем выполнить команду `b` независимо от результата выполнения команды `a`|
| [command-a] && [command-b] | Выполнить команду `b` только если команда `a` выполнилась успешно|
| [command-a] &#124;&#124; [command-b] | Выполнить команду `b` только если команда `a` выполнилась с ошибкой |
| [command-a] & | Выполнить команду `a` в фоновом режиме|


## ПЕРЕДАЧА РЕЗУЛЬТАТОВ ОДНОЙ КОМАНДЫ ДРУГОЙ КОМАНДЕ

| Команда | Описание |
| ----------- | ----------- |
| [command-a] \| [command-b] | Выполнить команду `a` и передать результат выполнения команде `b`. Например `ps auxwww \| grep google` |


## ИСТОРИЯ КОМАНД

| Команда | Описание |
| ----------- | ----------- |
| history n |  Показать последние набранные команды. Добавьте вместо `n` число чтобы ограничить количество команд |
| Ctrl + r  | Интерактивные поиск среди последних набранных команд |
| ![value] |  Выполнить последнюю набранную команду, которая начинается c ‘value’ |
| !! |  Выполнить последнюю набранную команду |

## РАБОТА С ФАЙЛАМИ

| Команда | Описание |
| ----------- | ----------- |
| touch [file] |   Создать новый файл |
| pwd | Отобразить полный путь текущей директории |
| . |  Текущая директория. Например `ls .` |
| .. | Родительская директория, Например `ls ..` |
| ls -l .. | Список всех файлов директорий, которые находятся на том же уровне что и родительская директория |
| cd ../../ | Переместиться на 2 уровня вверх |
| cat | Объединение и печать содержимого файлов |
| rm [file] |  Удалить файл. Например `rm data.tmp` |
| rm -i [file] | Удалить файл с подтверждением |
| rm -r [dir] | Удалить директорию и её содержимое |
| rm -f [file] | Удалить файл без подтверждения |
| cp [file] [newfile] | Копировать файл в другой файл |
| cp [file] [dir] | Копировать файл в директорию |
| mv [file] [new filename] |  Переместить/Переименовать файл. Например `mv file1.ad /tmp` |
| pbcopy < [file] | Копировать содержимое файла в буфер обмена |
| pbpaste | Вставить содержимое из буфера обмена |
| pbpaste > [file] | Вставить содержимое из буфера обмена в файл. Например `pbpaste > paste-test.txt` |

## РАБОТА С ДИРЕКТОРИЯМИ

| Команда | Описание |
| ----------- | ----------- |
| mkdir [dir] | Создать директорию |
| mkdir -p [dir]/[dir] |  Создать директорию и вложенную директорию |
| rmdir [dir] | Удалить директорию (работает только с пустыми директориями) |
| rm -R [dir] | Удалить директорию и содержимое |
| less [file]|  Вывести содержимое файла на экран. Прервать вывод если он не вмещается на экран. Можно продолжить вывод нажав `Space`  |
| [command] > [file] |  Поместить результат выполнения команды в файл. Существующий файл будет переписан с нуля |
| [command] >> [file] | Поместить результат выполнения команды в файл. Существующий файл будет дополнен |
| [command] < [file] |  Передать содержимое файла на вход команде |

## ПОИСК

| Команда | Описание |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Искать файлы в заданной директории. Например `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Искать строки в файле, которые подпадают под шаблон. Например `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | Рекурсивно искать строки в файлах в заданной директории, которые подпадают под шаблон. |
| grep -v [search_pattern] [file] | Искать строки в файле, которые НЕ подпадают под шаблон |
| grep -i [search_pattern] [file] | Искать строки в файле, которые подпадают под шаблон с учётом регистра |
| mdfind [search_pattern] | Искать при помощи `Spotlight` (название, содержимое, другие данные). Например `mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | Искать при помощи `Spotlight` в заданной директории |

## ПОМОЩЬ

| Команда | Описание |
| ----------- | ----------- |
| [command] -h |  Вывод справки по команде|
| [command] --help | Вывод справки по команде |
| info [command] | Вывод справки по команде |
| man [command] |  Вывод руководства пользователя по команде [command] |
| whatis [command] | Вывод описания команды или команд подпадающих под шаблон [command] |
| apropos [search-pattern] | Поиск по базе данных команд по шаблону |

***BASH*** – название является аббревиатурой от «Bourne-again shell», отсылкой к более ранней оболочке Bourne и каламбуром термина «рожденный заново», самый популярный командный интерпретатор в юниксоподобных системах, в особенности в GNU/Linux.   
Bash можно установить с помощью инструмента управления пакетами, такого как Homebrew

- [Использование оболочки zsh в качестве стандартной оболочки на компьютере Mac ](https://support.apple.com/ru-ru/HT208050)

- [Ресурс по #zsh](https://wiki.archlinux.org/title/Zsh_(%D0%A0%D1%83%D1%81%D1%81%D0%BA%D0%B8%D0%B9))

---
---
### Using Z Shell  #zsh on Macs with the Learn Enough Tutorials
 https://news.learnenough.com/macos-bash-zshell 

Как сменить оболочки с `zsh` on `bash`? How to change shells
The main technique is to use the chsh program, which stands for “change shell”. Note that this procedure is entirely reversible (as described below), so there is no need to be concerned about damaging your system.
The first step is to confirm the identity of your current shell program using the echo command

```bash
$ echo $SHELL
/bin/bash
```
This prints out the `$SHELL` environment variable, which in most cases prints out the value of the current shell—in this case, Bash. (In rare cases, `$SHELL` may differ from the current shell, but the procedure below will still correctly change from one shell to another.) To change to `Zsh`, simply follow Apple’s suggestion from Listing 1 and run chsh (“change shell”) with the ` -s ` (“newshell”) option:

```bash
$ chsh -s /bin/zsh
```
You’ll almost certainly be prompted to type your system password at this point, which you should do. Then completely exit your shell program using **Command-Q** and relaunch it.
Once you’ve followed the steps above, you’ll be running Z shell instead of Bash, as you can confirm with echo:

```bash
$ echo $SHELL
/bin/zsh
```
If you ever want to switch back, simply use the same `chsh` command with bash in place of zsh:

```bash
$ chsh -s /bin/bash
```
As with the previous case, type in your password and then restart your terminal program. The result will be a restoration of your previous settings:

```bash
$ echo $SHELL
/bin/bash
```

---
### Отличия оболочек
Более существенное отличие связано с поведением по умолчанию. Системы Bash обычно называют потенциально опасные команды `rm` (удалить), `mv` (переместить) и `cp` (копировать) версиями, использующими параметр `-i`, который требует подтверждения для любых возможных удалений:
При удалении требуется подтверждение

#### Bash example.

```bash
$ touch foo
$ rm foo
remove foo? n
$ ls foo
foo
```

`rm` alone is sufficient. Его можно переопределить с помощью `-f` (force) option:

#### Bash example continued.

```bash
$ rm -f foo
$ ls foo
ls: foo: No such file or directory
```

The same patterns apply to the wildcard operator ` * `:

#### Bash example.

```bash
$ touch foo.baz
$ touch bar.baz
$ rm *.baz
remove bar.baz? n
remove foo.baz? n
$ rm -f *.baz
$ ls *.baz
ls: *.baz: No such file or directory
```

Для использования таких команд в zsh нужно внести изменения
To ensure that this behavior is the same in Zsh, two changes are needed. First, we need to add the corresponding aliases, which fortunately follow the same syntax as Bash 

#### Avoid accidental deletions

```bash
alias rm='rm -i'
alias mv='mv -i'
alias cp='cp -i'
```
[Подробнее в статье есть гайды](https://news.learnenough.com/macos-bash-zshell)

--- 
[Learn Enough Command Line to Be Dangerous](https://www.learnenough.com/command-line-tutorial/basics) 

Графический интерфейс пользователя (GUI) может значительно упростить использование компьютера, но во многих случаях наиболее мощным и гибким способом взаимодействия с компьютером является интерфейс командной строки (CLI).
Возможно нужно будет поставить [iTerm2](https://iterm2.com/features.html)  

Тильда ` ~ ` указывает на домашний каталог, в котором вы находитесь.
Забавно, что причина, по которой символ тильды используется для домашнего каталога, заключается просто в том, что клавиша “Home” была такой же, как клавиша для создания `~` на некоторых ранних клавиатурах

<img alt="image" src="images/1.png"> </img> 

The **prompt** (to “prompt – побудить к действию, подсказка” the user to do something) followed by a **command** (as in “give the computer a command”), an **option** (as in “choose a different option”), and an **argument** (as in the “argument of a function” in mathematics).  prompt выдается терминалом автоматически, и вам не нужно его набирать

<img alt="image" src="images/2.png"> </img> 







