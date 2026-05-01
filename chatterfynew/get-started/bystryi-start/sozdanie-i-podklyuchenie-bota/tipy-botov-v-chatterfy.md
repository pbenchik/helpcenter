---
icon: clipboard-list-check
---

# Типы ботов в Chatterfy

> ### В Chatterfy доступны четыре типа подключений.
>
> ### Выбор зависит от того, как вы хотите общаться с пользователем.

{% tabs %}
{% tab title="Standard" %}
{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2251.png" alt=""><figcaption></figcaption></figure></div>

Основной тип бота.

Подходит для большинства сценариев.

Поддерживает:

* CRM-обработку
* AI-обработку
* работу как invite-бот
{% endhint %}
{% endtab %}

{% tab title="Invite" %}
{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2251 (1).png" alt=""><figcaption></figcaption></figure></div>

Используется как invite-бот для каналов.

Поддерживает:

* приём заявок в канал
* приветственное сообщение после вступления

Не поддерживает:

* CRM-обработку
* AI-обработку
{% endhint %}
{% endtab %}

{% tab title="Personal" %}
{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2251 (2).png" alt=""><figcaption></figcaption></figure></div>

Это подключённый личный Telegram-аккаунт.

Подключение доступно по номеру телефона или через QR-код.

Особенности:

* все чаты автоматически попадают в CRM
* по возможностям аналогичен Standard-боту
{% endhint %}
{% endtab %}

{% tab title="Business" %}
{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2251 (3).png" alt=""><figcaption></figcaption></figure></div>

Это бот, подключённый к личному аккаунту с Telegram Premium.

Особенности:

* общение идёт от лица личного аккаунта
* доступны увеличенные лимиты сообщений
{% endhint %}

{% hint style="warning" %}
Если пользователь не писал более 24 часов, новый исходящий message отправить нельзя.

Сначала пользователь должен ответить снова.
{% endhint %}
{% endtab %}
{% endtabs %}

### Что делать дальше:

{% hint style="info" %}
* <a href="kak-sozdat-bota-v-telegram.md" class="button secondary" data-icon="telegram">Как создать бота в Telegram</a><a href="podklyuchenie-bota-ili-lichnyi-akkaunt-k-chatterfy.md" class="button secondary" data-icon="plug">Подключение бота или личного аккаунта</a>
* <a href="../bazovaya-nastroika-bota.md" class="button secondary" data-icon="sliders">Базовая настройка бота</a><a href="../../../dobro-pozhalovat/arkhitektura-sistemy/crm-rabota-s-klientami.md" class="button secondary" data-icon="comments">CRM — работа с клиентами</a>
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
