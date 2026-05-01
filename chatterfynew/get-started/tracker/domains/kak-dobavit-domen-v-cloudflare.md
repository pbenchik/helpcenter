---
icon: cloud
---

# Как добавить домен в Cloudflare

> ### Как добавить домен в Cloudflare - это первый шаг перед добавлением домена в Tracker.

{% hint style="info" %}
С его помощью можно:

* передать управление DNS в Cloudflare
* подключить основной домен для кампаний и лендингов
* создать нужную запись для работы с Chatterfy
* подготовить домен к SSL и дальнейшему подключению в Tracker
{% endhint %}

### Видеоинструкция:

{% hint style="info" icon="cloud" %}
В видео показано, как добавить основной домен в Cloudflare и направить его на Chatterfy.

Подойдёт, если вы подключаете домен для кампаний, лендингов и трекинга.

{% embed url="https://youtu.be/zcJyh-e2o4k" %}
{% endhint %}

### Как работает подключение домена:

{% hint style="info" %}
Здесь вы передаёте управление DNS в Cloudflare и создаёте нужную запись.
{% endhint %}

{% hint style="info" %}
Это нужно, чтобы домен корректно работал с Chatterfy.
{% endhint %}

### Как добавить домен в Cloudflare:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Добавьте домен в Cloudflare**

    Перейдите в Cloudflare и добавьте ваш домен.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (76).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Выберите тариф Free plan**

    На этапе подключения выберите бесплатный тариф.

    Этого достаточно для стандартной настройки домена.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (77).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Замените nameservers у регистратора**

    Cloudflare покажет новые nameservers для домена.

    Откройте панель регистратора и замените текущие значения на новые.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (78).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Откройте DNS → Records**

    После активации домена откройте настройки DNS в Cloudflare.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (79).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Создайте запись CNAME**

    Укажите такие значения:

    * `Type` — `CNAME`
    * `Name` — `@`
    * `Target` — `nemo.chatterfy.ai`

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (80).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Сохраните запись**

    Нажмите сохранение и дождитесь применения настроек.

    После этого Cloudflare начнёт обслуживать домен с новой DNS-записью.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (81).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Что настраивается в Cloudflare</summary>

{% hint style="info" %}
В этой настройке обычно делают:

* добавление основного домена в Cloudflare
* замену текущих nameservers на nameservers Cloudflare
* создание DNS-записи `CNAME`
* привязку домена к `nemo.chatterfy.ai`
{% endhint %}

</details>

<details>

<summary>Когда использовать эту инструкцию</summary>

{% hint style="info" %}
Эта инструкция нужна, когда вы хотите:

* подключить основной домен к Tracker
* использовать домен в кампаниях и лендингах
* передать DNS-управление в Cloudflare
* подготовить домен к настройке SSL
* дальше добавить домен в Chatterfy
{% endhint %}

</details>

<details>

<summary>Что проверить перед настройкой</summary>

{% hint style="warning" %}
Перед настройкой проверьте:

* домен уже куплен у регистратора
* у вас есть доступ к панели регистратора
* вы подключаете именно основной домен
{% endhint %}

{% hint style="info" %}
Если нужен поддомен, используйте статью [Как добавить поддомен в Cloudflare](kak-dobavit-poddomen-v-cloudflare.md).
{% endhint %}

</details>

<details>

<summary>Какую роль эта настройка играет в системе</summary>

{% hint style="warning" %}
Сначала вы добавляете домен в Cloudflare.

После этого сервис подготавливает его к управлению DNS.
{% endhint %}

{% hint style="warning" %}
Дальше вы меняете nameservers у регистратора.

С этого момента DNS начинает обслуживать Cloudflare.
{% endhint %}

{% hint style="warning" %}
После этого вы добавляете запись `CNAME`.

Она направляет домен на инфраструктуру Chatterfy.
{% endhint %}

{% hint style="warning" %}
Когда запись сохранена, можно настраивать SSL и добавлять домен в Chatterfy.

Без этого домен не получится использовать в Tracker.
{% endhint %}

</details>

<details>

<summary>Какие данные понадобятся</summary>

{% hint style="info" %}
`Nameservers` — адреса DNS-серверов, которые выдаёт Cloudflare.

Их нужно вставить у регистратора домена.
{% endhint %}

{% hint style="info" %}
`Type` — тип DNS-записи.

Для этой настройки используйте `CNAME`.
{% endhint %}

{% hint style="info" %}
`Name` — имя записи.

Для основного домена используйте `@`.
{% endhint %}

{% hint style="info" %}
`Target` — адрес назначения для домена.

Укажите `nemo.chatterfy.ai`.
{% endhint %}

</details>

<details>

<summary>Что проверить после настройки</summary>

{% hint style="info" %}
После сохранения проверьте:

* домен отображается в Cloudflare без ошибок
* nameservers у регистратора уже обновлены
* запись `CNAME` создана с `@ → nemo.chatterfy.ai`
* домен готов к следующему шагу с SSL
* дальше домен можно добавить в Chatterfy
{% endhint %}

</details>

### Где удобно использовать эту инструкцию:

{% hint style="success" %}
Эта инструкция удобна, когда нужно:

* подключить основной домен для Tracker
* подготовить домен под лендинги и кампании
* передать DNS в Cloudflare без ошибок
* подготовить основу для SSL и добавления домена в Chatterfy
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
