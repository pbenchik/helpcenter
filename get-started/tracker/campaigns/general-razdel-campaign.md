---
icon: head-side-gear
---

# General - раздел campaign

> ### General - это раздел Campaigns для настройки маршрута пользователя после клика.

{% hint style="info" %}
С его помощью можно:

\- определить, куда попадёт пользователь после клика

\- выбрать Telegram-точку входа

\- задать стартовый Flow и Step

\- назначить DM bot для дальнейшей обработки лида
{% endhint %}

### Видеоинструкция:

{% hint style="info" icon="head-side-gear" %}
В видео показано, как заполнить поля раздела General внутри Campaigns.

Подойдёт, если нужно быстро понять логику полей `Campaign traffic type`, `Invite Bot / Bot`, `Channel`, `Start Flow`, `Start Step` и `DM bot`.

{% embed url="https://youtu.be/hYwNhUlfXJ0" fullWidth="false" %}
{% endhint %}

### Как работает General:

{% hint style="info" %}
Здесь выбирается, куда попадёт пользователь и какой сценарий запустится дальше.
{% endhint %}

{% hint style="info" %}
Именно на этом этапе определяется логика перехода в Telegram.
{% endhint %}

### Как заполнить General:

{% stepper %}
{% step %}
{% hint style="info" %}
**Выберите маршрут пользователя**

Сначала определяется тип трафика кампании.

Система должна понимать, ведёте вы пользователя в канал или сразу в бота.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Подключите приёмщик трафика**

Затем выбираются Invite Bot, Bot и при необходимости канал.

Так задаётся точка входа пользователя в Telegram.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Определите сценарий взаимодействия**

После этого выбираются Flow, Step и DM bot.

Так система понимает, какой сценарий запускать и где обрабатывать лид дальше.
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Что настраивается в General</summary>

{% hint style="info" %}
В этом разделе обычно задают:

* тип маршрута пользователя: в канал или в бота
* Invite Bot или Bot для обработки перехода
* Telegram-канал для сценария `Channel`
* Flow и Step для первого запуска
* DM bot для дальнейшей обработки лида
{% endhint %}

</details>

<details>

<summary>Campaign traffic type</summary>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
`Campaign traffic type` определяет тип маршрута пользователя.
{% endhint %}

{% hint style="info" %}
Доступны варианты:

* `Channel` — пользователь сначала попадает в Telegram-канал
* `Bot` — пользователь сразу попадает в Telegram-бота
{% endhint %}

</details>

<details>

<summary>Invite Bot / Bot</summary>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
`Invite Bot / Bot` — бот, который используется для входа пользователя в сценарий.
{% endhint %}

{% hint style="info" %}
* `Invite Bot` нужен для типа `Channel`
* `Bot` нужен для типа `Bot`
{% endhint %}

</details>

<details>

<summary>Channel</summary>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
`Channel` — Telegram-канал, в который попадёт пользователь.
{% endhint %}

{% hint style="info" %}
Это поле доступно только для типа `Channel`.
{% endhint %}

</details>

<details>

<summary>Start Flow и Start Step</summary>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
`Start Flow` — Flow, который запускается после перехода пользователя.

`Start Step` — первый Step выбранного Flow.
{% endhint %}

{% hint style="info" %}
Эти поля позволяют запускать пользователя с нужного этапа сценария.
{% endhint %}

</details>

<details>

<summary>DM bot</summary>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
`DM bot` — бот или Telegram-аккаунт для обработки лида и получения события `contact`.
{% endhint %}

</details>

<details>

<summary>Start Flow и Start Step для DM bot</summary>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Это отдельный сценарий для DM bot.
{% endhint %}

{% hint style="info" %}
Если Invite Bot и DM bot совпадают, заполнять это обычно не нужно.
{% endhint %}

</details>

<details>

<summary>Важные особенности</summary>

{% hint style="warning" %}
Для сценария `Channel` Invite Bot должен быть активирован в системе.

Также его нужно добавить администратором канала и выдать право на принятие заявок.

Если заявки принимает другой бот, события не будут фиксироваться в Tracker.
{% endhint %}

</details>

<details>

<summary>Что находится рядом</summary>

{% hint style="info" %}
Следующие этапы настройки Campaigns:

* [Information](information-razdel-campaign.md) - базовая информация о кампании
* [Sources](sources-razdel-campaign/) - выбор и настройка источника трафика
* [Auto actions](auto-actions-razdel-campaing.md) - автоматические действия внутри кампании
* [Parameters](parameters-razdel-campaing.md) - параметры передачи данных
* [Test](test-razdel-campaign.md) - проверка кампании перед запуском
{% endhint %}

</details>

### Где удобно использовать General:

{% hint style="success" %}
General удобно использовать, когда нужно:

* определить маршрут пользователя после клика
* связать кампанию с ботом или каналом
* запустить пользователя с нужного Flow и Step
* подготовить DM-обработку лида
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
