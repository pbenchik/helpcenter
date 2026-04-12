---
icon: globe-pointer
---

# Webhook

> ### Webhook - это шаг, который позволяет отправлять данные пользователя во внешние сервисы по URL.

{% hint style="info" %}
{% embed url="https://youtu.be/zuvJjU8nGXw" %}

Используется для:

* передачи данных во внешние системы
* интеграции с базами данных и другими сервисами
* автоматизации обработки лидов
* передачи параметров пользователя
{% endhint %}

### Важно перед началом:

{% hint style="warning" %}
Необходимо понимать, куда будут отправляться данные (URL) и в каком формате их ожидает принимающая сторона.

Webhook отправляет данные наружу.\
Для приёма данных в Chatterfy используется отдельный механизм (Bot Settings -> Webhook / API).
{% endhint %}

### Основные возможности:

{% hint style="info" %}
С помощью Webhook вы можете:

* отправлять данные пользователя во внешние сервисы
* передавать параметры (id, username, clickid и т.д.)
* настраивать GET и POST запросы
* формировать собственное тело запроса (Body)
{% endhint %}

### Структура шага:

{% hint style="info" %}
**Шаг состоит из 2 блоков:**

* Settings (Настройки)
* Webhook (Настройки запроса)
{% endhint %}

### Важно:

<details>

<summary>1. Settings (Настройки)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (15).png" alt=""><figcaption></figcaption></figure></div>

**Title**\
<mark style="color:$primary;">Название шага.</mark>\
<mark style="color:$primary;">Используется для удобной навигации внутри flow.</mark>

***

**Delay**\
<mark style="color:$primary;">Задержка перед выполнением шага.</mark>\
<mark style="color:$primary;">Во время задержки:</mark>

* <mark style="color:$primary;">сообщения пользователя игнорируются</mark>
* <mark style="color:$primary;">действие не выполняется</mark>

***

**Finish Status**\
<mark style="color:$primary;">Статус диалога после выполнения шага.</mark>\
<mark style="color:$primary;">Варианты:</mark>

* <mark style="color:$primary;">nothing - переход к следующему шагу</mark>
* <mark style="color:$primary;">auto - автоматическое продолжение диалога</mark>
* <mark style="color:$primary;">waiting - ожидание ответа пользователя</mark>
* <mark style="color:$primary;">manual - перевод в ручной режим</mark>
* <mark style="color:$primary;">blocked - блокировка диалога</mark>
* <mark style="color:$primary;">finished - завершение диалога</mark>

***

**Hide keyboard**\
<mark style="color:$primary;">Скрывает клавиатуру из предыдущего шага.</mark>

***

**Is start step of flow**\
<mark style="color:$primary;">Отмечает шаг как стартовый.</mark>

***

<mark style="color:$primary;">Отключает автоматический переход на следующий шаг.</mark>

<mark style="color:$primary;">Используется в связке со статусом waiting.</mark>

<mark style="color:$primary;">Если опция включена:</mark>

* <mark style="color:$primary;">шаг не переключится автоматически</mark>
* <mark style="color:$primary;">система останется на текущем шаге</mark>
* <mark style="color:$primary;">будет ожидать ответ пользователя</mark>
{% endhint %}



</details>

<details>

<summary>2. Webhook (Настройки запроса)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (14).png" alt=""><figcaption></figcaption></figure></div>

URL - ссылка, на которую будет отправлен запрос.

Method - тип запроса:

* GET - данные передаются через URL
* POST - данные передаются в теле запроса
{% endhint %}



</details>

<details>

<summary>Body (для POST)</summary>

{% hint style="info" %}
*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (16).png" alt=""><figcaption></figcaption></figure>
* Поле для формирования тела запроса.
* В теле запроса можно использовать переменные пользователя и системы.

Пример:

<mark style="color:yellow;">{"username": "{username}","chat\_id": "{chatId}","clickid": "{tracker.clickid}"}</mark>
{% endhint %}



</details>

<details>

<summary>Available variables</summary>

{% hint style="info" %}
Доступные переменные для отправки:

* {username} - имя пользователя в Telegram (текстовое значение)
* {chatId} - Chat ID пользователя в Telegram (числовое значение)
* {stepKey} - ключ шага, на котором находится пользователь (текстовое значение)
* {createdAt} - время начала диалога (формат: 2024-03-10T17:49:32.806Z)

***

**Также доступны динамические переменные:**

* {KEYCUSTOMFIELD} - значение кастомного поля (замените KEYCUSTOMFIELD на ключ вашего поля из Bot Settings → Custom Fields)
* {tracker.KEYTRACKERFIELD} - значение поля из трекера (например: {tracker.clickid})
{% endhint %}



</details>

<details>

<summary>Пример использования</summary>

{% hint style="info" %}
Сценарий 1: отправка данных в трекер (например, Keitaro)

Webhook → GET

Пример: https://keitaro.yoursite.com/25123a/postback?subid={tracker.clickid}\&username={username}\&chatid={chatId}\&startdialogue={createdAt}\
Где:

* <mark style="color:yellow;">subid={tracker.clickid}</mark> - clickid пользователя
* <mark style="color:yellow;">username={username}</mark> - имя пользователя
* <mark style="color:yellow;">chatid={chatId}</mark> - Telegram ID
* <mark style="color:yellow;">startdialogue={createdAt}</mark> - время начала диалога

***

Сценарий 2: отправка параметров в базу данных

Webhook → POST

Body: <mark style="color:yellow;">{"username": "{username}","chat\_id": "{chatId}"}</mark>
{% endhint %}



</details>

### Важная логика работы:

{% hint style="warning" %}
Запрос отправляется сразу после выполнения шага\
Данные подставляются автоматически через переменные\
Используется для передачи данных во внешние системы

Корректность отправки можно проверить в разделе Logs → Webhooks
{% endhint %}

### Когда использовать Webhook:

{% hint style="success" %}
Используйте этот шаг, когда нужно:

* передать данные во внешний сервис
* отправить данные пользователя в систему аналитики
* автоматизировать обработку лидов
* интегрировать Chatterfy с другими сервисами
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
