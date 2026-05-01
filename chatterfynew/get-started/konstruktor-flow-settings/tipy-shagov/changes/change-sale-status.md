---
icon: right-left-large
---

# Change sale status

> ### Change sale status - это шаг для присвоения пользователю sale status.

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2260 (6).png" alt=""><figcaption></figcaption></figure></div>

С помощью Change sale status можно:

* Сегментировать пользователей
* Отслеживать этапы воронки
* Обновлять текущий статус лида
{% endhint %}

{% hint style="warning" %}
Перед использованием шага создайте статусы в **Bot Settings → Sale status**.

Без этого выбрать нужный статус в настройках шага не получится.
{% endhint %}

### Как работает Change sale status:

{% hint style="info" %}
После выполнения шага система:

* присваивает пользователю выбранный статус
* заменяет предыдущий статус новым
* обновляет состояние лида для дальнейшей логики
{% endhint %}

<details>

<summary>Settings (Настройки)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (41).png" alt=""><figcaption></figcaption></figure></div>

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
* статус не изменяется
{% endhint %}

{% hint style="warning" %}
Если используется статус `waiting`, можно включить **Skip the transition to next step**.

Тогда шаг не переключится автоматически, и система останется в текущем состоянии.
{% endhint %}



</details>

<details>

<summary>Sale status (Статус)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (42).png" alt=""><figcaption></figcaption></figure></div>

В этом блоке выбирается статус, который будет присвоен пользователю.

Основное поле:

* **Choose sale status** — выбор статуса из списка
{% endhint %}

{% hint style="info" %}
Если список пуст, сначала создайте статусы в **Bot Settings → Sale status**.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (43).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

### Важная логика работы:

{% hint style="warning" %}
* Статус применяется сразу после выполнения шага
* Новый статус заменяет предыдущий
* У пользователя может быть только один текущий sale status
* Этот статус можно использовать в фильтрах и логике воронки
{% endhint %}

### Пример использования:

{% hint style="info" %}
Сценарии:

* пользователь прошёл регистрацию → `Registration`
* пользователь сделал депозит → `Sale`
* пользователь сделал повторный депозит → `Resale`
{% endhint %}

### Когда использовать Change sale status:

{% hint style="success" %}
Используйте этот шаг, когда нужно:

* отслеживать этапы воронки
* сегментировать пользователей по статусам
* обновлять текущее состояние лида
* использовать sale status в дальнейшей логике
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
