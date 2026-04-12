---
icon: swap
---

# AI Routings

> ### **AI Routing** помогает направлять пользователя на разные шаги в зависимости от смысла его ответа.

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (168).png" alt=""><figcaption></figcaption></figure></div>

**Используется для:**

* разделения пользователей по странам
* обработки возражений
* определения намерения пользователя
* запуска разных сценариев внутри одного диалога
{% endhint %}

{% hint style="info" %}
**После сообщения пользователя система:**

* анализирует ответ через AI Reply
* проверяет условия всех подключенных AI Routing
* переводит пользователя на подходящий следующий шаг

Если ни одно условие не выполнено, пользователь остается на текущем шаге.
{% endhint %}

### Важно перед началом:

{% hint style="warning" %}
**Перед настройкой AI Routing нужно заранее понять:**

* какие сценарии вы хотите разделить
* какие ответы пользователя считаются подходящими
* какие переходы должны срабатывать после AI Reply
{% endhint %}

<details>

<summary>Основные возможности</summary>

{% hint style="info" %}
**С помощью AI Routing вы можете:**

* направлять пользователя по разным веткам
* выделять конкретные намерения в ответах
* обрабатывать разные типы возражений
* строить гибкую логику после AI Reply
{% endhint %}



</details>

<details>

<summary>1. Settings (Настройки)</summary>

{% hint style="info" %}
**Title**\
Название роутинга.\
Используется для удобной навигации внутри flow.

Лучше использовать короткие и понятные названия:

* Germany
* Poland
* Has objection
* Ready for registration
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (8).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>2. AI Routing</summary>

{% hint style="info" %}
**Здесь задается условие, при котором пользователь должен перейти на следующий шаг.**

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (9).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>Condition</summary>

{% hint style="info" %}
**Condition** - это логика перехода на следующую ветку.

Пишите условие:

* <mark style="color:$danger;">**Кратко**</mark>
* <mark style="color:$danger;">**Конкретно**</mark>
* <mark style="color:$danger;">**Без смешивания нескольких сценариев в одном роутинге**</mark>

Чем точнее условие, тем стабильнее переход.
{% endhint %}



</details>

<details>

<summary>AI Helper</summary>

{% hint style="info" %}
Если не хотите прописывать условие вручную, используйте AI Helper.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (10).png" alt=""><figcaption></figcaption></figure></div>

**Как это работает:**

* кратко опишите смысл условия в поле Condition
* нажмите кнопку AI Helper
* подтвердите генерацию
* получите 2 варианта условия
* выберите подходящий вариант
* нажмите Apply

**После этого новое условие заменит предыдущее.**
{% endhint %}



</details>

<details>

<summary>The condition will only trigger once and will not be considered again</summary>

{% hint style="info" %}
**Эта настройка не дает пользователю повторно перейти по уже отработанному AI Routing.**

**Используйте её, если переход по этой ветке должен сработать только один раз.**

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (11).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>Пример использования</summary>

{% hint style="info" %}
Сценарий: нужно определить страну пользователя и перевести его на нужную ветку.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (169).png" alt=""><figcaption></figcaption></figure></div>

Что нужно сделать:

* создать два AI Routing от шага AI Reply
* в первом роутинге указать условие: пользователь сказал, что он из Германии
* во втором роутинге указать условие: пользователь сказал, что он из Польши
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (170).png" alt=""><figcaption></figcaption></figure></div>

Результат:

* если пользователь сказал, что он из Германии - сработает первый роутинг
* если пользователь сказал, что он из Польши - сработает второй роутинг
* если пользователь назвал другую страну - он останется на текущем шаге
{% endhint %}



</details>

### Важная логика работы:

{% hint style="warning" %}
* **AI Routing работает после шага AI Reply**
* Один роутинг должен описывать одно условие
* Слишком широкие условия могут давать неточные переходы
* Если ни одно условие не подошло, пользователь остается на текущем шаге
{% endhint %}

### Когда использовать AI Routing:

{% hint style="success" %}
Используйте этот инструмент, когда нужно:

* разделить пользователей по смыслу ответа
* вести разные сценарии после AI Reply
* обрабатывать намерения и возражения
* точнее управлять переходами внутри flow
{% endhint %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
