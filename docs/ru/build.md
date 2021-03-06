# Сборка

## Используемые инструменты

* npm: 6.x
* node: 8.x

## Разработка

Мы используем Webpack HMR при разработке Boostnote.
Выполнение следующих команд в корне проекта запустит Boostnote с настройками по умолчанию.

Установите необходимые пакеты с помощью yarn.

```
$ yarn
```

Соберите и запустите.

```
$ yarn run dev
```

> ### Примечание
> В некоторых случаях вам необходимо обновить приложение вручную.
> 1. При редактировании метода конструктора компонента
> 2. При добавлении нового класса CSS (аналогично 1: Класс CSS перезаписывается каждым компонентом. Этот процесс выполняется в методе Constructor.)

## Деплой

Мы используем Grunt для автоматического деплоя.
Вы можете создать задачу, используя `grunt`. Однако мы не рекомендуем этого делать, так как задача по умолчанию включает в себя код и аутентификацию.

Мы подготовили отдельный скрипт, который просто создает исполняемый файл.

```
grunt pre-build
```

Вы найдете исполняемый файл в папке `dist`. Обратите внимание: автоматическое обновление не будет работать, потому что приложение не подписано.

Если вам необходимо, вы можете использовать код или аутентификацию с помощью этого исполняемого файла.

---

Special thanks:
Translated by @AlexanderBelkevich
