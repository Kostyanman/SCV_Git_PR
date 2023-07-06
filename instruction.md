]![Logo](Git.png)

# Работа с Git и GitHub

## 1) Проверка наличия установленного Git

В терминале выполнить команду *`git version`*
Если Git установлен появится сообщение с информацией о версии программы, иначе будет сообщение об ошибке.

## 2) Установка Git

Загружаем последнюю версию Git с сайта https://git-scm.com
Устанавливаем с настройками по умолчанию.

## 3) Настройка Git

При первом использовании Git необходимо представиться. Для этого нужно выполнить в терминале две команды
```
git config --global user.name «Ваше имя английскими буквами»
git config --global user.email ваша почта@example.com
```

## 4) Инициализация репозотория

Для работы с Git необходимо создать папку.
Открываем данную папку в Git. В терминале необходимо выполнить команду 
```
 git init
  ``` 

Данная команда позволяет нам отслеживать все действия происходящие в папке.

## 5) Запись изменений в репозитории

### Для получения информации о внесенных изменениях в вайле необходимо выполнить команду
```
 git diff
 ```
 
  Которая покажет все изменения проделанные в файле.

### После этого выполняем команду 
```
git status
```
 Данная команда покажет что есть изменения в файле но они не записаны.

### Далее необходимо добавить изменения к отслеживаемому файлу выполнив это командой 
```
git add <Необходимо написать имя файла с расширением>
```

### После чего необходимо произвести запись изменений выполнив команду 

```
git commit -m "Нужно написать сообщения с указанием изменений внесенных в данный комит
```

После чего дерево задачь очиститься и приступаем к новым изменениям.


## 6) Просмотр истории комитов

Для того что бы посмотреть историю всех комитов записанных в файле необходимо выполнить команду 
```
git diff
```

Данная команда покажет все комиты с их индивидуальным именем.

## 7) Перемещение между сохранениями

Для перемещения между сохранениями необходимо выполнить команду
```

git chekout <и указать первые 5-7 символов индивидуального номера комита>
```

Для возврашения к актуальной версии файла необходимо выполнить команду
```
git chekout master
```

## 8) Игнорирование файлов
Для того, что бы исключить из отслеживания в репозиториях отдельные файлы и папки Необходимо создать файл ***`.gitignore`***
И написать в него названия или шаблоны соответствующие файлам или папкам.

## 9) Создание веток в Git
Список веток в репозитории можно посмотреть с помощью команды 
```
git branch
```
Создать ветку можно командой
```
Git branch <название новой ветки>
```
По умолчанию имя основной ветки в Git - *main*

Для переключения между ветками использкется команда 
```
git checkout <название ветки куда хотим перейти>
```

## 10) Слияние веток и устранениразрешениее конфликтов
Для слияния выбранной ветки с текущей нужно выполнить команду: 
```
git merge <название выбранной ветки>
```
```
git chechaut -b <Название ветки которую хотим удалить>
```


Команда для удаления ветки

# Работа с удаленными репозиториями

### 1. Создали аккаунт на Github.com

### 2. Создали локальный репозиторий

### 3. "Подружили" наш локальный и удаленный репозиторий. Github при зоздании нового репозитория подскажет как это можно сделать.

### 4. Отправввить (push) наш локальный репозиторий в удаленный (на Github), при этом нам, возможно, нужна будет авторизация на удаленном репозитории. 

### 5. Провести изменения "с другого компьютера"

### 6. Загрузить с удаленного репозитория на локальный по команде (pull)

# Pull request

1. Делаем форк (fork) интересующего нас репозитория.

2. Выполняем команду 
```
Git clone
```
Для выведения нашей версии данного репозитория

3. Создаем новую ветку в реппозитории для внесения своих изменений.

**Производим все изменения только в данной ветке**

4. Отправляем все изменения на свой аккаунт Github по команде
```
Git push
```

5. В окне на Github появляется возможность отправить pull request.