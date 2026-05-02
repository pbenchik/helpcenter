---
icon: brain-circuit
---

# AI Reply

**AI Reply** генерирует ответы с помощью нейросети во время общения с пользователем.

Он учитывает легенду, инструкции, правила и условия перехода.

### Как это работает

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2139 (6).png" alt=""><figcaption></figcaption></figure></div>

**AI Reply** срабатывает только при входящем сообщении пользователя.

Переход на следующий шаг происходит при выполнении `Requirements`.

### Settings

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (50).png" alt=""><figcaption></figcaption></figure></div>

* **Title** — название шага
* **Delay** — задержка перед выполнением
* **Finish Status** — обычно не требуется задавать вручную
* **Hide keyboard** — скрывает клавиатуру из предыдущего шага
* **Is start step of flow** — делает шаг стартовым
* **Skip the transition to next step** — оставляет систему на текущем шаге

### Блоки AI Reply

#### Goal

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure></div>

* задаёт цель общения на текущем шаге

#### Requirements

<figure><img src="../../../../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure>

* определяет условие перехода на следующий шаг
* формулируйте условие так, чтобы на него можно было ответить `YES` или `NO`
* если используются [AI Routings](../../ai-routings.md), этот блок не используется

#### Legend

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure></div>

* добавляет легенду только для этого шага
* не дублируйте здесь то, что уже задано в **AI Settings**

#### Reply Addition Info

<figure><img src="../../../../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

* добавляет дополнительные вводные для финального ответа

#### Skip transition blocking on first run

<img src="../../../../.gitbook/assets/image (63).png" alt="" data-size="original">

* если опция включена, пользователь перейдёт дальше без ответа от ИИ, когда условие уже выполнено
* если опция выключена, ИИ всё равно отправит сообщение перед переходом

### Push Messages

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (53).png" alt=""><figcaption></figcaption></figure></div>

* **Global push messages** — берутся из глобальных настроек
* **Step push messages** — настраиваются внутри шага

### Где посмотреть примеры

1. Перейдите в компанию Chatterfy.
2. Откройте `Demo space`.
3. Выберите любого бота.
4. Перейдите в **Flow Settings**.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (51).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/unknown (16).jpeg" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (52).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/unknown (18).jpeg" alt=""><figcaption></figcaption></figure></div>

### Notes

{% hint style="danger" %}
В **AI Reply** логика перехода строится через `Requirements`, а не через **Finish Status**.
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
