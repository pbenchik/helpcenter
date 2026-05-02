---
icon: person-simple
---

# Operator

**Operator** — это шаг для назначения или снятия оператора у диалога.

### Как это работает

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2260 (5).png" alt=""><figcaption></figcaption></figure></div>

Шаг используется для распределения чатов между сотрудниками и передачи диалога оператору.

### Settings

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (34).png" alt=""><figcaption></figcaption></figure></div>

* **Title**
* **Delay**
* **Finish Status**
* **Hide keyboard**
* **Is start step of flow**
* **Skip the transition to next step**

### Assigns

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (36).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><img src="../../../../.gitbook/assets/Frame 2248 (37).png" alt=""></div>

* **Action** — `Assign` или `Remove`
* **Operator** — выбор оператора
* **Probability (%)** — вероятность распределения
* **Add action** — добавляет ещё одного оператора

#### Probability

* сумма всех значений должна быть `100%`
* можно распределять чаты между несколькими операторами

Пример:

* `Operator 1` — `50%`
* `Operator 2` — `50%`

### Assign Manager

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (39).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (38).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (40).png" alt=""><figcaption></figcaption></figure></div>

В **Assign Manager** доступны режимы:

* **Show all chats**
* **Show only assigned chats**
* **Show assigned + unassigned chats**

### Notes

{% hint style="warning" %}
Перед использованием шага настройте логику отображения чатов в **Bot Settings** → **Assign Manager**.
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
