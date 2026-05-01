---
icon: square-root-variable
---

# Bot Variables

> ### Bot Variables - это переменные, которые можно создать для конкретного бота или лички.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2256 (6).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
С их помощью можно:

\- централизованно хранить ссылки, ID и другие значения

\- использовать одни и те же данные в сообщениях и шагах

\- быстро обновлять значение в одном месте

\- сокращать длинные ссылки через свой домен
{% endhint %}

### Как создать Bot Variable:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Перейдите в Bot Settings**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2213 (1).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Пролистайте вниз до блока Bot Variables**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2215.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Нажмите Add New Variable**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2215 (1).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **В поле Variable Name укажите название переменной**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* #### **В поле Value укажите значение переменной**
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Примеры переменных</summary>

{% hint style="info" %}
Примеры названий:

* `regLink`
* `trader_id`
{% endhint %}

{% hint style="info" %}
Примеры значений:

* `https://pp.com?clickid={{tracker.clickid}}`
* `{{fields.trader_id}}`
{% endhint %}

</details>

<details>

<summary>Как использовать Bot Variables</summary>

{% hint style="info" %}
После создания переменную можно использовать в сообщениях, шагах и сценариях через макрос:

* <mark style="color:$primary;">`\{{variables.regLink\}}`</mark>
* <mark style="color:$primary;">`\{{variables.trader_id\}}`</mark>
{% endhint %}

{% hint style="info" %}
Если значение изменится, достаточно обновить его один раз в Bot Settings.

После этого изменения применятся везде, где используется этот макрос.
{% endhint %}

</details>

<details>

<summary>Shorten the link</summary>

{% hint style="info" %}
Если значение переменной - длинная ссылка, можно включить опцию `Shorten the link`.
{% endhint %}

{% hint style="info" %}
Для этого:

* включите `Shorten the link`
* выберите один из своих доменов в поле `Domains`
{% endhint %}

</details>

<details>

<summary>Пример сокращения ссылки</summary>

{% hint style="info" %}
Пример:

Изначальная ссылка:

https://partner.program/registerutm\_campaign=111111\&utm\_source=11111\&utm\_medium=11111\&a=11111\&ac=11111\&code=50START\&click\_id=\{{tracker.clickid\}}

Домен:

testdomain.com

Финальная ссылка:

https://testdomain.com/qp7h3zi
{% endhint %}

</details>

<details>

<summary>Использование в AI</summary>

{% hint style="info" %}
Bot Variables можно использовать и в AI-промптах.
{% endhint %}

{% hint style="info" %}
Это удобно, потому что:

* вместо вставки ссылки вручную AI может использовать `{{variables.regLink}}`
* при изменении ссылки достаточно обновить одну переменную
* не нужно редактировать каждый шаг или каждый промпт отдельно
{% endhint %}

</details>

### Где удобно использовать Bot Variables:

{% hint style="success" %}
Bot Variables удобно использовать, когда нужно:

* хранить общие ссылки и ID в одном месте
* быстро менять данные без ручного поиска по шагам
* использовать одни и те же значения в нескольких сценариях
* сокращать длинные ссылки через собственный домен
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
