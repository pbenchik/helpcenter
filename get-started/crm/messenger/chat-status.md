---
icon: chart-simple-horizontal
---

# Chat status

> ### Status - это параметр, который показывает текущее состояние диалога с клиентом.

{% hint style="info" %}
Статусы используются для:

* понимания этапа общения
* фильтрации пользователей в CRM
* управления логикой обработки диалогов
*

    <figure><img src="../../../.gitbook/assets/Frame 2137.png" alt=""><figcaption></figcaption></figure>

<mark style="color:$warning;">**Где настраиваются статусы?**</mark>

Чтобы открыть список статусов:

* Найдите выдвигающийся раздел Chat Status
{% endhint %}

### **Auto**:

{% hint style="info" %}
Диалог находится в автоматическом режиме.

Пользователь обрабатывается ИИ и движется по воронке.

*

    <figure><img src="../../../.gitbook/assets/Frame 2226.png" alt=""><figcaption></figcaption></figure>
{% endhint %}

### Manual:

{% hint style="info" %}
Диалог переведён в ручную обработку.

*

    <figure><img src="../../../.gitbook/assets/Frame 2225.png" alt=""><figcaption></figcaption></figure>

Например:

пользователь отправил медиа и был переведён в Manual - см. [AI Recognition](../../bot-settings/automation-and-ai/ai-recognition.md)

\*пуш-уведомления в этом статусе не отправляются
{% endhint %}

### **Waiting**:

{% hint style="info" %}
Бот ожидает ответа от пользователя.

*

    <figure><img src="../../../.gitbook/assets/Frame 2227.png" alt=""><figcaption></figcaption></figure>

Диалог не будет двигаться дальше по воронке, пока пользователь не ответит каким-либо сообщением..
{% endhint %}

### **Ignore**:

{% hint style="info" %}
*

    <figure><img src="../../../.gitbook/assets/Frame 2233.png" alt=""><figcaption></figcaption></figure>

Статус присваивается автоматически, если пользователь находился в Manual более 10 минут
{% endhint %}

### **Blocked**:

{% hint style="info" %}
*

    <figure><img src="../../../.gitbook/assets/Frame 2232.png" alt=""><figcaption></figcaption></figure>
* Пользователь заблокировал бота.
* Отправка сообщений становится невозможной.
{% endhint %}

### **Error**:

{% hint style="info" %}
* Чаты с ошибками от ИИ.
*

    <figure><img src="../../../.gitbook/assets/Frame 2228.png" alt=""><figcaption></figcaption></figure>
* Если вы сталкиваетесь с этим статусом - сначала попробуйте перевести в статус Auto. В случае, если ошибка сохранится - рекомендуется обратиться в технический чат.
{% endhint %}

### **Stopped**:

{% hint style="info" %}
* Статус Stopped означает, что бот/личка получил ошибку о том, что он не может больше отправлять сообщения в чат.
*

    <figure><img src="../../../.gitbook/assets/Frame 2229.png" alt=""><figcaption></figcaption></figure>
* Например, пользователь заблокировал бота/личку и он больше не может писать ему. То есть, бот/личка получил ошибку о том, что он не может больше отправлять сообщения в чат. Также, это может быть ошибкой от Telegram - например, попадание в лимиты отправки сообщений или же сбой на стороне их серверов.
{% endhint %}

### **Finished**:

{% hint style="info" %}
* Диалог полностью завершён.
* В таком случае ИИ больше не будет отвечать, а пуш-уведомления прекратятся.
*

    <figure><img src="../../../.gitbook/assets/Frame 2231.png" alt=""><figcaption></figcaption></figure>
{% endhint %}

{% hint style="info" %}
<a href="./" class="button secondary" data-icon="envelope-circle-check">Messenger</a><a href="inbox-control.md" class="button secondary" data-icon="inbox-full">Inbox Control</a><a href="custom-filters/" class="button secondary" data-icon="bookmark">Custom Filters</a>
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
