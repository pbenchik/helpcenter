---
icon: shoe-prints
---

# Типы Шагов

> ### Step - это отдельное действие, которое выполняется в диалоге с пользователем.
>
> ### В конструкторе Chatterfy каждый Flow состоит из шагов.

{% hint style="info" %}
С помощью шагов вы можете:

* отправлять сообщения
* обрабатывать ответы пользователя
* управлять логикой сценария
* работать с тегами и операторами
* отправлять события и данные во внешние сервисы
{% endhint %}

{% hint style="info" %}
Все шаги в конструкторе разделены на несколько категорий.

Это упрощает сборку сценария и помогает быстрее находить нужные действия.
{% endhint %}

<details>

<summary>Коммуникация</summary>

{% hint style="info" %}
<mark style="color:orange;">Коммуникация</mark> - шаги для взаимодействия с пользователем.

*

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (3).jpeg" alt=""><figcaption></figcaption></figure></div>

В эту категорию входят:

* Send message - отправка текста, медиа и документов
* AI Reply - генерация ответов с помощью ИИ
* Custom push - отправка пушей для напоминаний и догрева
{% endhint %}

</details>

<details>

<summary>Изменения</summary>

{% hint style="info" %}
<mark style="color:orange;">Изменения</mark> - шаги, которые меняют состояние диалога или пользователя.

*

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (4).jpeg" alt=""><figcaption></figcaption></figure></div>

В эту категорию входят:

* Change tag - добавление или удаление тегов
* Change flow - перевод пользователя в другой flow
* Operator - назначение или удаление оператора
* Change sale status - изменение статуса сделки
{% endhint %}

</details>

<details>

<summary>Условия и логика</summary>

{% hint style="info" %}
<mark style="color:orange;">Условия и логика</mark> - шаги для управления переходами внутри сценария.

*

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (5).jpeg" alt=""><figcaption></figcaption></figure></div>

В эту категорию входят:

* Condition - условия перехода по тегам, полям и данным трекера
* A/B router - распределение пользователей по разным веткам
* Delay - задержка перед следующим шагом
{% endhint %}

</details>

<details>

<summary>Трекинг и интеграции</summary>

{% hint style="info" %}
<mark style="color:orange;">Трекинг и интеграции</mark> - шаги для передачи данных.

*

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (6).jpeg" alt=""><figcaption></figcaption></figure></div>

В эту категорию входят:

* Send event - отправка событий: subscribe, registration, sale, resale
* Webhook - отправка данных во внешние сервисы
{% endhint %}

</details>

<details>

<summary>Дополнительно</summary>

{% hint style="info" %}
<mark style="color:orange;">Дополнительно</mark> - служебные шаги для удобства работы со сценарием.

*

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (7).jpeg" alt=""><figcaption></figcaption></figure></div>

В эту категорию входит:

* Note - комментарий внутри flow, который не влияет на логику
{% endhint %}

</details>

### Принцип работы:

{% hint style="info" %}
Все шаги в сценарии связаны между собой и выполняются последовательно.

1. Пользователь попадает в шаг.
2. Шаг выполняет нужное действие.
3. Пользователь переходит на следующий шаг по заданной логике.
{% endhint %}

### Важно учитывать:

{% hint style="info" %}
* Каждый шаг выполняет одну конкретную задачу.
* Логика сценария строится через связь шагов между собой.
* Некоторые шаги, например AI Reply и Condition, влияют на переходы по воронке.
* Delay может временно блокировать выполнение следующего действия.
{% endhint %}

### Когда использовать разные типы шагов:

{% hint style="info" %}
* Для общения - Send message и AI Reply
* Для логики - Condition и A/B router
* Для сегментации - Change tag и Change sale status
* Для маршрутизации - Change flow
* Для интеграций - Webhook и Send event
* Для таймингов - Delay
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
