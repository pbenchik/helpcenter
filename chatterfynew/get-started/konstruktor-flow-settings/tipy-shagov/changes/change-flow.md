---
icon: arrow-progress
---

# Change flow

**Change flow** переводит пользователя в другой _flow_.

Здесь выбирается сценарий и конкретный шаг, с которого продолжится диалог.

### Как это работает

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2260 (4).png" alt=""><figcaption></figcaption></figure></div>

1. Система доходит до шага **Change Flow**.
2. Берёт _flow_, который выбран в настройках.
3. Переводит пользователя на указанный шаг внутри этого _flow_.
4. Продолжает диалог уже в новом сценарии.

### Settings

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (108).png" alt=""><figcaption></figcaption></figure></div>

* **Title**
* **Delay**
* **Finish Status**
* **Hide keyboard**
* **Is start step of flow**
* **Skip the transition to next step**

### Flow

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (66).png" alt=""><figcaption></figcaption></figure></div>

* **Choose flow** — выбор _flow_
* **Choose step** — выбор шага внутри него

### Notes

{% hint style="warning" %}
После выполнения шага текущий сценарий прекращается.

Если выбрать не тот _flow_ или не тот шаг, пользователь попадёт в неправильную часть воронки.
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
