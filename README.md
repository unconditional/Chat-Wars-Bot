# Chat-Wars-Bot
Бот для текстовой мморпг Chat Wars в Telegram<br />
НЕ ПЫТАЙТЕСЬ СКОМПИЛИРОВАТЬ КЛИ НА ВИНДОУС И ТЕЛЕФОНАХ, ЕСЛИ ВЫ НЕ ШАРИТЕ - НЕ ПОЛУЧИТСЯ. <br />

Работающие функции бота:
  - тратить всю выносливость в лес/пещеру (по умолчанию ходит только в лес)
  - арена с рандомным выбором места атаки и защиты
  - перехват корованов
  - атака/защита по приказу бота/игрока или автоматическая защита замка
  - донат в казну замка перед битвой (по умолчанию выключен)
  - донат в лавку вместо казны (покупка-продажа барахла) (по умолчанию выключен. Для работы должен быть включен обычный донат. Если инвентарь полон - отключается, и происходит обычный донат в казну)
  - прокачка атаки/защиты при получении уровня (по умолчанию выключен)
  - ответы бота в групповой чат (по умолчанию выключен)
  - форвард лесных квестов от бота для помощи
  - сохранение текущего состояния и настроек в конфиг-фаил, для восстановления после перезапуска
  - постройки в замке, когда закончилась арена и нет стамины
  - суммирование стока через PenguindrumStockBot

Как запустить:<br />
  1) Устанавливаем telegram-cli по официальной инструкции [https://github.com/vysheng/tg]<br />
  2) Устанавливаем pip3: sudo apt-get install python3-pip<br />
  3) Устанавливаем pytg для 3 питона: pip3 install pytg pytz<br />
  4) Запускаем telegram-cli: ./telegram-cli --json -P 1338<br />
  5) Качаем этот скрипт и запускаем: `python3 ./main.py --admin "ваш ник" --order "ник игроков/ботов, выдающих приказы, через запятую   без пробелов" --castle "blue/red/black/white/yellow" --gold "сколько золота оставлять в кармане при автодонате" --buy "любое значение для включения доната в лавку" --lvlup "lvl_def - прокачка защиты/lvl_atk - прокачка атаки" --group_name 'название группового чата для отправки сообщений'`<br />
  6) Для работы с капчой, начинаем общение с @ChatWarsCaptchaBot (тестируется) 
  7) Для работы со стоками начинаем общение с @PenguindrumStockBot и @chatwarstradebot. А так же в первом объявляем майн профиль по инструкции бота
  
Команды боту от админа:<br />
    #help Список всех команд<br />
    #enable_bot - Включить бота<br />
    #disable_bot - Выключить бота<br />
    #enable_arena - Включить арену<br />
    #disable_arena - Выключить арену<br />
    #enable_les - Включить лес<br />
    #disable_les - Выключить лес<br />
    #enable_peshera - Включить пещеры<br />
    #disable_peshera - Выключить пещеры<br />
    #enable_corovan - Включить корован<br />
    #disable_corovan - Выключить корован<br />
    #enable_order - Включить приказы<br />
    #disable_order - Выключить приказы<br />
    #enable_auto_def - Включить авто деф<br />
    #disable_auto_def - Выключить авто деф<br />
    #enable_donate - Включить донат<br />
    #disable_donate - Выключить донат<br />
    #enable_buy - Включить донат в лавку вместо казны<br />
    #disable_buy - Вылючить донат в лавку вместо казны<br />
    #enable_quest_fight - Включить битву во время квеста<br />
    #disable_quest_fight - Выключить битву во время квеста<br />
    #lvl_atk - качать атаку<br />
    #lvl_def - качать защиту<br />
    #lvl_off - ничего не качать<br />
    #status - Получить статус<br />
    #hero - Получить информацию о герое<br />
    #push_order - Добавить приказ<br />
    #order - Дебаг, последняя команда защиты/атаки замка<br />
    #log - Дебаг, последние 30 сообщений из лога<br />
    #time - Дебаг, текущее время<br />
    #lt_arena - Дебаг, последняя битва на арене<br />
    #get_info_diff - Дебаг, последняя разница между запросами информации о герое<br />
    #ping - Дебаг, проверить жив ли бот<br />
    #enable_build - Включить постройки<br />
    #disable_build - Выключить постройки<br />
    #build_target - Задать цель для построек<br />
    #stock - Обновить сток в боте<br />
