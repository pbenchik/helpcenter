---
icon: bookmark
---

# Настройка- готовая интеграция

> ### Настройка готовой интеграции - это инструкция по подключению партнёрской программы через готовый шаблон.

{% hint style="info" %}
С её помощью можно:

* подключить готовую интеграцию без ручной сборки postback-ссылок
* настроить передачу событий из партнёрской программы в Chatterfy
* связать события с пользователями через `clickid`
* добавить регистрационную ссылку для выдачи пользователям
{% endhint %}

### Как работает готовая интеграция:

{% hint style="info" %}
В готовых интеграциях основные настройки уже подготовлены системой.

Поэтому вам не нужно самостоятельно создавать postback-ссылки и настраивать параметры с нуля.
{% endhint %}

{% hint style="info" %}
В данной инструкции рассматривается пример подключения `PocketOption RevShare [v2] NEW`.
{% endhint %}

### Как настроить готовую интеграцию:

{% stepper %}
{% step %}
{% hint style="info" %}
**Откройте нужную интеграцию**

Перейдите в `Tracker → Integrations`.

Найдите `PocketOption RevShare [v2] NEW`.

Нажмите `Connect +`.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Укажите параметр clickid**

Первый шаг - указать `Click ID Parameter`.

Обычно используется параметр `click_id`.

*

```
<figure><img src="/files/RvFcPkzWkztdwx2MBonV" alt=""><figcaption></figcaption></figure>
```
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Проверьте конфигурации событий**

После выбора `clickid` система автоматически создаёт конфигурации событий и postback URL.

*

```
<figure><img src="/files/sjy6nfBOzgU9nwuSR65R" alt=""><figcaption></figcaption></figure>
```
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Настройте postback в партнёрской программе**

Скопируйте Postback URL из интеграции и добавьте его в кабинет партнёрской программы.

*

```
<div data-with-frame="true"><figure><img src="/files/xfg0jgeFAqfkX0CbzRdQ" alt=""><figcaption></figcaption></figure></div>
```

*

```
<div data-with-frame="true"><figure><img src="/files/G72L8b5dufCGDHiwV61Z" alt=""><figcaption></figcaption></figure></div>
```
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Добавьте регистрационную ссылку**

После настройки postback добавьте регистрационную ссылку в `Registration Links`.

*

```
<div data-with-frame="true"><figure><img src="/files/vYdfm8XDgbyVPv7YnhK7" alt=""><figcaption></figcaption></figure></div>
```

*

```
<div data-with-frame="true"><figure><img src="/files/HLJpP3LUZWpMHqEBZoMI" alt=""><figcaption></figcaption></figure></div>
```
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Выполните проверку**

Сделайте тестовую регистрацию, дождитесь postback и проверьте события в `Tracker → Logs → Postback logs`.
{% endhint %}
{% endstep %}
{% endstepper %}

### Полезно:

<details>

<summary>Что уже настроено в готовой интеграции</summary>

{% hint style="info" %}
В готовой интеграции уже настроены:

* postback-параметры
* события, которые будут передаваться в систему
* готовые postback-ссылки
{% endhint %}

{% hint style="info" %}
Вам остаётся:

* скопировать postback-ссылки
* добавить их в настройки партнёрской программы
* проверить соответствие параметров
{% endhint %}

</details>

<details>

<summary>Почему важен clickid</summary>

{% hint style="danger" %}
Если `clickid` не передаётся в ссылке регистрации, система не сможет связать событие с конкретным пользователем.

Тогда события не будут записываться в Tracker корректно.
{% endhint %}

</details>

<details>

<summary>Конфигурации событий</summary>

{% hint style="info" %}
После выбора параметра `clickid` система автоматически создаёт конфигурации событий.
{% endhint %}

{% hint style="info" %}
В интеграции доступны события:

* `Registration (registration)` — регистрация пользователя
* `Email Confirmation (emailconf)` — подтверждение email
* `First Deposit (sale)` — первый депозит
* `Re-Deposit (resale)` — повторный депозит
* `Withdrawal (withdraw)` — вывод средств
* `Commission (Revshare)` — ревшарная комиссия
{% endhint %}

{% hint style="warning" %}
Для каждого события система генерирует свой `Postback URL`, который нужно использовать в настройках партнёрской программы.
{% endhint %}

</details>

<details>

<summary>Кастомные поля</summary>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (131).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Внутри postback используются дополнительные параметры, которые автоматически создают Custom Fields в CRM.
{% endhint %}

{% hint style="info" %}
Например:

* `fields.trader_id`
{% endhint %}

{% hint style="info" %}
Это означает:

* система создаст поле `trader_id`
* в это поле будет записываться ID клиента из партнёрской программы
{% endhint %}

</details>

<details>

<summary>Как настроить postback в PocketOption</summary>

{% hint style="info" %}
Для каждого события необходимо создать отдельный postback.
{% endhint %}

{% hint style="info" %}
Процесс настройки одинаковый:

* откройте раздел Постбеки в кабинете PocketPartners
* выберите тип постбека: `Global` или `Campaign`
* выберите событие
* вставьте соответствующий Postback URL из Chatterfy
* сопоставьте параметры события
{% endhint %}

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (132).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (134).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (135).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (136).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (137).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (133).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="warning" %}
Самый важный параметр:

* `clickid → CLICK_ID`
{% endhint %}

</details>

<details>

<summary>Дополнительные параметры</summary>

{% hint style="info" %}
При необходимости можно включить дополнительные параметры, например:

* `site_id`
* `trader_id`
* `cid`
* `ac`
* `country`
* `sub_id1 ... sub_id5`
* `promo`
* `device_type`
* `os_version`
* `browser`
* `link_type`
* `date_time`
* `sumdep`
* `wdr_sum`
* `status`
{% endhint %}

</details>

<details>

<summary>Регистрационная ссылка</summary>

{% hint style="info" %}
После настройки postback необходимо добавить регистрационную ссылку.
{% endhint %}

{% hint style="info" %}
Заполните поля:

* `Link name` — внутреннее название ссылки
* `Base URL` — партнёрская ссылка
{% endhint %}

{% hint style="info" %}
После этого система автоматически сформирует `Final URL with Parameters`.
{% endhint %}

{% hint style="info" %}
Пример:

`https://u3.shortink.io/smart/mByVsLe71bbFFH?click\_id=\{{tracker.clickid\}}`
{% endhint %}

</details>

<details>

<summary>Проверка после настройки</summary>

{% hint style="info" %}
После завершения настройки рекомендуется:

1. совершить тестовую регистрацию
2. дождаться отправки postback
3. проверить события в `Tracker → Logs → Postback logs`
{% endhint %}

{% hint style="info" %}
Если события отображаются в логах без ошибок, интеграция настроена корректно.
{% endhint %}

</details>

### Где удобно использовать готовую интеграцию:

{% hint style="success" %}
Готовая интеграция удобна, когда нужно:

* быстро подключить поддерживаемую партнёрскую программу
* избежать ручной сборки postback-ссылок
* связать регистрации и депозиты с пользователями через `clickid`
* автоматически получать события и работать с ними в Tracker
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
