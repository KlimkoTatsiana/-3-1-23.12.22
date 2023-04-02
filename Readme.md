# Инструкция по работе с Git

## Что такое гит?

***Git*** - самая популярная реализация распределённой системы контроля версий(версионность поддерживается и на сервере, и у каждого клиента). Самой распространнённой реализацией ***Git*** является (GitHub)[https://github.com]

## Подготовка репозитория

Для создания репозитория используется команда *git init*. Для этого необходимо открыть в терминале папку с будущем репозиторием и написать *git init*

## Создание коммитов

### Добавление файлов к коммиту

Для добавления файла к новому коммиту используется команда *git add*. Используется она следующим образом: в терминале с папкой-репозиторием пишем *git add <название файла>*.

### Создание коммита

Для создание новой фиксации(коммита) используется команда *git commit*. Для этого в терминале с папкой-репозиторием пишем *git commit -m "<сообщение к коммиту>*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!***

## Перемещение между коммитами

Для перемещения на другую фиксацию(коммит) используется команда *git checkout*. Для этого необходимо, как показано в прошлом пункте, в журнале изменений найти необходимый коммит и его хеш(номер), после чего в терминале с папкой-репозиторием надо написать *git checkout <хеш коммита>*. После выполнения этой команды мы попадаем в состояние **detached head**, в котором никакие следующие коммиты сохраняться не будут. Для выхода из этого состояния необходимо написать *git checkout master*.

## Журнал изменений

Для просмотра истории изменений используется команда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*

## Перемещение между "сохранениями"

### Ветки в гит

## Создание веток в гит

Для создание новой ветки используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <название ветки>*.

## Слияние веток и разрешение конфликтов

Для слияния веток в *Git* Используется команда *git merge* , для этого в терминале необходимо сначала перейти в ветку (например : Master) Для этого используется команда *git checkout master*, затем написать команду *git merge<название ветки>*. (Команда merge вызывается из той ветки куда вы хотите слить изменения!!!!)  Разрешение конфликтов при слиянии веток. Для получения финальной версии необходимо либо выбрать вариант вручную: Для этого необходимо удалить строки *<<<<HEAD И строку =====* после необходимо в терминале набрать команду *git add* и команду *git commit -m "коментарий"*, Либо воспользоватся встроеным механизмом VSC.

## Удаление веток

### Работа с удаленным репозиторием

## скачивание репозитория

Для начала следует завести акаунт на *github*. Там мы находим интересующий нас репозиторий. Копируем его адресс на вкладке *Code*. На комрьютере запускаем терминал, выбираем свободную папку. В терминале папки-репозитория прописываем команду *git branch -M master* - этим мы создаём главную ветвь в скачиваемом репозитоии. Далее клонируем на компьтер репозиторий, пишим команду *git clone <адрес скопированный с github>*. теперь репозиторий находится у нас на компьютере и мы можем с ним работать. Теперь следует ввести команду *cd <название клонированной паки>* для перехода в клонированный репозиторий.

## Передача репозитория

## Создание удаленного репозитория
