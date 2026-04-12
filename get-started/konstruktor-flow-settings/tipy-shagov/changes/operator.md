---
icon: person-simple
---

# Operator

> ### Operator - это шаг для назначения или снятия оператора у диалога.

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2260 (5).png" alt=""><figcaption></figcaption></figure></div>

С помощью Operator можно:

* распределения чатов между сотрудниками
* передачи диалога оператору
* настройки логики обработки лидов
{% endhint %}

{% hint style="warning" %}
Перед использованием шага настройте логику отображения чатов в **Bot Settings → Assign Manager**.

Именно там определяется, какие чаты увидит оператор после назначения.
{% endhint %}

### Важно:

<details>

<summary>Settings (Настройки)</summary>

{% hint style="info" %}


*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (34).png" alt=""><figcaption></figcaption></figure></div>

В блоке **Settings** задаются общие параметры шага:

* **Title** — название шага
* **Delay** — задержка перед выполнением действия
* **Finish Status** — статус диалога после шага
* **Hide keyboard** — скрывает клавиатуру из предыдущего шага
* **Is start step of flow** — делает шаг стартовым
* **Skip the transition to next step** — отключает автоматический переход дальше
{% endhint %}

{% hint style="info" %}
Во время `Delay`:

* сообщения пользователя игнорируются
* назначение не выполняется
{% endhint %}

{% hint style="warning" %}
Если используется статус `waiting`, можно включить **Skip the transition to next step**.

Тогда шаг не переключится автоматически, и система останется в текущем состоянии.
{% endhint %}

</details>

<details>

<summary>Assigns (Назначение оператора)</summary>

{% hint style="info" %}


*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (36).png" alt=""><figcaption></figcaption></figure></div>

В этом блоке настраивается действие с оператором.

Основные поля:

* **Action** — выбрать `Assign` или `Remove`
* **Operator** — выбрать оператора для назначения
* **Probability (%)** — задать вероятность распределения
* **Add action** — добавить ещё одного оператора в распределение
{% endhint %}

#### Assigns → Operator

<div data-with-frame="true"><img src="../../../../.gitbook/assets/Frame 2248 (37).png" alt=""></div>

{% hint style="success" %}
При выборе действия **Assign**:

* выбирается оператор
* можно задать `Probability (%)` для распределения чатов
{% endhint %}

{% hint style="danger" %}
При выборе действия **Remove** чат снимается с текущего оператора.

Это удобно, если нужно вернуть диалог в общий пул или передать его дальше по логике.
{% endhint %}

#### Probability (Вероятность)

{% hint style="info" %}
Probability позволяет распределять чаты между операторами.

Важно:

* суммарно должно быть 100%
* можно добавить несколько операторов
{% endhint %}

{% hint style="info" %}
Пример распределения:

* Operator 1 - 50%
* Operator 2 - 50%
{% endhint %}

</details>

<details>

<summary>Настройки в Bot Settings</summary>

{% hint style="info" %}


*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (39).png" alt=""><figcaption></figcaption></figure></div>

В разделе **Assign Manager** доступны дополнительные параметры:

* **Show all chats** — оператор видит все чаты
* **Show only assigned chats** — оператор видит только свои чаты
* **Show assigned + unassigned chats** — оператор видит свои и неназначенные чаты

Эти настройки влияют на работу операторов после назначения.
{% endhint %}

{% hint style="info" %}
Можно не только автоматически назначать чаты операторам через **Assign**, но и передавать их другому оператору или забирать у текущего через **Remove**.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (38).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
В поле Probability (Вероятность), выберите % соотношение вероятного распределения чатов для оператора. Сумма должна равняться 100%.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (40).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

</details>

### Важная логика работы:

{% hint style="warning" %}
* Назначение или снятие происходит сразу после выполнения шага
* Если задана вероятность, чат распределяется случайным образом
* Один шаг можно использовать для распределения между несколькими операторами
* Результат шага зависит и от настроек в **Assign Manager**
{% endhint %}

### Пример использования:

{% hint style="info" %}
Сценарий: распределение лидов между двумя менеджерами.

* `Operator 1` — `70%`
* `Operator 2` — `30%`

Так можно автоматически делить нагрузку внутри команды.
{% endhint %}

### Когда использовать Operator:

{% hint style="success" %}
Используйте этот шаг, когда нужно:

* передать диалог оператору
* распределить лиды между менеджерами
* снять оператора с чата
* автоматизировать работу команды
* управлять нагрузкой через проценты
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
