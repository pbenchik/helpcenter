---
description: Настройка источника Facebook для передачи событий и конверсий из Tracker.
icon: facebook
---

# Тип источника Facebook

Источник _Facebook_ нужен для передачи событий из Tracker в Meta.

Он связывает события кампании с пикселем Facebook.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image 32582.png" alt="Настройка источника Facebook"><figcaption></figcaption></figure></div>

### Как это работает

Во время настройки вы указываете данные пикселя и правила сопоставления событий.

После этого Tracker может отправлять события и конверсии в Meta Ads.

### Шаги

1. создайте новый источник с `Provider = Facebook`
2. укажите `Pixel ID`, `Pixel Access Token` и при необходимости `Proxy`
3. настройте `Mapping events`
4. проверьте данные перед запуском

### Mapping events

<div data-with-frame="true"><img src="../../../../.gitbook/assets/unknown (32).png" alt="Блок Mapping events"></div>

Стандартное соответствие:

* `page view` → `ViewContent`
* `click` → `Lead`
* `subscribe` → `Subscribe`
* `contact` → `Contact`
* `registration` → `CompleteRegistration`
* `sale` → `Purchase`

Дополнительно передаются:

* `value` → `{cost}`
* `currency` → `{currency}`

### Notes

{% hint style="warning" %}
Перед запуском проверьте корректность `Pixel ID`, активность токена и сопоставление событий.
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
