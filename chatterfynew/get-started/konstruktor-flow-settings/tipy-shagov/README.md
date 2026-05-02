---
icon: shoe-prints
---

# Типы Шагов

_Step_ — это отдельное действие внутри диалога с пользователем.

В конструкторе каждый _flow_ состоит из шагов.

### Что можно делать шагами

* отправлять сообщения
* обрабатывать ответы пользователя
* управлять логикой сценария
* работать с тегами и операторами
* отправлять события и данные во внешние сервисы

### Категории шагов

#### Communication

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (3).jpeg" alt=""><figcaption></figcaption></figure></div>

* [Send message](communication/send-message.md)
* [AI Reply](communication/ai-reply.md)
* [Custom push](communication/custom-push.md)

#### Changes

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (4).jpeg" alt=""><figcaption></figcaption></figure></div>

* [Change tag](changes/change-tag.md)
* [Change flow](changes/change-flow.md)
* [Operator](changes/operator.md)
* [Change sale status](changes/change-sale-status.md)

#### Terms

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (5).jpeg" alt=""><figcaption></figcaption></figure></div>

* [Condition](terms/condition.md)
* [A/B router](terms/a-b-router.md)
* [Delay](terms/delay.md)

#### Tracking

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (6).jpeg" alt=""><figcaption></figcaption></figure></div>

* [Send event](tracking/send-event.md)
* [Webhook](tracking/webhook.md)

#### Additional

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (7).jpeg" alt=""><figcaption></figcaption></figure></div>

* [Note](additional/note.md)

### Как это работает

1. Пользователь попадает в шаг.
2. Шаг выполняет нужное действие.
3. Пользователь переходит на следующий шаг по заданной логике.

### Notes

{% hint style="info" %}
Каждый шаг выполняет одну конкретную задачу.

Шаги вроде **AI Reply**, **Condition** и **Delay** сильнее влияют на логику переходов.
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
