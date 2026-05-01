---
description: Настройка источника Google для передачи конверсий из Tracker в Google Ads.
icon: google-plus
---

# Тип источника Google

> ### Google - это тип источника для передачи конверсий из Tracker в Google Ads.

{% hint style="info" %}
С его помощью можно:

\- передавать конверсии обратно в Google Ads

\- связывать события Tracker с conversion labels

\- отслеживать результат по разным событиям кампании

\- автоматически перенаправлять пользователя по маршруту кампании

*   Скриншот настройки источника Google:

    <div data-with-frame="true"><img src="../../../../.gitbook/assets/image 32584.png" alt=""></div>
{% endhint %}

### Как работает источник Google:

{% hint style="info" %}
Источник Google используется, когда трафик закупается в Google Ads и нужно передавать конверсии обратно в рекламный кабинет.
{% endhint %}

{% hint style="info" %}
На этом этапе задаются данные конверсии и правила передачи событий.
{% endhint %}

### Как настроить источник Google:

{% stepper %}
{% step %}
{% hint style="info" %}
**Выберите тип источника Google**

Создайте новый источник и укажите `Provider = Google`.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Заполните основные поля**

Укажите:

* <mark style="color:$primary;">`Conversion ID`</mark>
* <mark style="color:$primary;">`Conversion labels`</mark> <mark style="color:$primary;">для нужных событий</mark>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Проверьте соответствие labels**

Убедитесь, что labels совпадают с теми, которые созданы в Google Ads.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**При необходимости включите Auto redirect**

Так пользователь будет автоматически перенаправляться по маршруту кампании.
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Когда использовать</summary>

{% hint style="info" %}
Выбирайте этот источник, если:

* <mark style="color:$primary;">трафик закупается в Google Ads</mark>
* <mark style="color:$primary;">нужно передавать конверсии обратно в рекламный кабинет</mark>
* <mark style="color:$primary;">вы отслеживаете результат по разным событиям кампании</mark>
{% endhint %}

</details>

<details>

<summary>Что нужно заполнить</summary>

{% hint style="info" %}
При настройке укажите:

* <mark style="color:$primary;">`Conversion ID`</mark>
* <mark style="color:$primary;">`Conversion labels`</mark> <mark style="color:$primary;">для нужных событий</mark>
{% endhint %}

</details>

<details>

<summary>Как работает передача</summary>

{% hint style="info" %}
Для каждого события можно указать свой label.

Это позволяет отдельно отслеживать клики, регистрации и другие конверсии.
{% endhint %}

{% hint style="info" %}
Проверьте, что labels соответствуют тем, которые созданы в Google Ads.
{% endhint %}

</details>

<details>

<summary>Auto redirect</summary>

{% hint style="info" %}
Опция `Auto redirect` автоматически перенаправляет пользователя после перехода по ссылке источника.
{% endhint %}

{% hint style="info" %}
Маршрут перенаправления берётся из настроек кампании.
{% endhint %}

</details>

### Где удобно использовать источник Google:

{% hint style="success" %}
Источник Google удобно использовать, когда нужно:

* передавать конверсии в Google Ads
* разделять эффективность по типам событий
* связывать результаты рекламы с данными Tracker
* автоматически перенаправлять пользователя по маршруту кампании
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
