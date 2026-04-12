---
icon: person-circle-exclamation
---

# Logs

> ### Logs - это раздел для проверки событий и postback в реальном времени.

{% hint style="info" %}
С его помощью можно:

* проверить, дошёл ли postback до системы
* увидеть, передался ли `clickid`
* понять, какой тип события пришёл
* проверить, ушло ли событие в рекламный источник
* найти ошибку обработки или отправки
{% endhint %}

### Как работает Logs:

{% hint style="info" %}
Раздел помогает понять, что система приняла и что отправила дальше.
{% endhint %}

{% hint style="info" %}
Здесь можно отдельно смотреть входящие postback и исходящие события по source.
{% endhint %}

### Как открыть Logs:

{% stepper %}
{% step %}
{% hint style="info" %}
**Откройте Tracker**
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Перейдите в Logs**

Откроется таблица событий с фильтрами.
{% endhint %}
{% endstep %}
{% endstepper %}

<details>

<summary>Postback logs</summary>

![Postback logs](<../../.gitbook/assets/Frame 2110.png>)

{% hint style="info" %}
`Postback logs` показывают события, которые приходят от партнёрских программ и продуктов.
{% endhint %}

{% hint style="info" %}
В таблице отображаются:

* `Status` — статус обработки postback
* `Postback` — название интеграции
* `Created at` — дата и время получения
* `Click ID` — идентификатор клика
* `Error` — ошибка обработки
* `URL` — полный URL полученного postback
{% endhint %}

{% hint style="info" %}
Эти данные помогают быстро понять, принят ли postback корректно.
{% endhint %}

</details>

<details>

<summary>Sources logs</summary>

![Sources logs](<../../.gitbook/assets/image 32596.png>)

{% hint style="info" %}
`Sources logs` показывают события, которые Tracker отправляет в рекламные источники.
{% endhint %}

{% hint style="info" %}
Например, в Facebook или другой подключённый source.
{% endhint %}

{% hint style="info" %}
В таблице отображаются:

* `Status` — статус отправки события
* `Source name` — название источника
* `Provider` — рекламный провайдер
* `Created at` — дата и время события
* `Event` — тип события
* `Click ID` — идентификатор клика
* `Error` — ошибка отправки
{% endhint %}

{% hint style="info" %}
Этот блок помогает проверить факт отправки и причину возможной ошибки.
{% endhint %}

</details>

<details>

<summary>Фильтры</summary>

{% hint style="info" %}
Чтобы быстрее найти нужное событие, используйте фильтры над таблицей.
{% endhint %}

{% hint style="info" %}
Доступны фильтры по:

* `Source` — названию источника
* `Event type` — типу события
* `Postback` — названию интеграции
{% endhint %}

{% hint style="info" %}
Используйте уникальные названия Sources.

Так нужные события находятся быстрее.
{% endhint %}

</details>

### Где удобно использовать Logs:

{% hint style="success" %}
Logs удобно использовать, когда нужно:

* проверить получение postback
* найти причину ошибки по событию
* убедиться, что `clickid` передался корректно
* проверить отправку события в рекламный источник
{% endhint %}

{% include "../../.gitbook/includes/na-glavnuyu.md" %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
