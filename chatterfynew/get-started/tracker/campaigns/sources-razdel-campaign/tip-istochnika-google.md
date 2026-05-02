---
description: Настройка источника Google для передачи конверсий из Tracker в Google Ads.
icon: google-plus
---

# Тип источника Google

Источник _Google_ нужен для передачи конверсий из Tracker в Google Ads.

Он связывает события кампании с `Conversion ID` и `Conversion labels`.

<div data-with-frame="true"><img src="../../../../.gitbook/assets/image 32584.png" alt=""></div>

### Как это работает

Во время настройки вы задаёте данные конверсии и labels для нужных событий.

Для каждого события можно использовать отдельный label.

### Шаги

1. создайте новый источник с `Provider = Google`
2. укажите `Conversion ID`
3. заполните `Conversion labels` для нужных событий
4. проверьте совпадение labels с Google Ads
5. при необходимости включите `Auto redirect`

### Поля

* **Conversion ID** — идентификатор конверсии
* **Conversion labels** — labels для событий кампании
* **Auto redirect** — автоматический редирект по маршруту кампании

### Notes

{% hint style="info" %}
Используйте этот тип источника, если трафик закупается в Google Ads и нужно передавать конверсии обратно в рекламный кабинет.
{% endhint %}

* Маршрут `Auto redirect` берётся из настроек кампании

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
