---
icon: nfc-signal
---

# Как добавить домен в Chatterfy

> ### Как добавить домен в Chatterfy - это финальный шаг после настройки DNS и SSL.

{% hint style="info" %}
С его помощью можно:

* добавить домен или поддомен в Tracker
* сделать домен доступным в `Tracker → Domains`
* выдать доступ нужным байерам
* использовать домен в кампаниях и лендингах
{% endhint %}

### Видеоинструкция:

{% hint style="info" icon="nfc-signal" %}
В видео показано, как подключить домен для работы в Tracker и довести настройку до использования в Chatterfy.

Подойдёт, если вы уже настроили DNS и SSL и хотите быстро проверить общий порядок подключения домена.

{% embed url="https://youtu.be/zcJyh-e2o4k" fullWidth="false" %}

**Таймкоды:**

* 00:05 — добавление домена в Cloudflare
* 00:34 — настройка Name Service
* 01:17 — добавление DNS-записи
* 01:52 — добавление домена в Chatterfy
* 02:01 — настройка SSL
{% endhint %}

### Как работает добавление домена:

{% hint style="info" %}
После этого домен появится в `Tracker → Domains`.
{% endhint %}

{% hint style="info" %}
Дальше его можно использовать в кампаниях и назначать байерам.
{% endhint %}

### Как добавить домен в Chatterfy:

{% stepper %}
{% step %}
{% hint style="info" %}
* **Откройте раздел Tracker → Domains**
* Перейдите в раздел `Tracker → Domains`.
* Здесь хранится список всех доменов, подключённых к Tracker.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Нажмите Create domain**
* Нажмите кнопку `Create domain`.
* После этого откроется форма добавления нового домена.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2165.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Заполните поля Domain и Buyers**
* Укажите:
* `Domain` — ваш домен или поддомен
* `Buyers` — байеры, которым нужно дать доступ
* Проверьте значения перед сохранением.
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2166.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Нажмите Apply**
* Сохраните настройку кнопкой `Apply`.
* После сохранения домен появится в списке и станет доступен для работы.
{% endhint %}
{% endstep %}
{% endstepper %}

<details>

<summary>Что проверить перед настройкой</summary>

{% hint style="warning" %}
Перед настройкой проверьте:

* домен уже добавлен в Cloudflare
* DNS-запись уже создана
* SSL уже настроен
* домен открывается в браузере по `HTTPS`
{% endhint %}

{% hint style="info" %}
Если эти шаги ещё не сделаны, сначала откройте статьи [Как добавить домен в Cloudflare](kak-dobavit-domen-v-cloudflare.md) и [Как настроить SSL](kak-nastroit-ssl.md).
{% endhint %}

</details>

<details>

<summary>Какую роль эта настройка играет в системе</summary>

{% hint style="warning" %}
Сначала домен настраивается в Cloudflare.

Там создаются DNS-записи и включается SSL.
{% endhint %}

{% hint style="warning" %}
После этого домен вручную добавляется в Chatterfy.

На этом этапе система начинает видеть его внутри раздела Domains.
{% endhint %}

{% hint style="warning" %}
Когда домен сохранён, его можно выбирать в Campaigns.

Также он становится доступен тем байерам, которых вы укажете.
{% endhint %}

</details>

<details>

<summary>Какие поля нужно заполнить</summary>

{% hint style="info" %}
`Domain` — домен или поддомен, который вы уже подготовили в Cloudflare.

Указывайте его в том же виде, в котором он должен использоваться в Tracker.
{% endhint %}

{% hint style="info" %}
`Buyers` — список байеров, которым будет доступен этот домен.

Если не выбрать нужных байеров, они не смогут использовать домен в своих кампаниях.
{% endhint %}

</details>

<details>

<summary>Что проверить после настройки</summary>

{% hint style="info" %}
После сохранения проверьте:

* домен появился в `Tracker → Domains`
* домен открывается в браузере по `HTTPS`
* в браузере нет ошибок SSL
* нужные байеры видят домен
* домен доступен для выбора в Campaigns
*

```
<div data-with-frame="true"><figure><img src="/files/aM6fYacFA20q0iWVEjPM" alt=""><figcaption></figcaption></figure></div>
```
{% endhint %}

</details>

### Где удобно использовать эту инструкцию:

{% hint style="success" %}
Эта инструкция удобна, когда нужно:

* завершить подключение домена после DNS и SSL
* сделать домен доступным для кампаний
* выдать доступ к домену нужным байерам
* подготовить домен к работе в Tracker и лендингах
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
