---
icon: swap
---

# A/B router

> ### A/B router - это шаг, который позволяет случайным образом распределять пользователей по разным веткам сценария.

{% hint style="info" %}
**AB Router - проведение A/B тестов, позволит вам в одном боте и одном скрипте распределять пользователей в процентном соотношении по разными флоу.**

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

### Структура шага:

<details>

<summary>1. Settings (Настройки)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (21).png" alt=""><figcaption></figcaption></figure></div>

**Title**\
<mark style="color:$primary;">Название шага.</mark>\ <mark style="color:$primary;">Используется для удобной навигации внутри flow.</mark>

***

**Delay**\
<mark style="color:$primary;">Задержка перед выполнением шага.</mark>\ <mark style="color:$primary;">Во время задержки:</mark>

* <mark style="color:$primary;">сообщения пользователя игнорируются</mark>
* <mark style="color:$primary;">действие не выполняется</mark>

***

**Finish Status**\
<mark style="color:$primary;">Статус диалога после выполнения шага.</mark>\ <mark style="color:$primary;">Варианты:</mark>

* <mark style="color:$primary;">**nothing**</mark> <mark style="color:$primary;"></mark><mark style="color:$primary;">- переход к следующему шагу</mark>
* <mark style="color:$primary;">**auto**</mark> <mark style="color:$primary;"></mark><mark style="color:$primary;">- автоматическое продолжение диалога</mark>
* <mark style="color:$primary;">**waiting**</mark> <mark style="color:$primary;"></mark><mark style="color:$primary;">- ожидание ответа пользователя</mark>
* <mark style="color:$primary;">**manual**</mark> <mark style="color:$primary;"></mark><mark style="color:$primary;">- перевод на оператора</mark>
* <mark style="color:$primary;">**blocked**</mark> <mark style="color:$primary;"></mark><mark style="color:$primary;">- блокировка диалога</mark>
* <mark style="color:$primary;">**finished**</mark> <mark style="color:$primary;"></mark><mark style="color:$primary;">- завершение диалога</mark>

***

**Hide keyboard**\
<mark style="color:$primary;">Скрывает клавиатуру из предыдущего шага.</mark>

***

**Is start step of flow**\
<mark style="color:$primary;">Отмечает шаг как стартовый.</mark>

***

Skip the transition to next step

<mark style="color:$primary;">Отключает автоматический переход на следующий шаг.</mark>

<mark style="color:$primary;">Используется в связке со статусом waiting.</mark>

<mark style="color:$primary;">Если опция включена:</mark>

* <mark style="color:$primary;">шаг не переключится автоматически</mark>
* <mark style="color:$primary;">система останется на текущем шаге</mark>
* <mark style="color:$primary;">будет ожидать ответ пользователя</mark>
{% endhint %}

</details>

<details>

<summary>Распределение трафика</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/unknown (50).jpeg" alt=""><figcaption></figcaption></figure></div>

После создания шага необходимо:

* <mark style="color:$primary;">провести линии к нужным шагам</mark>
* <mark style="color:$primary;">задать процент распределения для каждой линии</mark>

Сумма всех веток должна быть равна 100%
{% endhint %}

</details>

<details>

<summary>Пример использования</summary>

{% hint style="info" %}
**Сценарий: тест двух сообщений**

<mark style="color:$primary;">Шаг 1 - 50%</mark>\ <mark style="color:$primary;">→ сообщение с оффером A</mark>

<mark style="color:$primary;">Шаг 2 - 50%</mark>\ <mark style="color:$primary;">→ сообщение с оффером B</mark>
{% endhint %}

</details>

### Используется для:

{% hint style="info" %}
* <mark style="color:$primary;">A/B тестирования</mark>
* <mark style="color:$primary;">сравнения эффективности сценариев</mark>
* <mark style="color:$primary;">распределения трафика</mark>
* <mark style="color:$primary;">оптимизации воронки</mark>
{% endhint %}

### Важно перед началом:

{% hint style="warning" %}
<mark style="color:$primary;">Перед использованием шага необходимо определить:</mark>

* <mark style="color:$primary;">какие сценарии вы хотите протестировать</mark>
* <mark style="color:$primary;">как будет распределяться трафик между ними</mark>
{% endhint %}

### Основные возможности:

{% hint style="info" %}
С <mark style="color:$primary;">помощью A/B router вы можете:</mark>

* <mark style="color:$primary;">распределять пользователей по разным веткам</mark>
* <mark style="color:$primary;">задавать процент распределения</mark>
* <mark style="color:$primary;">тестировать разные сообщения и сценарии</mark>
* <mark style="color:$primary;">анализировать эффективность</mark>
{% endhint %}

### Важная логика работы:

{% hint style="warning" %}
<mark style="color:$primary;">Проценты задаются на переходах (линиях), а не внутри шага</mark>\ <mark style="color:$primary;">Распределение происходит в момент выполнения шага</mark>\ <mark style="color:$primary;">Один пользователь попадает только в одну ветку</mark>\ <mark style="color:$primary;">Пользователь случайным образом попадает в одну из веток</mark>
{% endhint %}

### Когда использовать A/B router:

{% hint style="success" %}
**Используйте этот шаг, когда нужно:**

* <mark style="color:$primary;">протестировать разные сценарии</mark>
* <mark style="color:$primary;">сравнить конверсию</mark>
* <mark style="color:$primary;">оптимизировать воронку</mark>
* <mark style="color:$primary;">распределить трафик между вариантами</mark>
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
