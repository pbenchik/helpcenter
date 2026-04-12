---
description: Настройка источника Facebook для передачи событий и конверсий из Tracker.
icon: facebook
---

# Тип источника Facebook

> ### Facebook - это тип источника для передачи событий из Tracker в Meta.

{% hint style="info" %}
С его помощью можно:

\- отправлять события из Tracker в Meta

\- передавать конверсии по пользователям

\- сопоставлять события Tracker с событиями Facebook

\- использовать стоимость и валюту в передаче Purchase

*   Скриншот настройки источника Facebook:

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32582.png" alt="Настройка источника Facebook"><figcaption></figcaption></figure></div>
{% endhint %}

### Как работает источник Facebook:

{% hint style="info" %}
Источник Facebook используется, когда нужно отправлять события из Tracker в Meta Ads.
{% endhint %}

{% hint style="info" %}
На этом этапе задаются данные пикселя и правила сопоставления событий.
{% endhint %}

### Как настроить источник Facebook:

{% stepper %}
{% step %}
{% hint style="info" %}
**Выберите тип источника Facebook**

Создайте новый источник и укажите `Provider = Facebook`.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Заполните основные поля**

Укажите:

* `Pixel ID`
* `Pixel Access Token`
* `Proxy` — при необходимости
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Настройте Mapping events**

Сопоставьте события Tracker с событиями Facebook.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Проверьте данные перед запуском**

Убедитесь, что `Pixel ID`, `Access Token` и правила событий заполнены корректно.
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Какие поля нужно заполнить</summary>

{% hint style="info" %}
При настройке укажите:

* `Pixel ID`
* `Pixel Access Token`
* `Proxy` — необязательно
{% endhint %}

{% hint style="info" %}
Если прокси не требуется, поле можно оставить пустым.
{% endhint %}

</details>

<details>

<summary>Mapping events</summary>

*   Скриншот блока `Mapping events`:

    <div data-with-frame="true"><img src="../../../../.gitbook/assets/unknown (32).png" alt="Блок Mapping events"></div>

{% hint style="info" %}
Через `Mapping events` вы сопоставляете события Tracker с событиями Facebook.
{% endhint %}

{% hint style="info" %}
Стандартное соответствие:

* `page view` → `ViewContent`
* `click` → `Lead`
* `subscribe` → `Subscribe`
* `contact` → `Contact`
* `registration` → `CompleteRegistration`
* `sale` → `Purchase`
{% endhint %}

{% hint style="info" %}
Дополнительно передаются параметры:

* `value` → `{cost}`
* `currency` → `{currency}`
{% endhint %}

{% hint style="info" %}
При необходимости можно добавить собственные правила через `Add event`.
{% endhint %}

</details>

<details>

<summary>Что важно проверить</summary>

{% hint style="warning" %}
Перед запуском трафика убедитесь, что:

* введён корректный `Pixel ID`
* `Access Token` активен
* нужные события сопоставлены правильно
{% endhint %}

</details>

### Где удобно использовать источник Facebook:

{% hint style="success" %}
Источник Facebook удобно использовать, когда нужно:

* передавать конверсии в Meta Ads
* связывать события Tracker с пикселем Facebook
* анализировать эффективность рекламы по событиям
* отправлять стоимость и валюту для покупки
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
