---
icon: chart-simple-horizontal
---

# Chat status

Status — это параметр, который показывает текущее состояние диалога с клиентом.

### Как это работает

Статусы используются для понимания этапа общения, фильтрации пользователей в CRM и управления логикой обработки диалогов.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2137.png" alt=""><figcaption></figcaption></figure></div>

#### Где смотреть статусы

* откройте блок **Chat Status** в Messenger

### Auto

Диалог находится в автоматическом режиме.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2226.png" alt=""><figcaption></figcaption></figure></div>

#### Что это значит

* пользователь обрабатывается ИИ
* диалог движется по воронке автоматически

### Manual

Диалог переведён в ручную обработку.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2225.png" alt=""><figcaption></figcaption></figure></div>

#### Когда используется

* например, если пользователь отправил медиа
* см. [AI Recognition](../../bot-settings/automation-and-ai/ai-recognition.md)

#### Notes

* пуш-уведомления в этом статусе не отправляются

### Waiting

Бот ожидает ответа от пользователя.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2227.png" alt=""><figcaption></figcaption></figure></div>

#### Что это значит

* диалог не двигается дальше по воронке, пока пользователь не ответит

### Ignore

Этот статус присваивается автоматически, если пользователь находился в `Manual`.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2233.png" alt=""><figcaption></figcaption></figure></div>

### Blocked

В этом статусе исходящие сообщения можно отправлять, и пользователь будет их получать.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2232.png" alt=""><figcaption></figcaption></figure></div>

#### Ограничение

* если пользователь пишет, находясь в этом статусе, входящие сообщения не будут видны

### Error

Чаты с ошибками от ИИ.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2228.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="warning" %}
Если вы видите этот статус, сначала попробуйте перевести диалог в **Auto**. Если ошибка сохранится, обратитесь в технический чат.
{% endhint %}

### Stopped

Статус означает, что бот или личный аккаунт больше не может отправлять сообщения в чат.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2229.png" alt=""><figcaption></figcaption></figure></div>

#### Примеры

* пользователь заблокировал бота или личный аккаунт
* Telegram вернул ошибку, например из-за лимитов или ограничений канала

### Finished

Диалог полностью завершён.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2231.png" alt=""><figcaption></figcaption></figure></div>

#### Что это значит

* ИИ больше не отвечает
* пуш-уведомления прекращаются

### Связанные страницы

* [Messenger](./)
* [Inbox Control](inbox-control.md)
* [Custom Filters](custom-filters/)

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
