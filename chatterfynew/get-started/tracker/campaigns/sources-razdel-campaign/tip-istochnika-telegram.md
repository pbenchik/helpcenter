---
description: Настройка Telegram-источника для канала, публичного канала или бота.
icon: telegram
---

# Тип источника Telegram

Источник _Telegram_ нужен для запуска трафика напрямую в Telegram.

Он поддерживает канал, публичный канал и Telegram-бота.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32585.png" alt="Настройка источника Telegram"><figcaption></figcaption></figure></div>

### Как это работает

Источник используется, когда пользователь должен попасть в канал или сразу в бота.

При включённом `Auto redirect` маршрут продолжается по логике кампании.

### Шаги

1. создайте кампанию и откройте **Sources**
2. добавьте источник с типом `Telegram`
3. выберите формат перехода
4. проверьте маршрут пользователя

### Форматы

#### **Telegram channel**

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32585.png" alt="Блок Telegram channel"><figcaption></figcaption></figure></div>

Подходит для закрытого или приватного канала.

Можно:

* вставить готовый `Invite link`
* создать ссылку через **Create link**

#### **Public Telegram**

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32586.png" alt="Блок Public Telegram"><figcaption></figcaption></figure></div>

Подходит для открытых каналов.

После настройки система создаёт `Internal invite ID`.

#### **Telegram Bot**

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32587.png" alt="Блок Telegram Bot"><figcaption></figcaption></figure></div>

Подходит для перелива трафика сразу в бота.

### Notes

{% hint style="info" %}
Используйте `Telegram channel` для invite link, `Public Telegram` для открытого канала и `Telegram Bot` для прямого входа в бот.
{% endhint %}

* `Auto redirect` перенаправляет пользователя по маршруту кампании

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
