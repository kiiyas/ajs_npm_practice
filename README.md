# практика по npm-eslint-babel

AJS-17, 2021

поинт в том, чтобы любой разраб смог запустить проект полностью идентичный твоему, используя только 
- git clone ...
- npm install
- npm start

папка dist/ нужна только как вместилище для компилирующихся файлов в результате работы команд из package.json
  
-  "start": "npm run build & http-server ./dist",  (выполняет build и подключает хттп-сервер)
  
-  "build": "stylus ./src/index.stylus --out ./dist && cp src/**.html dist/ && run babel",  
  (компилит css из stylus'а, скрипты для старых версий, копирует хтмл и кидает все это в папку dist/, которая генерится первой копандой полностью)
  
-  "lint": "eslint ./src", (находит ошибки, '$ npm run lint -- -- fix' правит их автоматически по возможности)

-  "babel": "babel ./src -d ./dist"
  
===> требуется WebPack
