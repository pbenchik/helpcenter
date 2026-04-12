---
icon: indent
---

# Notifications

> ### Notifications позволяют получать уведомления о событиях, происходящих в диалогах бота.

Они используются для оповещения команды о чатах, которые требуют ручной проверки. Уведомления могут отправляться.

{% hint style="info" %}
**Видеоинструкция как подключить Notifications**

{% embed url="https://youtu.be/pYCUUyoCDtA" %}
{% endhint %}

### Как настроить Notifications:

{% hint style="info" %}
Чтобы получать уведомления, необходимо подключить Telegram-чат к боту/личке.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (8).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% stepper %}
{% step %}
### Подготовьте чат

{% hint style="info" %}
**Выберите, куда будут приходить уведомления.**

*

    <div align="center" data-full-width="false" data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (158).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
### Получите Telegram ID

{% hint style="info" %}
* Формат Telegram ID
* Единственное отличие зависит от типа бота - как записывается ID:
* Если это бот - ID указывается с минусом (-)
* Если это личка - ID указывается без минуса

<mark style="color:blue;">Примеры:</mark> Примеры:

* Бот: `-2894347`
* Личка: `2894347`
{% endhint %}
{% endstep %}

{% step %}
### **Для подключения необходимо узнать Telegram ID выбранного чата.**

{% hint style="info" %}
* Чтобы это сделать, просто добавьте @username\_to\_id\_bot в нужный вам чат, напишите команду /start, и он напишет вам нужный ID.
* Нужный нам ID — это ID чата.
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (9).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
### Шаг 3. Добавьте ID в настройки

{% hint style="info" %}
* Откройте вашего бота в платформе
* Перейдите в Bot Settings
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2255.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
### Откройте раздел Notifications

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2254.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
### Вставьте Telegram ID

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2253.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
### Добавьте параметр, при котором должно отправляться уведомление.

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2252.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}
{% endstepper %}

{% hint style="info" %}
После сохранения уведомления начнут отправляться в указанный чат.
{% endhint %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
