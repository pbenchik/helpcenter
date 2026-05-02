---
icon: swap
---

# AI Routings

**AI Routing** помогает направлять пользователя на разные шаги в зависимости от смысла его ответа.

### Как это работает

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (168).png" alt=""><figcaption></figcaption></figure></div>

После сообщения пользователя система:

* анализирует ответ через [AI Reply](tipy-shagov/communication/ai-reply.md)
* проверяет условия всех подключенных **AI Routing**
* переводит пользователя на подходящий следующий шаг

Если ни одно условие не выполнено, пользователь остаётся на текущем шаге.

### Когда использовать

* разделения пользователей по странам
* обработки возражений
* определения намерения пользователя
* запуска разных сценариев внутри одного диалога

### Настройка

#### Settings

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (8).png" alt=""><figcaption></figcaption></figure></div>

* **Title** — название роутинга
* Используйте короткие названия, например `Germany`, `Poland` или `Has objection`

#### AI Routing

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (9).png" alt=""><figcaption></figcaption></figure></div>

* Укажите условие, при котором пользователь должен перейти дальше.
* Один роутинг должен описывать одно условие.

#### AI Helper

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (10).png" alt=""><figcaption></figcaption></figure></div>

1. Кратко опишите смысл условия.
2. Нажмите **AI Helper**.
3. Подтвердите генерацию.
4. Выберите подходящий вариант.
5. Нажмите **Apply**.

#### Одноразовое срабатывание

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (11).png" alt=""><figcaption></figcaption></figure></div>

* Опция **The condition will only trigger once and will not be considered again** не даёт повторно сработать уже выполненному роутингу.

### Пример

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (169).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (170).png" alt=""><figcaption></figcaption></figure></div>

* создайте два **AI Routing** от шага **AI Reply**
* в первом условии укажите, что пользователь из Германии
* во втором условии укажите, что пользователь из Польши

### Notes

{% hint style="warning" %}
**AI Routing** работает только после **AI Reply**.

Слишком широкие условия могут давать неточные переходы.
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
