# Dao.Casino Hackathon

Команда DAO.Casino рада приветствовать вас на хакатоне!
Мы подготовили для вас несколько крутых задач. Н
е упустите свой шанс попробовать свои силы в создании блокчейн-игр!

Присоединяйтесь к нашему чату в [telegram](https://t.me/daocasino_developers)
Удачи!

## Содержание
    
- [Задачи](#Задачи)
- [Номинации](#Номинации)
- [Технические требования](#Технические-требования)
- [Правила подачи решений](#Процедура-подачи-работ-от-участников)

## Задачи

Мы предлагаем вам несколько задач по улучшению нашего протокола. Авторы лучших решений и реализаций будут вознаграждены в рамках номинаций, либо отдельно на усмотрение нашей команды.

### Сделать игру c использованием DAO.Casino SDK

SDK и документация https://developers.dao.casino/

### Интегрировать элементы протокола в игру

Например, в существующую игру вы добавляете механику, основанную на элементах нашего протокола (Signidice, GameChannels)

### Создать chrome extension для работы с играми:

разработать браузерное расширение (форк/аналог [metamask](https://metamask.io/)) который позволит:

 - импортировать/создать аккаунт (приватный ключ / mnemonic) 
 - принимать данные из iframe, и подписывать эти данные приватным ключом (без спроса пользователя) и передавать подпись обратно в iframe.
 - уметь валидировать приходящие данные и в случае невалидность выдавать предупреждение
 - сохранять данные и подписи этих данных
 - иметь интеграцию с web3js 1.0

Опционально предлагается:

 - Отобразить в доступном виде данные, которые подписывались, 
 - иметь возможность запрашивать данные со смарт-контракта
 - иметь возможность отправлять данные на смарт-контракт,
 - иметь интеграцию с gameChannels, отзываться только на подписи функций gameChannels(open/update/close/gameRound), 
 - иметь вайтлист/блеклист смарт-контрактов/сайтов/открытых ключей.

### IPFS deployer

Реализация механизма деплоя игры в IPFS c последующей записью в контракт Game Market

Steps:

 - Написать деплой игры (размер ~50-150 MB) в IPFS через ipscend.js либо своим способом (поднятие ipfs демона и т.д.)
 - После получение хеша нужно добавить игру на контракт (Game market contract) (адрес контракта игры и хеш ipfs, по которому расположен фронтенд игры)
 - Получение и рендер списка игр

## Номинации

### Призовой фонд: 10 ETH (в токенах BET)

Дополнителнительные бонусы:

 - **Размещение игры на платформе и дальнейшее проодвижение игры**
 - **Попадание команды в Sandbox для разработчиков**
 - **Трудоустройство в одном из крупнейших проектов в идустрии Igaming на блокчейне**

Исходя из наиболее значимых для нас направлений развития и приоритетов, мы предлагаем следующие номинации:

### «Лучшая игра, созданная на протоколе DAO.Casino»

Создайте новую игру на нашем протоколе при помощи наших инструментов!

 - Принимаются одноранговые (одноходовые) игры с простой бинарной логикой и элементом случайного выбора (результат определяется алгоритмом генерации случайных чисел. Примеры таких игр: Dice, Slots, Roulette, Баккара, "Наперстки", "Угадай число". Удивите нас интерпретацией таких простых механик!

### «Лучшая интеграция протокола DAO.Casino»

Если у вас уже есть готовые игры, интегрируйте DAO.Casino в существующий проект! Используя наш инструментарий, интегрируйте мини-игры, лут-боксы, лотереи!

 - Реализация подразумевает использование механики Signidice и/или Game channels, либо нашего протокола в иной форме.

### «Лучшее решение для протокола DAO.Casino»

Знаете, как нам помочь улучшить наш продукт или реализацию? Предлагайте собственные механизмы игр, получения случайных чисел, а также offchain-решения и многое другое!

- критерий оценки - полезность для протокола Dao.Casino или его конкретной реализации. 

### «Лучший смарт-контракт»

Для гуру **Solidity!** Напишите лучший смарт-контракт игры, реализуйте сложную логику или расширьте функционал исходных контрактов!

 - обязательна возможность компиляции решения и его развертывания в **Ropsten network**

### «Лучшая визуализация»

Красивая графика и богатая фантазия ваш конек? Нарисуйте и реализуйте визуальное решение для игры! Пусть, например, единорог вращает колесо фортуны, а хомяки подбрасывают кубики!

- игра должна использовать  протокол Dao.Casino, либо быть совместимой с ним

## Технические требования:

Протокол реализован на стеке JS/Solidity, поэтому все решения должны быть реализованы на нем, либо иметь возможность интеграции с ним:

 - Javascript (ES6+) / React.js / Vue.js / Angular.js / Pixi.js / Phaser
 - Docker, Node.JS (10.0), IPFS
 - Solidity, Truffle, Web3.js

## Процедура подачи работ от участников:

Решения принимаются в виде **pull-request'ов** в этот репозиторий!

 - сделайте форк **этого** репозитория
 - Реализуйте свое решение в собственном форке
 - оформите README по [образцу]()
 - отправьте **pull-request**
 - ...
 - **PROFIT!**
