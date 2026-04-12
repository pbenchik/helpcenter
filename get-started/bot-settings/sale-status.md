---
icon: calendar
---

# Sale Status

> ### Sale Status - это инструмент для отслеживания этапа продажи, на котором находится лид.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2256 (1).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
С его помощью можно:

* визуально контролировать этапы продаж
* быстрее ориентироваться по лидам
* вручную и автоматически сегментировать диалоги
* видеть, на каком этапе воронки находится пользователь
{% endhint %}

### Как назначается Sale Status:

{% hint style="info" %}
Статус можно назначить двумя способами:

* вручную — через карточку клиента
* автоматически — через шаг Change Sale Status
{% endhint %}

### Как создать Sale Status:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Перейдите в раздел Sale Status**

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Нажмите Add new sale status**

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2212.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Укажите название статуса**

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
#### **Нажмите Save**
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Как работает Sale Status</summary>

{% hint style="info" %}
По своей логике Sale Status похож на теги.

Разница в том, что здесь статус привязан именно к этапу продажи.

Это делает работу с воронкой понятнее для команды.
{% endhint %}

</details>

<details>

<summary>Примеры статусов</summary>

{% hint style="info" %}
Например, можно использовать такие статусы:

* Первое касание
* Второе касание
* Третье касание
{% endhint %}

</details>

<details>

<summary>Где отображается Sale Status</summary>

{% hint style="info" %}
**После назначения статус отображается:**

* в карточке клиента
* в списке чатов — в правом верхнем углу иконки диалога

**Пример:**

Если установить пользователю статус «Третье касание», он будет:

* виден в его карточке
* отображаться рядом с диалогом в списке чатов
{% endhint %}

</details>

<details>

<summary>Автоматическое назначение</summary>

{% hint style="info" %}
Для автоматической смены статуса используйте шаг:

<a href="../konstruktor-flow-settings/tipy-shagov/changes/change-sale-status.md" class="button secondary">Change Sale Status</a>
{% endhint %}

</details>

<details>

<summary>Ограничения</summary>

{% hint style="warning" %}
**На текущий момент:**

* Sale Status нельзя использовать в Webhooks
* Sale Status нельзя передавать через Postback
{% endhint %}

{% hint style="info" %}
Этот инструмент предназначен исключительно для внутренней работы и визуального контроля этапов продаж.
{% endhint %}

</details>

### Где удобно использовать Sale Status:

{% hint style="success" %}
**Sale Status удобно использовать, когда нужно:**

* отмечать текущий этап продажи по каждому лиду
* разделять диалоги по стадии воронки
* помогать команде быстрее ориентироваться в CRM
* автоматически обновлять этап через сценарии
{% endhint %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
