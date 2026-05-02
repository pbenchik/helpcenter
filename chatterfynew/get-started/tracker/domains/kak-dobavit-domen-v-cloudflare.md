---
description: Подключение основного домена к Cloudflare для работы с Tracker.
icon: cloud
---

# Как добавить домен в Cloudflare

Это первый шаг перед добавлением основного домена в Tracker.

Инструкция подходит только для основного домена.

### Видео

{% embed url="https://youtu.be/zcJyh-e2o4k" %}

### Как это работает

Сначала домен подключается к Cloudflare.

Потом вы передаёте DNS-управление и создаёте запись `CNAME`.

### Шаги

#### 1. Добавьте домен в Cloudflare

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (76).png" alt=""><figcaption></figcaption></figure></div>

#### 2. Выберите тариф `Free plan`

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (77).png" alt=""><figcaption></figcaption></figure></div>

#### 3. Замените `nameservers` у регистратора

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (78).png" alt=""><figcaption></figcaption></figure></div>

#### 4. Откройте **DNS → Records**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (79).png" alt=""><figcaption></figcaption></figure></div>

#### 5. Создайте запись `CNAME`

Укажите:

* **Type** — `CNAME`
* **Name** — `@`
* **Target** — `nemo.chatterfy.ai`

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (80).png" alt=""><figcaption></figcaption></figure></div>

#### 6. Сохраните запись

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (81).png" alt=""><figcaption></figcaption></figure></div>

### Notes

{% hint style="info" %}
Если нужен поддомен, используйте [Как добавить поддомен в Cloudflare](kak-dobavit-poddomen-v-cloudflare.md).
{% endhint %}

* Перед началом проверьте доступ к панели регистратора и то, что вы подключаете именно основной домен
* После настройки проверьте обновление `nameservers`, запись `@ → nemo.chatterfy.ai` и готовность домена к `HTTPS`
* Следующие шаги: [Настройте SSL](kak-nastroit-ssl.md) и [Добавьте домен в Chatterfy](kak-dobavit-domen-v-chatterfy.md)
