---
icon: braille
---

# Custom Fields

> ### Custom Fields - это пользовательские поля, которые позволяют хранить дополнительную информацию о диалоге и пользователе.

### Видеоинструкция:

{% embed url="https://youtu.be/OZpz3OOsGPE" %}

{% hint style="info" %}
С их помощью можно:

\- сохранять дополнительные данные по пользователю и диалогу

\- использовать эти данные в логике бота

\- передавать значения через Webhooks и Postback

\- отображать информацию в карточке клиента
{% endhint %}

### Как заполняются Custom Fields:

{% hint style="info" %}
Поля могут заполняться двумя способами:

* автоматически — через Webhooks, Postback и другие интеграции
* вручную — оператором внутри CRM
{% endhint %}

### Как создать Custom Field:

{% stepper %}
{% step %}
{% hint style="info" %}
* **Перейдите в раздел Custom Fields**
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2210.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Нажмите Add Custom Field**
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2210 (1).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Выберите тип поля**
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2211.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Заполните необходимые параметры**
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
#### **Нажмите Save**
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Типы полей</summary>

{% hint style="info" %}
При создании поля нужно выбрать его тип:

* `Text` - короткий текст
* `Long Text` - длинный текст, например заметка
* `Link` - ссылка
* `Number` - числовое значение
* `Date` - дата в формате `2030-01-30T10:20:30Z`
* `Select` - выбор одного варианта из списка
* `Multiselect` - выбор нескольких вариантов
{% endhint %}

</details>

<details>

<summary>Select и Multiselect</summary>

{% hint style="info" %}
Для типов `Select` и `Multiselect` можно заранее задать список значений в поле `Show items in field`.

Пример значений:

\- Yes

\- No

\- Maybe

Разница между типами:

* `Select` — можно выбрать только один вариант
* `Multiselect` — можно выбрать несколько вариантов одновременно
{% endhint %}

</details>

<details>

<summary>Основные параметры</summary>

{% hint style="info" %}
`Field Key` - это уникальный ключ поля.

Он используется как переменная внутри системы.

Через него можно:

* передавать данные через Webhooks
* подставлять значения в Postback
* использовать поле в логике сценариев

Пример переменной:

`{{fields.refId}}`
{% endhint %}

{% hint style="warning" %}
Подробнее об использовании:

<a href="webhooks-and-api.md" class="button secondary">Webhooks &#x26; API</a> <a href="../tracker/integrations/nastroika-postback-kastomnaya-integraciya.md" class="button secondary">Настройка Postback - кастомная интеграция</a>
{% endhint %}

{% hint style="info" %}
`Name` - это название поля, которое отображается в интерфейсе.

Обычно оно видно в карточке клиента.

Примеры:

`Deposit Amount`

`User Status`

`Manager Comment`
{% endhint %}

{% hint style="info" %}
`Visible field` отвечает за отображение поля в карточке клиента.

Если опция включена:

* поле видно в CRM

Если опция выключена:

* поле скрыто из карточки клиента
{% endhint %}

</details>

### Где используются Custom Fields:

{% hint style="success" %}
**Custom Fields удобно использовать, когда нужно:**

* Хранить ID трейдера, менеджера или сделки
* Сохранять дату, сумму или статус
* Передавать параметры между внешней системой и ботом
* Показывать дополнительные данные оператору в CRM
{% endhint %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
