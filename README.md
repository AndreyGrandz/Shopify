# Shopify
Сборка Shopify/Shopify 2.0
Устанавливаем Node.js - https://nodejs.org/uk/
Устанавливаем модуля - npm i (в терминале проекта)

1. Заходим в config.yml. Вводим theme_id, password (api_key - private apps), store_url.
2. Делаем theme download (также в терминале)
3. Theme deploy - чтобы зачистить старые файлы темы и оставить тему чистую. Делать в том случае, когда нужно иметь полностью чистую тему, если же проект под
саппорт, то просто theme download
4. theme open - открываем тему
5. npm run dev - запускаем watcher of theme


///// Стили
Все стили находятся в папке src - styles. Main file: custom.scss. Сюда импортируем другие ваши стили. Папка global, в ней можем создать папку common.
В папке common создам уже ваши папки, котоыре вам нужны для создания красивой иерархии стилей.
Например, homepage, а в ней уже файлы стилей для данной page. Все файлы билдятся в файл styles.css. Он находится в главной папке - assets. Файл подключен 
в theme.liquid.

///// Скрипты
Все скрипты находятся в папке src - scripts. Main file: custom.js. Сюда импортируем другие ваши скрипты. Папка common, в ней можем создать папку customScripts
(или же с другим названиям, под ваше усмотрения).
В папке customScripts создам уже ваши папки, котоыре вам нужны для создания красивой иерархии скриптов.
Например, homepage, а в ней уже файлы скриптов для данной page. Все файлы билдятся в файл scripts.bundle.js. Он находится в главной папке - assets. Файл подключен 
в theme.liquid.

///// Section/snippets
Папки section, snippets
