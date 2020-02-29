## Базавой шаблон для верстки проектов с использованием tars

## Документация

    Документакция доступна по ссылке: [установить TARS]: https://github.com/tars/tars


## Основные команды

**Обращаем ваше внимание, что предпочтительно использовать [TARS-CLI](https://github.com/tars/tars-cli). Это удобнее, нагляднее, занимает меньше места! Все команды, описанные ниже, [доступны в TARS-CLI](https://github.com/tars/tars-cli/blob/master/docs/ru/commands.md), используйте именно его для работы над проектом. TARS запускался через Gulp, когда не было CLI.**

`gulp init` — Инициализирует проект с заданными опциями в tars-config. Создает файловую структуру.

`gulp re-init` — **команда будет удалена в одном из следующих релизов** Переинициализирует проект с заданными опциями в tars-config. Предлагается использовать данную команду, если вы инициализировали проект с неверными опциями. **Внимание, при переинициализации все папки и файлы удаляются.**

`gulp` или `gulp build` — делает сборку проекта. Подключаются не минимизированные файлы. Тип сборки зависит от переданных ключей вместе с этой командой. Доступные ключи:

* `--min` – в html подключаются минимизированные файлы.
* `--release` – в html подключаются минимизированные файлы, в названии которых есть hash. Данный режим полезен, если вы напрямую выкладываете верстку на сервер. 

`gulp dev` — инициализация сборщика в режиме разработки. Создается dev-версия проекта, без всех минификаций. Также запускает вотчеры за файлами проекта. Доступные ключи:

* `--lr` – инициализация livereload (живая презагрузка страницы при изменениях в файлах проекта), если он включен в конфиге проекта.
* `--tunnel` – инициализация проекта с расшариванием верстки во внешний веб.

Ссылка будет указана в консоли. Также будет указана ссылка на панель управления устройствами, на которые расшарена верстка.

`gulp build-dev` — генерация dev-версии проекта без вотчеров.

Ключи, доступные при любом режиме сборки:

* `--ie8` – включить в сборку стили для ie8.
* `--ie9` – включить в сборку стили для ie9.
* `--ie` – включить в сборку стили для ie9 и ie8.


## Особенности данной сборки
* Включены базовые иконки
* Загружена моя фавиконка)
* Изменены стандартные настройки для более удобной разработки
* Добавлены нужные mixin-ы
* 
