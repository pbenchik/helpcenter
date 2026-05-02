---
icon: expeditedssl
---

# Как настроить SSL

Эта инструкция нужна для включения `HTTPS` на домене через Cloudflare.

Без корректного SSL домен может открываться с ошибками.

### Как это работает

Настройка выполняется после добавления DNS-записи.

Cloudflare выпускает сертификат автоматически после выбора режима SSL.

### Шаги

#### 1. Откройте `SSL/TLS → Overview`

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (82).png" alt=""><figcaption></figcaption></figure></div>

#### 2. Выберите режим `Flexible`

После этого Cloudflare начнёт выпускать сертификат.

#### 3. Проверьте сертификат

Откройте `SSL/TLS → Edge Certificates`.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (83).png" alt=""><figcaption></figcaption></figure></div>

Убедитесь, что сертификат имеет статус `Active`.

### Notes

{% hint style="warning" %}
Используйте режим `Flexible`. Другой режим может привести к ошибкам открытия страницы.
{% endhint %}

* Перед настройкой проверьте, что домен уже добавлен в Cloudflare и DNS-запись создана
* Если статус `Active` не появился сразу, подождите несколько минут и проверьте ещё раз
* После настройки проверьте открытие домена по `HTTPS`

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
