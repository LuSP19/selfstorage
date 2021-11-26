###Инструкция по подключению тестовой оплаты


##### Как создать своего бота и подключить оплату?

- Найти @botfather в Telegram, запустить его командой 
`/start`
- Создать нового бота командой `/newbot`
- Выбрать название для бота,
- Выбрать псевдоним для бота, по которому его можно будет найти, используя поиск. Псевдоним должен заканчиваться на bot. Если все проходит успешно, вы получаете токен следующего вида:  
`12312312312:12318C-123123123`  
Бот создан. Самое время подключить оплату. 
- Для этого в диалоге с @botfather введите:
`/mybots` для настройки своих ботов. 
- Выберете того бота, к которому будет подключаться оплата
- В открывшемся подменю выберите раздел `Payments`
- В следующем появившемся списке нажмите на кнопку `Сбербанк` затем на `Connect Сбербанк Test` для подключения тестовой оплаты
- Вы автоматически перейдете в диалог с ботом Сбербанка. Необходимо начать диалог командой `/start` и написать `test` для получения тестового токена
- Возвращайтесь к @botfather, ищите подобный текст:  
```
1 method connected:
Сбербанк Test: 213123:TEST:okpokpo123123pok 
2011-11-11 11:11
```
- То, что после `Сбербанк Test` - токен Сбербанка
- Номера карт для проведения тестовой оплаты находятся здесь:  
  https://securepayments.sberbank.ru/wiki/doku.php/test_cards

Теперь в папке, где находится python-файл cоздать .env файл следующего содержания:
```text
BOT_TOKEN = "ТОКЕН ВАШЕГО БОТА"
SB_TOKEN = "ТОКЕН СБЕРБАНКА"
```
Готово! Тестовая оплата подключена










