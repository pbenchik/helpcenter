---
description: Автоматический прием заявок на вступление в канал
hidden: true
---

# Telegram source Channels

**В случае если мы общаемся с юзерами через личку:**

* Создаем отделльного телеграм бота который будет принимать заявки.
* Добавляем этого бота в админы канала.

<figure><img src="../../../.gitbook/assets/tg channe;s.png" alt=""><figcaption></figcaption></figure>

* В настройках бота нажимаем **Add channel**



<div><figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 5.57.03 AM.png" alt=""><figcaption></figcaption></figure> <figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 5.57.22 AM.png" alt=""><figcaption></figcaption></figure></div>

<figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 5.57.50 AM.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Handle invites** нужен только если хотим чтобы бот принимал заявки и собирал статистику, если только для статистики, то этот чекбокс не нужен.
{% endhint %}



<figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 5.58.48 AM.png" alt=""><figcaption></figcaption></figure>

* [x] Нажимаем **Save и обновляем страницу**
* [x] На этом этапе в нашей личке или боте должен быть хотя бы один степ
* [x] Нажимаем **Add notification bot**



<figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 6.02.10 AM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 6.10.23 AM.png" alt=""><figcaption></figcaption></figure>

Выбираем нашу личку (для синхронизации данных) и добавляем степ (в боте) на который юзер попадет при отправке завяки на вступление в канал.

{% hint style="info" %}
**Custom parameter in Source** - при добавлении значения в это поле в диалоге будет создан дополнительный Custom field с этим значением.
{% endhint %}

{% hint style="info" %}
**Set tag after join** - добавление тега к диалогу.
{% endhint %}

<figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 6.18.05 AM.png" alt=""><figcaption></figcaption></figure>

Обязательно нажимаем **Save** для генерации ссылки.



<figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-16 at 6.19.54 AM.png" alt=""><figcaption></figcaption></figure>

Сгенерированную ссылку нам необходимо вставить во флоу общения с юзером.
