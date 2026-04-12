---
description: Настройка Telegram-источника для канала, публичного канала или бота.
icon: telegram
---

# Тип источника Telegram

> ### Telegram - это тип источника в Tracker для запуска трафика прямо в Telegram.

{% hint style="info" %}
С его помощью можно:

\- вести трафик сразу в Telegram

\- отправлять пользователя в закрытый или публичный канал

\- направлять трафик прямо в Telegram-бота

\- использовать auto redirect по логике кампании

*   Скриншот настройки источника Telegram:

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32585.png" alt="Настройка источника Telegram"><figcaption></figcaption></figure></div>
{% endhint %}

### Как работает источник Telegram:

{% hint style="info" %}
Источник подходит для сценариев, где пользователь должен перейти в канал или сразу попасть в бота.
{% endhint %}

{% hint style="info" %}
Источник поддерживает три варианта входа:

* закрытый канал
* публичный канал
* Telegram-бот
{% endhint %}

### Как настроить источник Telegram:

{% stepper %}
{% step %}
{% hint style="info" %}
**Создайте кампанию и откройте Sources**

Сначала в Tracker создаётся кампания.

Внутри неё определяется сценарий маршрутизации трафика.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Выберите тип источника Telegram**

После этого в источниках кампании добавляется тип `Telegram`.

Он нужен для запуска пользователя сразу в нужный Telegram-сценарий.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Выберите формат перехода**

Дальше определяется один из трёх вариантов: закрытый канал, публичный канал или бот.

От этого зависит, куда именно попадёт пользователь после клика.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Проверьте маршрут пользователя**

После перехода пользователь попадает в канал или бот.

При включённом `Auto redirect` можно продолжить маршрут по логике кампании.
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Что управляется в Telegram</summary>

{% hint style="info" %}
В этом источнике обычно настраивают:

* переход в закрытый канал по `Invite link`
* переход в публичный Telegram-канал
* перелив трафика сразу в Telegram-бота
* выдачу внутреннего идентификатора для публичного канала
* автоматический редирект после перехода
{% endhint %}

</details>

<details>

<summary>Telegram channel</summary>

*   Скриншот блока `Telegram channel`:

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32585.png" alt="Блок Telegram channel"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Этот вариант подходит для закрытого или приватного канала.
{% endhint %}

{% hint style="info" %}
Что можно сделать:

* вставить готовый `Invite link`
* создать ссылку через `Create link`
{% endhint %}

</details>

<details>

<summary>Public Telegram</summary>

*   Скриншот блока `Public Telegram`:

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32586.png" alt="Блок Public Telegram"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Этот вариант подходит для открытых каналов.
{% endhint %}

{% hint style="info" %}
После настройки система автоматически создаёт `Internal invite ID`.
{% endhint %}

</details>

<details>

<summary>Telegram Bot</summary>

*   Скриншот блока `Telegram Bot`:

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32587.png" alt="Блок Telegram Bot"><figcaption></figcaption></figure></div>

{% hint style="info" %}
Этот вариант подходит для перелива трафика сразу в Telegram-бота.
{% endhint %}

{% hint style="info" %}
Такой сценарий удобен, если пользователь должен сразу начать диалог.
{% endhint %}

</details>

<details>

<summary>Как выбрать вариант</summary>

{% hint style="info" %}
Используйте:

* `Telegram channel`, если нужен доступ по invite link
* `Public Telegram`, если канал открыт
* `Telegram Bot`, если трафик ведётся сразу в бота
{% endhint %}

</details>

<details>

<summary>Auto redirect</summary>

{% hint style="info" %}
Опция `Auto redirect` автоматически перенаправляет пользователя после перехода по ссылке источника.
{% endhint %}

{% hint style="info" %}
Направление редиректа зависит от настроек кампании.
{% endhint %}

</details>

### Где удобно использовать источник Telegram:

{% hint style="success" %}
Источник Telegram удобно использовать, когда нужно:

* вести трафик напрямую в Telegram
* приглашать пользователей в канал по ссылке
* сразу начинать диалог в Telegram-боте
* использовать Telegram как основную точку входа
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
