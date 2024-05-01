[<img src="https://img.shields.io/badge/Telegram-%40Me-orange">](https://t.me/sho6ot)


![img1](.github/images/demo.png)

> 🇪🇳 README in english available [here](README-EN.md)

## Функционал  
| Функционал                                                     | Поддерживается  |
|----------------------------------------------------------------|:---------------:|
| Многопоточность                                                |        ✅        |
| Привязка прокси к сессии                                       |        ✅        |
| Авто-покупка предметов при наличии монет (tap, energy, charge) |        ✅        |
| Рандомное время сна между кликами                              |        ✅        |
| Рандомное количество кликов за запрос                          |        ✅        |
| Поддержка tdata / pyrogram .session / telethon .session        |        ✅        |


## [Настройки](https://github.com/shamhi/HamsterKombatBot/blob/main/.env-example)
| Настройка                | Описание                                                                                      |
|--------------------------|-----------------------------------------------------------------------------------------------|
| **API_ID / API_HASH**    | Данные платформы, с которой запускать сессию Telegram _(сток - Android)_                      |
| **MIN_AVAILABLE_ENERGY** | Минимальное количество доступной энергии, при достижении которой будет задержка _(напр. 100)_ |
| **SLEEP_BY_MIN_ENERGY**  | Задержка при достижении минимальной энергии в секундах _(напр. 200)_                          |
| **ADD_TAPS_ON_TURBO**    | Сколько тапов будет добавлено при активации турбо _(напр. 2500)_                              |
| **AUTO_UPGRADE**         | Улучшать ли пассивный заработок _(True / False)_                                              |
| **MAX_LEVEL**            | Максимальный уровень прокачки апгрейда _(напр. 20)_                                           |
| **APPLY_DAILY_ENERGY**   | Использовать ли ежедневный бесплатный буст энергии _(True / False)_                           |
| **APPLY_DAILY_TURBO**    | Использовать ли ежедневный бесплатный буст турбо _(True / False)_                             |
| **RANDOM_CLICKS_COUNT**  | Рандомное количество тапов _(напр. 50,200)_                                                   |
| **SLEEP_BETWEEN_TAP**    | Рандомная задержка между тапами в секундах _(напр. 10,25)_                                    |
| **USE_PROXY_FROM_FILE**  | Использовать-ли прокси из файла `bot/config/proxies.txt` _(True / False)_                     |


## Установка
Вы можете скачать [**Репозиторий**](https://github.com/shamhi/HamsterKombatBot) клонированием на вашу систему и установкой необходимых зависимостей:
```shell
~ >>> git clone https://github.com/shamhi/HamsterKombatBot.git 
~ >>> cd HamsterKombatBot

# Если вы используете Telethon сессии, то клонируйте ветку "converter"
~ >>> git clone https://github.com/shamhi/HamsterKombatBot.git -b converter
~ >>> cd HamsterKombatBot

# Linux
~/HamsterKombatBot >>> python3 -m venv venv
~/HamsterKombatBot >>> source venv/bin/activate
~/HamsterKombatBot >>> pip3 install -r requirements.txt
~/HamsterKombatBot >>> cp .env-example .env
~/HamsterKombatBot >>> nano .env  # Здесь вы обязательно должны указать ваши API_ID и API_HASH , остальное берется по умолчанию
~/HamsterKombatBot >>> python3 main.py

# Windows
~/HamsterKombatBot >>> python -m venv venv
~/HamsterKombatBot >>> venv\Scripts\activate
~/HamsterKombatBot >>> pip install -r requirements.txt
~/HamsterKombatBot >>> copy .env-example .env
~/HamsterKombatBot >>> # Указываете ваши API_ID и API_HASH, остальное берется по умолчанию
~/HamsterKombatBot >>> python main.py
```

Также для быстрого запуска вы можете использовать аргументы, например:
```shell
~/HamsterKombatBot >>> python3 main.py --action (1/2)
# Или
~/HamsterKombatBot >>> python3 main.py -a (1/2)

# 1 - Создает сессию
# 2 - Запускает кликер
```
