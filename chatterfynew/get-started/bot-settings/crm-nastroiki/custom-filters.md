---
icon: filter
---

# Custom Filters

> ### Custom Filters - это инструмент для создания пользовательских фильтров внутри CRM.

{% hint style="info" %}
С его помощью можно:

\- быстро находить нужных лидов

\- сегментировать диалоги по данным CRM

\- собирать выборки по нескольким условиям

\- упрощать навигацию по чатам и сценариям
{% endhint %}

### Как работают Custom Filters:

{% hint style="info" %}
Custom Filters объединяют пользователей по выбранным условиям.
{% endhint %}

{% hint style="info" %}
Фильтр может учитывать этап воронки, теги, события, менеджера и другие поля.

Это помогает быстро собирать нужные сегменты без ручного поиска.
{% endhint %}

### Как создать Custom Filter:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Нажмите Add New Filter**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2256 (10).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Нажмите Add Condition**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2248 (72).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Выберите нужные условия фильтрации**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2248 (74).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Сохраните фильтр**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2248 (75).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Какие условия доступны</summary>

{% hint style="info" %}
Сейчас доступны такие переменные:

* Step - шаг, на котором находится пользователь
* Flow - флоу, в котором находится пользователь
* Tags - наличие или отсутствие одного или нескольких тегов
* Custom Fields - значения кастомных полей
* Tracker Field - значения трекерных полей
* Assign - назначенный менеджер
* Status - текущий статус пользователя
* Sale Stage - этап продажи
* Events - события пользователя
* Total Deposit - сумма депозитов
* Created At - дата и время создания чата
{% endhint %}

{% hint style="info" %}
Через **Tracker Field** можно фильтровать по таким данным:

* кампания
* сорс
* домен
* лендинг
* тип залива
* тип сорса

Эти фильтры доступны, если у пользователя есть соответствующий доступ к Tracker.
{% endhint %}

</details>

<details>

<summary>Где используются Custom Filters</summary>

{% hint style="info" %}
Фильтры помогают работать с CRM точнее и быстрее:

* в списке диалогов для быстрого поиска
* при сегментации лидов по действиям и этапам
* при распределении пользователей между менеджерами
{% endhint %}

</details>

<details>

<summary>Связанные параметры</summary>

{% hint style="info" %}
Custom Filters часто используют вместе с этими разделами:

* [Tags](tags.md)
* [Custom Fields](../custom-fields.md)
* [Assign Manager](assign-manager.md)
* [Chat status](../../crm/messenger/chat-status.md)
* [Sale Status](../sale-status.md)
* [Events](../../crm/messenger/kartochka-klienta/events/)
{% endhint %}

</details>

<details>

<summary>Важные особенности</summary>

{% hint style="warning" %}
**Custom Filters нужны для внутренней работы в CRM.**

* чем точнее условия, тем быстрее оператор находит нужные чаты
* один фильтр можно собрать сразу по нескольким параметрам
* фильтры особенно полезны при большом количестве лидов
{% endhint %}

</details>

### Где удобно использовать Custom Filters:

{% hint style="success" %}
Custom Filters удобно использовать, когда нужно:

* быстро находить нужные сегменты лидов
* отделять пользователей по статусам, тегам и этапам
* собирать выборки для менеджеров и операторов
* ускорять работу с большим количеством чатов
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
