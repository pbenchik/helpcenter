---
icon: table
---

# Delays

**Delays** задаёт задержки перед отправкой сообщений пользователю.

Эти настройки управляют скоростью реакции бота и делают диалог более естественным.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (71).png" alt=""><figcaption></figcaption></figure></div>

### Как это работает

В разделе можно настроить:

* паузу перед обработкой сообщения пользователя
* скорость ответа для **AI Reply**
* задержку для шага **Send Message**
* скорость имитации набора текста

### Response time from the lead

**Response time from the lead (sec)** — базовая задержка после последнего сообщения пользователя.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (4).png" alt=""><figcaption></figcaption></figure></div>

#### How it works

Система ждёт указанное время, прежде чем запустить следующий шаг сценария.

#### Steps / Instructions

1. Откройте **Bot Settings → Delays**.
2. Найдите поле **Response time from the lead (sec)**.
3. Укажите значение в секундах.
4. Сохраните изменения.

#### Notes

* Если указано `60 sec`, бот начнёт обработку через `60` секунд после последнего сообщения пользователя.

### AI reply speed

**AI reply speed (sec)** задаёт задержку перед ответом из шага **AI Reply**.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (5).png" alt=""><figcaption></figcaption></figure></div>

#### How it works

Эта настройка включает:

* время ожидания после сообщения пользователя
* дополнительное время на генерацию и отправку ответа

Формула:

`AI reply speed = Response time from the lead + дополнительная задержка`

#### Steps / Instructions

1. Найдите поле **AI reply speed (sec)**.
2. Укажите итоговое время ответа в секундах.
3. Сохраните изменения.

#### Notes

* Если **Response time from the lead** = `60 sec`
* и **AI reply speed** = `80 sec`
* бот подождёт `60` секунд после сообщения пользователя
* затем добавит ещё `20` секунд перед отправкой ответа
* итоговая задержка составит `80` секунд

### Send message answer speed

**Send message answer speed (sec)** задаёт задержку для шага **Send Message**.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (6).png" alt=""><figcaption></figcaption></figure></div>

#### How it works

Здесь не используется генерация ИИ.

Система отправляет заранее подготовленный текст через указанное время после последнего сообщения пользователя.

#### Steps / Instructions

1. Найдите поле **Send message answer speed (sec)**.
2. Укажите значение в секундах.
3. Сохраните изменения.

#### Notes

* Если указано `45 sec`, сообщение будет отправлено через `45` секунд после последнего сообщения пользователя.

### Typing speed

**Typing speed** задаёт скорость имитации набора текста перед отправкой сообщения.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (7).png" alt=""><figcaption></figcaption></figure></div>

#### How it works

Эта настройка влияет на то, как быстро бот «печатает» сообщение в диалоге.

#### Steps / Instructions

1. Найдите поле **Typing speed**.
2. Выберите подходящее значение.
3. Сохраните изменения.

#### Notes

* Если хотите добавить более естественную паузу, уменьшите значение **Typing speed**.
* При более низкой скорости текст будет набираться дольше.

### Когда использовать

Откройте **Delays**, если нужно:

* сделать ответы бота менее мгновенными
* добавить естественную паузу перед сообщением
* разделить скорость ответа для **AI Reply** и **Send Message**
* точнее настроить восприятие диалога пользователем

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
