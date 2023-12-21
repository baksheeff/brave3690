# **Инструкция по работе с Git**

## Основные команды:

### Создание репозитория:

``` sh
git init
```

Эта команда инициализирует новый репозиторий GIT и начинает отслеживание существующего каталога. В существующий каталог добавляется скрытая вложенная папка, в которой размещается внутренняя структура данных, необходимая для управления версиями.

``` sh
git status - 
```
Выводит состояние изменений: не отслеживаются, изменены или подготовлены.

### Создание коммита:

``` sh
git add - 
```

Подготавливает изменение. GIT отслеживает изменения в базе кода разработчика, но для включения изменений в журнал проекта необходимо подготавливать их и создавать моментальные снимки. Эта команда выполняет первую часть этого двухэтапного процесса, то есть подготовку. Все подготовленные изменения станут частью следующего моментального снимка и журнала проекта. Раздельные подготовка и фиксация дают разработчикам полный контроль над историей проекта без необходимости изменять подход к написанию кода и работе в целом.

``` sh
git commit - 
```
Cохраняет моментальный снимок в журнале проекта и завершает процесс отслеживания изменений. Иначе говоря, фиксация похожа на создание фотографии. Все, что было подготовлено с помощью команды git add, станет частью моментального снимка при использовании git commit.

### Работа с ветками:

``` sh
git branch - 
```
Показывает ветви, с которыми ведется локальная работа.

``` sh
git checkout - 
```
Позволяет перемещаться между ветками, созданными командой git branch . При переключении ветки происходит обновление файлов в рабочем каталоге в соответствии с версией, хранящейся в этой ветке, а Git начинает записывать все новые коммиты в этой ветке.

``` sh
git merge - 
```
Выполняет слияние линий разработки. Эта команда обычно применяется для объединения изменений, внесенных в двух разных ветвях. Например, разработчик выполняет слияние, когда необходимо объединить изменения из ветви функции с главной ветвью для развертывания.

### Работа с удаленным репозиторием:

``` sh 
git clone -
```
 
Это утилита командной строки Git для выбора существующего репозитория и создания его клона, т. е. копии. На этой странице описаны варианты расширенной конфигурации и распространенные примеры использования команды git clone .

``` sh
git pull - 
```

Применяет к локальной линии разработки обновления из удаленного аналога. Разработчики используют эту команду, если коллега выполнил фиксации в ветви удаленного репозитория и эти изменения нужно отразить в локальной среде.

``` sh
git push - 
```
Обновляет удаленный репозиторий с учетом фиксаций, выполненных в ветви локально.