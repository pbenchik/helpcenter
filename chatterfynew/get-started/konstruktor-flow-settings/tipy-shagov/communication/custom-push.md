---
icon: gears
---

# Custom push

**Custom Push** — это шаг для отправки отложенных сообщений, если пользователь не отвечает.

Он помогает вернуть пользователя в диалог и продолжить догрев без участия оператора.

### Как это работает

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2139 (7).png" alt=""><figcaption></figcaption></figure></div>

Пуши работают, пока пользователь не ответил.

### Settings

* **Title** — название шага
* **Delay ms** — задержка перед запуском пушей
* **Finish Status** — статус после выполнения шага

Доступные статусы:

* `nothing`
* `auto`
* `waiting`
* `manual`
* `blocked`
* `finished`

### Push Messages

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (55).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (56).png" alt=""><figcaption></figcaption></figure></div>

Можно использовать:

* **Text**
* **Media**
* **Document**
* **Video note**
* **Voice**

Варианты настройки:

* **Global push messages** — берутся из настроек бота
* **Step push messages** — настраиваются вручную внутри шага

### Notes

{% hint style="danger" %}
Обычно для **Custom Push** используют статус `waiting`.

Если нужен догрев без перехода дальше, включайте **Skip the transition to next step**.
{% endhint %}

{% hint style="warning" %}
Пуши не отправляются во время `Delay ms`.

Если пользователь ответил, цепочка пушей останавливается.
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
