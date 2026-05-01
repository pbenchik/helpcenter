---
description: Настройка источников трафика и передачи событий в Tracker Campaigns.
icon: road
---

# Sources - раздел campaign

> ### Sources - это раздел Campaigns для подключения и настройки источников трафика.

{% hint style="info" %}
С его помощью можно:

\- подключить новый источник трафика к кампании

\- выбрать тип источника через `Provider`

\- настроить передачу событий и конверсий

\- получить рабочую ссылку для запуска трафика

\- разделять трафик по платформам и гипотезам
{% endhint %}

### Видеоинструкция:

{% hint style="info" icon="road" %}
В видео показано, как работать с разделом Sources внутри Campaigns.

Подойдёт, если нужно быстро понять логику добавления источника, выбора `Provider`, заполнения полей источника и получения рабочей ссылки для трафика.

{% embed url="https://youtu.be/DvlCSUyDOdM" fullWidth="false" %}

**Таймкоды:**

* 00:11 - общий обзор раздела
* 00:20 - Facebook
* 00:30 - Google ADS
* 00:55 - Telegram
{% endhint %}

### Как работает Sources:

{% hint style="info" %}
Здесь определяется, откуда приходит трафик и как Tracker будет его обрабатывать.
{% endhint %}

{% hint style="info" %}
Именно на этом этапе создаётся рабочая ссылка для запуска рекламы и передачи событий.
{% endhint %}

### Как добавить источник:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Откройте раздел Sources**

    Перейдите в нужную кампанию и откройте вкладку `Sources`.

    Здесь находятся все подключённые источники трафика для выбранной кампании.

    <figure><img src="../../../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Нажмите Add source**

    После этого откроется форма для создания нового источника.

    <figure><img src="../../../../.gitbook/assets/Group 1437255925.png" alt=""><figcaption></figcaption></figure>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Заполните базовые поля**

    Укажите `Name` и `Provider`.

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Заполните параметры источника**

    Набор полей зависит от выбранного провайдера.

    Для рекламных платформ обычно нужны ID, токены, labels или другие служебные значения.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Нажмите Save**

    После этого система сгенерирует рабочую ссылку для трафика.
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Что настраивается в Sources</summary>

{% hint style="info" %}
В этом разделе обычно задают:

* название источника
* тип источника через поле `Provider`
* параметры конкретной платформы или канала
* логику передачи событий и конверсий
* рабочую ссылку для залива трафика
{% endhint %}

</details>

<details>

<summary>Какие поля есть в Sources</summary>

{% hint style="info" %}
Основные поля:

* `Name` — название источника внутри кампании
* `Provider` — тип источника трафика
* поля источника — дополнительные параметры под выбранного провайдера
* `Tracking link` — ссылка, которая создаётся после сохранения
{% endhint %}

{% hint style="info" %}
От выбранного `Provider` зависит набор доступных полей и логика передачи событий.
{% endhint %}

</details>

<details>

<summary>Какие типы источников доступны</summary>

{% hint style="info" %}
В Tracker доступны несколько типов источников.

Каждый из них решает свою задачу и требует свой набор параметров.
{% endhint %}

* [Тип источника Facebook](tip-istochnika-facebook.md) — для передачи событий и конверсий в Meta
* [Тип источника Google](tip-istochnika-google.md) — для работы с Google Ads
* [Тип источника Telegram](tip-istochnika-telegram.md) — для трафика в канал или бота
* [Тип источника Custom](tip-istochnika-custom.md) — для тестовых и нестандартных сценариев

</details>

<details>

<summary>Важные особенности</summary>

{% hint style="warning" %}
* после сохранения источника создаётся рабочая ссылка для запуска трафика
* одна кампания может использовать несколько источников
* это удобно для разных платформ, офферов и сценариев тестирования
{% endhint %}

</details>

### Где удобно использовать Sources:

{% hint style="success" %}
Sources удобно использовать, когда нужно:

* подключить новый источник трафика к кампании
* разделить трафик по платформам и гипотезам
* получить отдельную ссылку для запуска рекламы
* подготовить кампанию к аналитике и тестам
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
