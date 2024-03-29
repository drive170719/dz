# Инструкция по работе с Git

## Что такое Git

Git — самая популярная в мире распределённая система контроля версий. Линус Торвальдс, разработчик ядра ОС Linux, создал этот инструмент ещё в 2005 году, а сегодня Git активно поддерживается как проект с открытым исходным кодом. Огромное количество открытых и коммерческих проектов используют Git для контроля версий.

В данной статье перечисляются самые основные команды, которые следует знать разработчику, чтобы освоить управление репозиториями GitHub на высоком уровне. Ознакомиться с ними будет полезно как новичкам, так и опытным разработчикам.

* 1. git init-Создать пустой репозиторий Git или вновь инициализировать существующий можно параметром init. При инициализации он создаст скрытую папку. В ней содержатся все объекты и ссылки, которые Git использует и создаёт в истории работы над проектом.
>Если вы прописали команду git init в терминале и не выдало ошибку, значит git настроен правильно и можно продолжать работу.

* 2. git status-Просмотреть статус нужного репозитория можно по ключевому слову status: его действие распространяется на подготовленные, неподготовленные и неотслеживаемые файлы.
>После того, как написали, что либо в файле, наберите команду git status и будет видна информация о текущем состоянии файла.

* 3. git add-добавляет содержимое рабочей директории в индекс для последующего коммита.
> Говоря простым языком, git add, сохраняет изменения, надо написать git add и имя файла (можно ввести первые буквы названия и нажать TAB, далее название наберётся само). В нашем случе это-  git add .\instrukciya.md

* 4. git commit — берёт все данные, добавленные в индекс с помощью git add, и сохраняет их слепок во внутренней базе данных.
>Пишем команду git commit -m "комментарий к сохранеию". К примеру git commit -m "pervii koment"
>(Пропишите пару строк, сохраните их, через Ctrl+S. Сделайте пару коммитов.)

* 5. Просматривать изменения, внесённые в репозиторий, можно с помощью параметра log. Он отображает список последних коммитов в порядке выполнения. 
>Введя данную команду, вы увидите все номера commit-ов.Если далее будут проблемы с написанием в терминале, нажмите q

* 6. git checkout — используется для переключения веток и выгрузки их содержимого в рабочую директорию.
>При помощи команды git checkout, можно перемещаться между commit-ами, а также ветками. Напишите git checkout и первые 4 цифры нужного комита.

* 7. git branch-Можно просматривать полный список веток, используя параметр branch. Команда отобразит все ветки, отметит текущую звёздочкой (*) и выделит её цветом.
>Кроме commit-ов можно создавать различные ветки.Представим, что ыетка master-чистовик, а другие ветки будут черновиком. Посмотреть список веток можно при помощи данной команды.

* 8. gi branch_name-Создать новую ветку можно с помощью параметра branch, указав имя ветки.
> Чтобы создать новую ветку введите команду git branch и добавьте имя новой ветки. Например git branch vtoraya_vetka (без пробелов). Также довайте сразу создадим еще две ветки.vtoraya_vetka и tretya_vetka. При помощи команды git branch, мы можем посмотреть список веток и на какой ветке находимся.

* 9. git checkout new_branch_name-Для автоматического перехода нужно добавить checkout branch name.

* 10. git merge branch name-Объединить две ветки можно параметром merge с указанием имени ветки. Команда объединит указанную ветку с основной.
 
* 11. git clone-копирует существующий репозиторий Git. Она похожа на команду SVN checkout, но имеет некоторые отличия: так, полученная «рабочая копия» представляет собой полноценный репозиторий Git с собственной историей и файлами, полностью обособленный от исходного репозитория.

* 12. git push-Git push — это одна из консольных команд Git. Она позволяет передать изменения из локального репозитория (набора файлов из папки .git) в удаленный.

* 13.git pull-sdиспользуется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым. Слияние удаленных вышестоящих изменений в локальный репозиторий — это обычное дело в процессе совместной работы на основе Git.

# Инструкция по работе с удаленным репозиторием

Регистрируемся на GitHub, создаем аккаунт и знакомим локальный git с удалённым GitHub, через git config. Затем создаём в GitHub, новый репозиторий и даём ему имя. Выбираем приявязать существующий репозиторий приявязать к локальному и выполняем три команды, что в инструкции.
 >В нашем случае это
 * 1. git remote add origin https://github.com/drive170719/Domashnee-Zadanie.git ( комнада гит должна понять, что у нас появился новый удалёный реаозиторий и его адрес)
 * 2. git branch -M main (указывае основную ветку)
 * 3. git push -u origin main (направляем удалёный репозиторий в локальный)

 Теперь наши репозитории связанны. Отправлять из git в GitHub, можно с помощью команды git push.

 Также можно вносить измениния в файл в удалёном репозитории. Закомитить его. И вызвать команду git pull . Тогда он перенесётся в локальный.

Вот такие пироги




