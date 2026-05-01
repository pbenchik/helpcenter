---
icon: expeditedssl
---

# Как настроить SSL

> ### Как настроить SSL - это инструкция для включения `HTTPS` на домене через Cloudflare.

{% hint style="info" %}
С её помощью можно:

* открыть домен по `HTTPS`
* убрать ошибки сертификата
* подготовить домен или поддомен к работе в Tracker
* завершить настройку после добавления DNS-записи
{% endhint %}

### Как работает SSL:

{% hint style="info" %}
Настройка выполняется в Cloudflare после добавления DNS-записи.
{% endhint %}

{% hint style="info" %}
Без корректного SSL домен может открываться с ошибками или не открываться совсем.
{% endhint %}

### Как настроить SSL:

{% stepper %}
{% step %}
{% hint style="info" %}
* **Откройте раздел SSL/TLS → Overview**
* Перейдите в Cloudflare и откройте настройки домена.
* Затем откройте раздел `SSL/TLS → Overview`.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (82).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Выберите режим Flexible**
* В блоке режима SSL установите значение `Flexible`.
* После этого Cloudflare начнёт автоматически выпускать сертификат.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Проверьте сертификат**
* Откройте раздел `SSL/TLS → Edge Certificates`.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (83).png" alt=""><figcaption></figcaption></figure></div>
* Убедитесь, что сертификат имеет статус `Active`.
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Что настраивается в SSL</summary>

{% hint style="info" %}
В этой настройке обычно делают:

* выбор режима SSL для домена
* проверку выпуска сертификата Cloudflare
* контроль статуса сертификата
* проверку открытия домена по `HTTPS`
{% endhint %}

</details>

<details>

<summary>Когда использовать эту инструкцию</summary>

{% hint style="info" %}
Эта инструкция нужна, когда вы хотите:

* открыть домен по `HTTPS`
* убрать ошибки сертификата
* подготовить домен или поддомен к работе в Tracker
* завершить настройку после добавления DNS-записи
* дальше добавить домен в Chatterfy
{% endhint %}

</details>

<details>

<summary>Что проверить перед настройкой</summary>

{% hint style="warning" %}
Перед настройкой проверьте:

* домен или поддомен уже добавлен в Cloudflare
* DNS-запись уже создана
* вы открыли настройки именно нужного домена
* для работы домена используется режим `Flexible`
{% endhint %}

{% hint style="info" %}
Другой режим может привести к ошибкам открытия страницы.
{% endhint %}

</details>

<details>

<summary>Какую роль SSL играет в системе</summary>

{% hint style="warning" %}
Сначала в Cloudflare выбирается режим SSL.

Он определяет, как домен будет открываться через защищённое соединение.
{% endhint %}

{% hint style="warning" %}
После выбора режима Cloudflare начинает автоматически выпускать сертификат.

На это может потребоваться несколько минут.
{% endhint %}

{% hint style="warning" %}
Когда сертификат активен, домен открывается по `HTTPS`.

После этого его можно безопасно использовать в Tracker и лендингах.
{% endhint %}

</details>

<details>

<summary>Какие поля важно проверить</summary>

{% hint style="info" %}
`SSL/TLS → Overview` — основной раздел, где выбирается режим SSL.

Здесь задаётся базовая логика работы сертификата.
{% endhint %}

{% hint style="info" %}
`Flexible` — рекомендованный режим SSL для этой настройки.

Используйте именно его, если домен работает через Cloudflare с Chatterfy.
{% endhint %}

{% hint style="info" %}
`Edge Certificates` — раздел со статусом сертификата.

Здесь можно проверить, активирован ли сертификат.
{% endhint %}

{% hint style="info" %}
`Active` — статус готового сертификата.

Если вы видите этот статус, домен уже должен открываться по `HTTPS`.
{% endhint %}

</details>

<details>

<summary>Что делать, если сертификат ещё не активен</summary>

{% hint style="info" %}
Если статус `Active` не появился сразу, подождите несколько минут.

Cloudflare выпускает сертификат автоматически.
{% endhint %}

{% hint style="info" %}
После активации сертификата откройте домен в браузере и проверьте, что он работает по `HTTPS`.
{% endhint %}

</details>

<details>

<summary>Что проверить после настройки</summary>

{% hint style="info" %}
После сохранения проверьте:

* в `SSL/TLS → Overview` выбран режим `Flexible`
* в `Edge Certificates` сертификат имеет статус `Active`
* домен открывается по `HTTPS`
* в браузере нет предупреждений о сертификате
* можно переходить к добавлению домена в Chatterfy
{% endhint %}

</details>

### Где удобно использовать эту инструкцию:

{% hint style="success" %}
Эта инструкция удобна, когда нужно:

* быстро включить `HTTPS` на домене
* убрать ошибки сертификата перед запуском
* подготовить домен или поддомен для Tracker
* завершить настройку перед добавлением домена в Chatterfy
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
