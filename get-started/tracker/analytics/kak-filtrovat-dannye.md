---
icon: filter
---

# Как фильтровать данные

> ### Как фильтровать данные - это инструкция для быстрого поиска нужного среза трафика в Analytics.

{% hint style="info" %}
С её помощью можно:

* быстро находить нужный сегмент трафика
* фильтровать данные по параметрам ссылки
* добавлять дополнительные условия по кампании и дате
* группировать статистику по нужному параметру
*   Скриншот блока `Filters`:

    ![Блок Filters в Analytics](<../../../.gitbook/assets/unknown (96).png>)
{% endhint %}

### Как работает фильтрация:

{% hint style="info" %}
Фильтры находятся в блоке `Filters` над таблицей Analytics.
{% endhint %}

{% hint style="info" %}
Они помогают быстро найти нужный срез трафика без ручного поиска по всей таблице.
{% endhint %}

### Как применить фильтр:

{% stepper %}
{% step %}
{% hint style="info" %}
**Откройте блок Filters**

Укажите нужные параметры для отбора трафика.
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**При необходимости задайте дополнительные условия**

Выберите:

* `Campaign`
* `Date`
* `Group By`
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
**Нажмите Search**

Таблица и метрики обновятся по выбранным условиям.
{% endhint %}
{% endstep %}
{% endstepper %}

<details>

<summary>Какие параметры можно фильтровать</summary>

{% hint style="info" %}
Вы можете использовать любые параметры, которые передаются в ссылке залива.

Например:

* `campaign_name`
* `ad_campaign_id`
* `adset_id`
* `ad_name`
* `placement`
* `utm_source`
* `utm_campaign`
* `utm_content`
* `keyword`
* `source_name`
* `buyer`
* и другие параметры
{% endhint %}

</details>

<details>

<summary>Как работает Group By</summary>

{% hint style="info" %}
`Group By` группирует статистику по выбранному параметру.
{% endhint %}

{% hint style="info" %}
Например, по:

* `Day`
* `source_name`
* `ad_name`
* `buyer`
* UTM-меткам
* другим параметрам из ссылки
{% endhint %}

{% hint style="info" %}
Это удобно для анализа эффективности отдельных связок и источников.

*   Скриншот поля `Group By`:

    ![Поле Group By](<../../../.gitbook/assets/unknown (97).png>)
{% endhint %}

</details>

<details>

<summary>Как лучше использовать Filters и Group By</summary>

{% hint style="info" %}
Фильтры и `Group By` работают вместе.

Сначала сузьте выборку, затем сгруппируйте данные по нужному параметру.
{% endhint %}

</details>

### Где удобно использовать фильтрацию:

{% hint style="success" %}
Фильтрацию удобно использовать, когда нужно:

* найти нужную кампанию или связку
* сравнить результаты по buyer, source или UTM
* сузить данные перед выгрузкой
* разобрать конкретный сегмент трафика
{% endhint %}

### Что дальше?

* [Как выгрузить данные](kak-vygruzit-dannye.md)
* [Вернуться в Analytics](./)

{% include "../../../.gitbook/includes/na-glavnuyu.md" %}
