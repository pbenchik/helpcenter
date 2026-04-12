---
icon: telegram
---

# Default

> ### Default - это стандартный режим создания Telegram-лендинга в Tracker.

{% hint style="info" %}
С его помощью можно:

* быстро собрать страницу из готовых полей
* настроить внешний вид лендинга внутри системы
* добавить кнопки, тексты и изображения без загрузки архива
* сразу использовать лендинг в Campaigns
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image 32592.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

### Как работает Default landing:

{% hint style="info" %}
Этот режим подходит, если не нужен собственный архив и достаточно стандартного шаблона.
{% endhint %}

{% hint style="info" %}
Лендинг настраивается внутри системы и после сохранения может использоваться в кампании.
{% endhint %}

### Как настроить Default landing:

{% stepper %}
{% step %}
{% hint style="info" %}
**Заполните General**

Сначала задаются базовые параметры лендинга.

Здесь указываются его внутреннее имя и список байеров, которым он будет доступен.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Настройте Settings**

Дальше настраивается внешний вид страницы.

На этом этапе заполняются тексты, изображения, кнопки и визуальные элементы лендинга.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**При необходимости используйте Custom code**

После этого можно добавить дополнительные стили и логику.

Этот блок нужен, если стандартных настроек недостаточно.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Подключите лендинг к кампании**

Когда лендинг сохранён, его можно выбрать в Campaigns.

Так он становится частью маршрута пользователя до Telegram.
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее про разделы :

<details>

<summary>General</summary>

{% hint style="info" %}
Раздел для базовой настройки лендинга.

Здесь указываются:

* `Name` — внутреннее название лендинга
* `Buyers` — байеры, которым доступен лендинг
{% endhint %}

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image 32592.png" alt=""><figcaption></figcaption></figure></div>

</details>

<details>

<summary>Settings</summary>

{% hint style="info" %}
Раздел для настройки внешнего вида стандартного лендинга.
{% endhint %}

{% hint style="info" %}
Здесь можно заполнить:

* `Description` — описание в верхней части страницы
* `Title` — основной заголовок
* `Avatar` — изображение в превью
* `Text` — дополнительный текст
* `Count` — количество участников или подписчиков
* `Header button` — текст верхней кнопки
* `Button text` — текст основной кнопки
{% endhint %}

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (92).png" alt=""><figcaption></figcaption></figure></div>

</details>

<details>

<summary>Custom code</summary>

{% hint style="info" %}
Раздел для дополнительной настройки лендинга.
{% endhint %}

{% hint style="info" %}
Через него можно:

* менять стили страницы
* добавлять кастомную вёрстку
* подключать аналитику
* обрабатывать действия пользователя
{% endhint %}

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (90).png" alt=""><figcaption></figcaption></figure></div>

</details>

<details>

<summary>Что важно учитывать</summary>

{% hint style="warning" %}
Если используется источник Facebook, invite-ссылки создаются системой автоматически.

Вручную добавлять их в лендинг не требуется.
{% endhint %}

{% hint style="info" %}
Если invite-ссылка Telegram добавляется вручную, сначала настройте источник в разделе Sources и укажите эту ссылку там.
{% endhint %}

</details>

<details>

<summary>Чем Default отличается от Custom</summary>

{% hint style="info" %}
`Default` подходит, если нужен стандартный шаблон внутри системы.
{% endhint %}

{% hint style="info" %}
Если нужен кастомный дизайн, своя структура и нестандартная логика страницы, используйте [Custom](custom.md).
{% endhint %}

</details>

### Где удобно использовать Default:

{% hint style="success" %}
Default удобно использовать, когда нужно:

* быстро собрать лендинг без загрузки архива
* использовать стандартный шаблон Tracker
* запустить страницу с базовыми настройками и кнопками
* подключить лендинг к Campaigns без долгой подготовки
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
