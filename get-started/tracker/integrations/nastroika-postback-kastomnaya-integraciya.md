---
icon: bookmark
---

# Настройка Postback - кастомная интеграция

> ### Настройка Postback - кастомная интеграция — это инструкция по ручному подключению партнёрской программы к Tracker.

{% hint style="info" %}
С её помощью можно:

* подключить партнёрскую программу, которой нет в списке готовых интеграций
* указать параметр `clickid` для связи событий с пользователем
* создать postback-события вручную
* добавить регистрационную ссылку для выдачи пользователям
{% endhint %}

### Как работает кастомная интеграция:

{% hint style="info" %}
Кастомная интеграция используется, если нужной партнёрской программы нет в списке готовых интеграций.
{% endhint %}

{% hint style="info" %}
Логика работы простая:

1. пользователь переходит по регистрационной ссылке
2. партнёрская программа сохраняет `clickid`
3. при наступлении события программа отправляет postback
4. Chatterfy находит пользователя по `clickid` и записывает событие
{% endhint %}

{% hint style="info" %}
Пример регистрационной ссылки:

`https://partner.com/signup?pbclick={{tracker.clickid}}`
{% endhint %}

### Как настроить кастомную интеграцию:

{% stepper %}
{% step %}
{% hint style="info" %}
**Откройте раздел Integrations**

Чтобы создать кастомную интеграцию:

1. перейдите в Tracker
2. откройте раздел Integrations
3. нажмите `Create Custom integration`

*

    <figure><img src="../../../.gitbook/assets/unknown (123).png" alt=""><figcaption></figcaption></figure>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Укажите параметр clickid**

Первый шаг — указать `Click ID Parameter`.

*

    <figure><img src="../../../.gitbook/assets/unknown (124).png" alt=""><figcaption></figcaption></figure>

Обычно используют:

* `clickid`
* `sub1`
* `sub4`
* `pbclick`
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Настройте postback события**

Нажмите `Add Postback Event`, укажите название события и скопируйте `Postback URL`.

*

    <figure><img src="../../../.gitbook/assets/unknown (125).png" alt=""><figcaption></figcaption></figure>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Добавьте регистрационную ссылку**

После настройки postback добавьте регистрационную ссылку через `Add Registration Link`.

*

    <figure><img src="../../../.gitbook/assets/unknown (128).png" alt=""><figcaption></figcaption></figure>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Выполните проверку**

Перейдите по регистрационной ссылке, выполните тестовое событие и проверьте postback в логах Tracker.
{% endhint %}
{% endstep %}
{% endstepper %}

<details>

<summary>Почему важен clickid</summary>

{% hint style="danger" %}
Если параметр `clickid` не передаётся, система не сможет связать событие с конкретным пользователем.

В этом случае события не будут записываться в Tracker.
{% endhint %}

</details>

<details>

<summary>Основные типы событий</summary>

{% hint style="info" %}
Обычно настраиваются три основных события:

* `Registration (registration)` — регистрация пользователя
* `Sale (sale)` — первый депозит
* `Resale (resale)` — повторный депозит
*

    <figure><img src="../../../.gitbook/assets/unknown (126).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

{% hint style="danger" %}
Используйте точные названия:

* `registration`
* `sale`
* `resale`
{% endhint %}

{% hint style="info" %}
Если назвать событие иначе, система может обработать его некорректно.
{% endhint %}

</details>

<details>

<summary>Параметры postback</summary>

*

    <figure><img src="../../../.gitbook/assets/unknown (127).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
При настройке postback можно передавать дополнительные параметры.

Например:

* `tracker.cost={amount}`
* `tracker.currency=usd`
* `tracker.tid={event_id}`
{% endhint %}

{% hint style="info" %}
Где:

* `amount` — сумма депозита
* `currency` — валюта
* `event_id` — уникальный ID события
{% endhint %}

{% hint style="danger" %}
Названия параметров могут отличаться в зависимости от партнёрской программы.

Перед сохранением проверьте, что вы используете её реальные переменные.
{% endhint %}

</details>

<details>

<summary>Как добавить регистрационную ссылку</summary>

{% hint style="info" %}
Для этого:

1. нажмите `Add Registration Link`
2. укажите `Link name` — внутреннее название ссылки
3. добавьте `Base URL` — регистрационную ссылку из партнёрской программы
{% endhint %}

{% hint style="info" %}
Система автоматически сформирует поле `Final URL with Parameters`.
{% endhint %}

{% hint style="info" %}
Пример:

`https://partner.com/signup?pbclick={{tracker.clickid}}`
{% endhint %}

{% hint style="info" %}
Эту ссылку можно отправлять пользователю.

Система автоматически подставит `clickid` для каждого перехода.
{% endhint %}

</details>

<details>

<summary>Проверка после настройки</summary>

{% hint style="info" %}
После завершения настройки рекомендуется сделать тест:

1. перейдите по регистрационной ссылке
2. выполните тестовое событие в партнёрской программе
3. проверьте, появился ли postback в логах Tracker
{% endhint %}

{% hint style="info" %}
Если событие отображается корректно, интеграция настроена правильно.
{% endhint %}

</details>

### Где удобно использовать кастомную интеграцию:

{% hint style="success" %}
Кастомная интеграция удобна, когда нужно:

* подключить партнёрскую программу без готового шаблона
* гибко настроить свои события и параметры
* связать postback с пользователем через `clickid`
* передавать регистрации и депозиты в Tracker вручную настроенной схемой
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
