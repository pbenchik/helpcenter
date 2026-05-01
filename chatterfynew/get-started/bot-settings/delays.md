---
icon: table
---

# Delays

> ### **Delays** — это настройки задержек перед отправкой сообщений пользователю.

Они позволяют управлять скоростью реакции бота и делать диалог более естественным.

{% hint style="info" %}
**Delays** содержит параметры, которые влияют на время ответа бота и поведение сообщений в диалоге.

Используется для:

* настройки паузы перед обработкой сообщения пользователя
* управления скоростью ответа AI
* настройки задержки для шага **Send Message**
* имитации набора текста
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (71).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

***

### Основные возможности:

{% hint style="info" %}
С помощью **Delays** можно настроить:

* когда бот начинает обрабатывать сообщение пользователя
* сколько времени проходит перед ответом AI
* как быстро отправляется сообщение из шага **Send Message**
* скорость имитации печати текста
{% endhint %}

***

### Важно:

<details>

<summary>1. Response time from the lead </summary>

{% hint style="info" %}
**Response time from the lead (sec)** — это время ожидания после последнего сообщения пользователя, прежде чем система начнёт запуск следующего шага сценария.

Это базовая задержка реакции на сообщение пользователя.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (4).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
Пример:

Если установлено:

* **Response time from the lead:** `60 sec`

бот начнёт обработку сообщения через `60` секунд после последнего сообщения пользователя.
{% endhint %}



</details>

<details>

<summary>2. AI reply speed</summary>

{% hint style="info" %}
**AI reply speed (sec)** — это задержка перед отправкой ответа, который сгенерирован шагом **AI Reply**.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (5).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
Она включает:

* время ожидания после сообщения пользователя
* дополнительное время на генерацию и отправку ответа

Фактически:

**AI reply speed = Response time from the lead + дополнительная задержка**
{% endhint %}

{% hint style="warning" %}
Пример:

Если указано:

* **Response time from the lead:** `60 sec`
* **AI reply speed:** `80 sec`

то:

* `60` секунд — ожидание после сообщения пользователя
* ещё `20` секунд — дополнительная задержка перед отправкой ответа

В результате сообщение будет отправлено через `80` секунд после последнего сообщения пользователя.
{% endhint %}



</details>

<details>

<summary>3. Send message answer speed</summary>

{% hint style="info" %}
**Send message answer speed (sec)** — это задержка перед отправкой сообщения для шага **Send Message**.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (6).png" alt=""><figcaption></figcaption></figure></div>

В отличие от **AI Reply**, здесь не используется генерация ИИ. Отправляется заранее подготовленный текст.
{% endhint %}

{% hint style="info" %}
Задержка отсчитывается от момента получения последнего сообщения пользователя.

Пример:

* **Send message answer speed:** `45 sec`

Сообщение будет отправлено через `45` секунд после последнего сообщения пользователя.
{% endhint %}



</details>

<details>

<summary>4. Typing speed</summary>

{% hint style="info" %}
**Typing speed** — это скорость имитации набора текста ботом перед отправкой сообщения.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (7).png" alt=""><figcaption></figcaption></figure></div>

Эта настройка влияет на то, как быстро бот «печатает» сообщение, создавая более реалистичное поведение в диалоге.
{% endhint %}

</details>

{% hint style="warning" %}
Если вы хотите, чтобы сообщения отправлялись с небольшой естественной задержкой, уменьшите значение **Typing speed**.

При более низкой скорости текст будет набираться дольше, и пользователь увидит эффект печати перед отправкой сообщения.
{% endhint %}

***

{% hint style="success" %}
**Когда использовать Delays**

Используйте эти настройки, когда нужно:

* сделать ответы бота менее мгновенными
* имитировать естественную паузу перед сообщением
* разделить скорость ответа для **AI Reply** и **Send Message**
* точнее настроить восприятие диалога пользователем
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
