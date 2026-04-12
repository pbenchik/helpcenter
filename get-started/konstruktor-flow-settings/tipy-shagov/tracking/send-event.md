---
icon: left-from-bracket
---

# Send event

> ### Send event - это шаг, который позволяет отправить событие в трекер.

{% hint style="info" %}
**Используется для:**

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (67).png" alt=""><figcaption></figcaption></figure></div>
* передачи событий по пользователю
* отслеживания конверсий по кампаниям
{% endhint %}

### Важно перед началом:

{% hint style="warning" %}
Событие отправляется в трекер и привязывается к пользователю автоматически.

* Если пользователь пришёл по рекламной кампании - событие будет зафиксировано в соответствующей кампании.
* Если пользователь органический - событие отобразится в органической кампании.
{% endhint %}

### Важно:

<details>

<summary>Основные возможности</summary>

{% hint style="info" %}
**С помощью Send event вы можете:**

* отправлять события в трекер
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (68).png" alt=""><figcaption></figcaption></figure></div>
* фиксировать действия пользователя (subscribe, registration, sale и resale)
* использовать события для аналитики и отслеживания конверсий
{% endhint %}



</details>

<details>

<summary>1.Settings (Настройки)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (70).png" alt=""><figcaption></figcaption></figure></div>

**Title**\
Название шага.\
Используется для удобной навигации внутри flow.

***

**Delay**\
Задержка перед выполнением шага.\
Во время задержки:

* сообщения пользователя игнорируются
* действие не выполняется

***

**Finish Status**\
Статус диалога после выполнения шага.\
Варианты:

* nothing - переход к следующему шагу
* auto - автоматическое продолжение диалога
* waiting - ожидание ответа пользователя
* manual - перевод в ручной режим
* blocked - блокировка диалога
* finished - завершение диалога

***

**Hide keyboard**\
Скрывает клавиатуру из предыдущего шага.

***

**Is start step of flow**\
Отмечает шаг как стартовый.

***

Skip the transition to next step

Отключает автоматический переход на следующий шаг.

Используется в связке со статусом waiting.

Если опция включена:

* шаг не переключится автоматически
* система останется на текущем шаге
* будет ожидать ответ пользователя
{% endhint %}



</details>

<details>

<summary>2.Event (Событие)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (69).png" alt=""><figcaption></figcaption></figure></div>

**Здесь выбирается событие, которое будет отправлено в трекер.**

Event type - выбор типа события из списка:

* Subscribe - подписка пользователя
* Registration - регистрация пользователя
* Deposit (sale) - депозит пользователя
* Redeposit (resale) - повторный депозит
{% endhint %}



</details>

### Важная логика работы:

{% hint style="warning" %}
**Событие отправляется сразу после выполнения шага**\
Событие передаётся в трекер с привязкой к пользователю и кампании\
Передача происходит по clickid\
Событие фиксируется в аналитике
{% endhint %}

### Пример использования:

{% hint style="info" %}
**Сценарий 1: пользователь зарегистрировался**

Send event → Registration\
→ событие регистрации отправится в трекер

***

**Сценарий 2: пользователь сделал депозит**

Send event → Deposit\
→ событие депозита отправится в трекер
{% endhint %}

### Когда использовать Send event:

{% hint style="success" %}
**Используйте этот шаг, когда нужно:**

* передать событие в трекер
* фиксировать действия пользователя
* строить аналитику
* отслеживать конверсии
{% endhint %}



{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
