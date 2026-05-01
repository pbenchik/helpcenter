---
icon: align-justify
---

# Webhooks & API

> ### **Webhooks & API** помогают передавать данные в бота и управлять диалогом из внешних сервисов.

{% hint style="info" %}
{% embed url="https://youtu.be/zuvJjU8nGXw" %}

**Через Webhooks & API можно:**

* отправлять данные по конкретному пользователю
* обновлять логику диалога в реальном времени
* использовать переданные данные в сообщениях и ссылках
* собирать данные еще до первого входа пользователя в бот
{% endhint %}

### Важно перед началом:

{% hint style="warning" %}
**Перед настройкой Webhooks & API важно учесть:**

* для одного бота можно создать несколько webhook-ссылок
* у каждого бота свои уникальные ссылки
* одну ссылку удобно использовать под один внешний сервис
* параметры передаются через GET-запрос
{% endhint %}

### Основные возможности:

{% hint style="info" %}
**С помощью Webhooks & API вы можете:**

* переводить пользователя на нужный шаг
* менять статус диалога
* сохранять значения в кастомные поля
* подставлять эти данные в сообщения и ссылки
{% endhint %}

### Подробнее:

<details>

<summary>Структура работы</summary>

{% hint style="info" %}
Основные части:

* создание webhook-ссылки
* работа с параметром chatId
* управление шагом и статусом
* передача данных в поля
* использование переменных в боте
{% endhint %}

</details>

<details>

<summary>Создание webhook-ссылки</summary>

{% hint style="info" %}
**Чтобы начать работу, сначала создайте уникальную ссылку.**

Что нужно сделать:

* открыть нужного бота
* перейти в Bot Settings
*

```
<div data-with-frame="true"><figure><img src="/files/8FL8Bsg7fL2eGwAFWWVr" alt=""><figcaption></figcaption></figure></div>
```

* открыть раздел Webhooks & API
*

```
<figure><img src="/files/hIS9HGkbTbb5ZNQu9tqo" alt=""><figcaption></figcaption></figure>
```

* нажать Add Webhook
*

```
<figure><img src="/files/xY7j9gIKQBVM3P14xFOt" alt=""><figcaption></figcaption></figure>
```

* нажать Save внизу страницы

После этого система создаст уникальную ссылку.

**Пример ссылки:**

`https://app.chatterfy.ai/api/bots/webhooks/<POSTBACK_ID>/updateDialog`

**Пример с реальным ID:**

`https://app.chatterfy.ai/api/bots/webhooks/55833627-242e-4061-9b0a-30da3e9cf7d4/updateDialog`
{% endhint %}

</details>

<details>

<summary>Работа с конкретным пользователем</summary>

{% hint style="info" %}
**Для обращения к конкретному пользователю используется параметр `chatId`.**

Пример:

`chatId=1227280`

Где `1227280` — это Telegram Chat ID пользователя.
{% endhint %}

{% hint style="warning" %}
**Данные можно отправлять по `chatId` даже до первого входа пользователя в бот.**

В этом случае:

* данные сохранятся заранее
* после первого входа они уже будут в карточке клиента
{% endhint %}

</details>

<details>

<summary>Управление диалогом через Webhook</summary>

{% hint style="info" %}
**Через ссылку можно передавать основные параметры:**

* `stepId` — переключение шага
* `status` — изменение статуса диалога
* `fields.*` — передача кастомных данных
{% endhint %}

</details>

<details>

<summary>Step ID</summary>

{% hint style="info" %}
**Чтобы перевести пользователя на конкретный шаг, передайте:**

* `chatId` — ID пользователя
* `stepId` — ID шага

Пример:

`https://app.chatterfy.ai/api/bots/webhooks/<POSTBACK_ID>/updateDialog?chatId=1227280&stepId=046050f6-38f6-4b18-b9fa-e6582f5352d0`
{% endhint %}

</details>

<details>

<summary>Status</summary>

{% hint style="info" %}
**Через `status` можно менять режим обработки диалога.**

Например:

* `auto` — автоматическая обработка
* `manual` — передача оператору
* `blocked` — блокировка диалога

Пример:

`...&chatId=1227280&status=manual`
{% endhint %}

</details>

<details>

<summary>Fields</summary>

{% hint style="info" %}
**Через Webhook можно сохранять любые данные в карточке клиента.**

Базовый формат:

`fields.anyKey=value`

Примеры:

* сохранение `refId`
* запись баланса пользователя

Пример 1:

`...&chatId=1227280&refId=12345`

Пример 2:

`...&chatId=1227280&userBalance=5000`
{% endhint %}

</details>

<details>

<summary>Использование данных в сообщениях и ссылках</summary>

{% hint style="info" %}
**Сохраненные значения можно использовать через переменные.**

Пример переменной:

`{{fields.refId}}`

Пример ссылки:

`https://some.service.com/signup?refId={{fields.refId}}`
{% endhint %}

</details>

<details>

<summary>Доступные переменные</summary>

{% hint style="info" %}
**В боте можно использовать несколько типов переменных.**

**Системные:**

* `{{chatId}}` — Telegram ID
* `{{username}}` — username
* `{{name}}` — имя пользователя
* `{{createdAt}}` — дата создания диалога

**Кастомные поля:**

* `{{fields.key}}` — данные, переданные через Webhook

**Трекер-параметры:**

* `{{tracker.key}}` — любое значение из трекера
* `{{tracker.clickid}}` — уникальный ID пользователя
{% endhint %}

</details>

<details>

<summary>Примеры использования</summary>

{% hint style="info" %}
**Webhooks & API часто используют в таких сценариях:**

* передача UTM-параметров
* генерация партнёрских ссылок
* персонализация сообщений
{% endhint %}

{% hint style="info" %}
**Работа с UTM-параметрами**

Если пользователь пришел с параметром:

`ad_name=test`

Его можно использовать так:

`https://some.service.com/signup?ad_name={{tracker.ad_name}}`

**Генерация партнёрской ссылки**

`https://partner.com/signup?sub1={{tracker.clickid}}`

Если `clickid = test123`, пользователь получит:

`https://partner.com/signup?sub1=test123`

**Персонализация сообщений**

Пример:

`Hello, {{name}}`
{% endhint %}

{% hint style="warning" %}
**Если пользователь пришел не через трекер, tracker-данных у него не будет.**

Например, это бывает, если он просто нажал `Start` в боте.
{% endhint %}

</details>

<details>

<summary>Проверка пользователя во внешней системе</summary>

{% hint style="info" %}
**Типовой сценарий работы:**

1. вы отправляете `chatId` во внешний сервис
2. на своей стороне проверяете пользователя
3. в ответ отправляете Webhook обратно в бота

Пример первого запроса:

`https://yourservice.com?chatId={{chatId}}`

Пример обратного запроса:

`https://app.chatterfy.ai/api/bots/webhooks/<POSTBACK_ID>/updateDialog?chatId=123&stepId=STEP_ID&status=auto`
{% endhint %}

</details>

### Важная логика работы:

{% hint style="warning" %}
* **Webhook работает по уникальной ссылке конкретного бота**
* без `chatId` нельзя управлять конкретным пользователем
* через Webhook можно заранее записывать данные в карточку
* tracker-переменные доступны только если пользователь пришел через трекер
{% endhint %}

### Когда использовать Webhooks & API:

{% hint style="success" %}
**Используйте этот инструмент, когда нужно:**

* передавать данные из внешних систем в бота
* управлять логикой диалога вне платформы
* сохранять значения в карточку клиента
* строить интеграции с CRM, лендингами и трекерами
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
