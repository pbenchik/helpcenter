---
icon: memo-circle-check
---

# Parameters- раздел campaing

> ### Parameters - это раздел Campaigns для настройки параметров трекинговой ссылки.

### С помощью Parameters можно:

{% hint style="info" %}
* передавать в ссылке служебные метки
* сохранять buyer, campaign, creative и `subid`
* выводить нужные параметры в CRM
* унифицировать аналитику по кампаниям
{% endhint %}

### Как работает Parameters:

{% hint style="info" %}
Здесь определяется, какие значения будут передаваться в ссылке кампании.
{% endhint %}

{% hint style="info" %}
Это нужно, чтобы сохранять служебные метки для аналитики, CRM и разрезов по трафику.
{% endhint %}

### Как добавить параметр:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Перейдите во вкладку Parameters**

    Откройте нужную кампанию и перейдите в раздел `Parameters`.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2163.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Добавьте новый параметр**

    Нажмите кнопку добавления нового параметра.

    После этого откроется строка или форма для заполнения полей.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2164.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Заполните основные поля**

    Укажите:

    * `Name`
    * `Parameter`
    * `Placeholder`
    * `Visible`

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2164 (1).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Проверьте формат параметра**

    Убедитесь, что техническое имя написано без пробелов и кириллицы.

    Если используется макрос, проверьте его синтаксис до запуска трафика.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Сохраните изменения**

    Нажмите `Save`.

    После сохранения параметр начнёт использоваться в трекинговой ссылке кампании.
{% endhint %}
{% endstep %}
{% endstepper %}

<details>

<summary>Что настраивается в Parameters</summary>

{% hint style="info" %}
В этом разделе обычно задают:

* отображаемое название параметра
* техническое имя параметра в ссылке
* значение, макрос или переменную для подстановки
* видимость параметра в CRM
* структуру служебных меток для аналитики
{% endhint %}

</details>

<details>

<summary>Что проверить перед настройкой</summary>

{% hint style="info" icon="exclamation" %}
Перед настройкой Parameters проверьте:

* кампания уже создана
* вы заранее определили нужные метки
* технические названия параметров согласованы
{% endhint %}

</details>

<details>

<summary>Какую роль Parameters играет в системе</summary>

{% hint style="warning" %}
Сначала вы задаёте, какие параметры должны попадать в трекинговую ссылку.

Так система понимает, какие значения нужно передавать вместе с переходом.
{% endhint %}

{% hint style="warning" %}
Дальше в параметры подставляются статичные значения, макросы или переменные.

Именно они передаются вместе с трафиком в кампанию.
{% endhint %}

{% hint style="warning" %}
После клика эти значения помогают строить аналитику и искать пользователя по меткам.

Часть параметров можно показывать в карточке лида.
{% endhint %}

</details>

<details>

<summary>Какие поля есть в Parameters</summary>

{% hint style="info" %}
`Name` — понятное название параметра внутри интерфейса.

Используйте короткие и читаемые названия.

Например: `Buyer`, `Creative`, `Campaign ID`.
{% endhint %}

{% hint style="info" %}
`Parameter` — техническое имя параметра, которое попадает в ссылку.

Обычно используют короткий формат без пробелов.

Например: `buyer`, `creative`, `campaign_id`, `sub1`.
{% endhint %}

{% hint style="warning" %}
Не используйте пробелы, кириллицу и случайные символы в `Parameter`.
{% endhint %}

{% hint style="info" %}
`Placeholder` — значение, макрос или переменная, которые будут подставляться в ссылку.

Это может быть статичное значение, макрос рекламной платформы или служебная переменная.
{% endhint %}

{% hint style="info" %}
`Visible` — показывает параметр в карточке пользователя в CRM.

Включайте только действительно полезные поля, чтобы не перегружать интерфейс.
{% endhint %}

</details>

<details>

<summary>Что проверить после настройки</summary>

{% hint style="info" %}
После сохранения проверьте:

* ссылка содержит нужные параметры
* технические имена написаны без ошибок
* макросы указаны в правильном формате
* в CRM отображаются только нужные поля
* структура меток подходит для вашей аналитики
{% endhint %}

</details>

<details>

<summary>Какие параметры используют чаще всего</summary>

{% hint style="info" %}
Чаще всего добавляют:

* `buyer`
* `campaign`
* `creative`
* `sub1`
* `sub2`
* `clickid`
{% endhint %}

</details>

### Где удобно использовать Parameters:

{% hint style="success" %}
Parameters удобно использовать, когда нужно:

* разметить ссылку до запуска трафика
* передавать служебные метки в аналитику и CRM
* сохранять buyer, campaign и creative в параметрах
* стандартизировать структуру ссылок по кампаниям
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
