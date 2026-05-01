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

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2137.png" alt=""><figcaption></figcaption></figure></div>

<mark style="color:$warning;">**Где настраиваются статусы?**</mark>

Чтобы открыть список статусов:

* Найдите выдвигающийся раздел Chat Status
{% endhint %}

### **Auto**:

{% hint style="info" %}
Диалог находится в автоматическом режиме.

Пользователь обрабатывается ИИ и движется по воронке.

*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2226.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

### Manual:

{% hint style="info" %}
Диалог переведён в ручную обработку.

*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2225.png" alt=""><figcaption></figcaption></figure></div>

Например:

пользователь отправил медиа и был переведён в Manual - см. [AI Recognition](../../bot-settings/automation-and-ai/ai-recognition.md)

\*пуш-уведомления в этом статусе не отправляются
{% endhint %}

### **Waiting**:

{% hint style="info" %}
Бот ожидает ответа от пользователя.

*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2227.png" alt=""><figcaption></figcaption></figure></div>

Диалог не будет двигаться дальше по воронке, пока пользователь не ответит каким-либо сообщением..
{% endhint %}

### **Ignore**:

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2233.png" alt=""><figcaption></figcaption></figure></div>

Статус присваивается автоматически, если пользователь находился в Manual.
{% endhint %}

### **Blocked**:

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2232.png" alt=""><figcaption></figcaption></figure></div>
* В этом статусе мы можем отправлять сообщения и пользователь будет их получать. Если пользователь будет нам что-то писать находясь в этом статусе, то мы не будем получать его сообщения
{% endhint %}

### **Error**:

{% hint style="info" %}
* Чаты с ошибками от ИИ.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2228.png" alt=""><figcaption></figcaption></figure></div>
* Если вы сталкиваетесь с этим статусом - сначала попробуйте перевести в статус Auto. В случае, если ошибка сохранится - рекомендуется обратиться в технический чат.
{% endhint %}

### **Stopped**:

{% hint style="info" %}
* Статус Stopped означает, что бот/личка получил ошибку о том, что он не может больше отправлять сообщения в чат.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2229.png" alt=""><figcaption></figcaption></figure></div>
* Например, пользователь заблокировал вашего бота/личку и бот/личка больше не может писать ему.&#x20;

То есть, бот/личка получил ошибку о том, что он не может больше отправлять сообщения в чат. Также, это может быть ошибкой от Telegram - например, попадание в лимиты после принятия заявки/открытый канал.


{% endhint %}

### **Finished**:

{% hint style="info" %}
* Диалог полностью завершён.
* В таком случае ИИ больше не будет отвечать, а пуш-уведомления прекратятся.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2231.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
<a href="./" class="button secondary" data-icon="envelope-circle-check">Messenger</a><a href="inbox-control.md" class="button secondary" data-icon="inbox-full">Inbox Control</a><a href="custom-filters/" class="button secondary" data-icon="bookmark">Custom Filters</a>
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
