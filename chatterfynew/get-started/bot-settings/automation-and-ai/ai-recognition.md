---
icon: text-size
---

# Ai Recognition

> ### AI Recognition - это блок настроек, который отвечает за обработку входящих медиа-сообщений с помощью AI.

{% hint style="info" %}
С его помощью можно:

\- распознавать голосовые сообщения

\- анализировать изображения

\- извлекать текст и данные

\- реагировать на медиа-контент от пользователя

\- автоматически записывать найденные данные в поля
{% endhint %}

### Как открыть AI Recognition:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Перейдите в Bot Settings**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2213.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Откройте раздел AI Recognition**

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2214.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Какие типы контента поддерживаются</summary>

{% hint style="info" %}
В AI Recognition можно отдельно настраивать реакцию на разные типы медиа:

* Voice - голосовые сообщения
* Video Note - кружки
* Photo - изображения
* Video - видео
* Document - документы
{% endhint %}

</details>

<details>

<summary>Режим Recognition</summary>

{% hint style="info" %}
В режиме Recognition AI:

* анализирует содержимое медиа
* преобразует его в текст или смысл
* учитывает результат в контексте диалога
*   продолжает общение автоматически

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2256 (2).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
Этот режим нужен, когда медиа должно обрабатываться без участия оператора.
{% endhint %}

</details>

<details>

<summary>Режим Manual</summary>

{% hint style="info" %}
В режиме Manual диалог переводится на ручную обработку.
{% endhint %}

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2256 (3).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Этот вариант подходит, если:

* нужна проверка оператором
* медиа нельзя обрабатывать автоматически
* требуется ручное решение по диалогу
{% endhint %}

</details>

<details>

<summary>Режим Skip</summary>

{% hint style="info" %}
В режиме Skip AI:

* <mark style="color:$primary;">игнорирует сообщение</mark>
* <mark style="color:$primary;">не учитывает его в контексте</mark>
*   <mark style="color:$primary;">продолжает диалог без изменений</mark>

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2256 (4).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
Этот режим удобен, когда медиа не должно влиять на сценарий.
{% endhint %}

</details>

<details>

<summary>Ограничения по типам</summary>

{% hint style="warning" %}
**На текущий момент:**

* Voice, Video Note и Photo поддерживают `Recognition`, `Manual` и `Skip`
* Video и Document поддерживают только `Manual` и `Skip`
{% endhint %}

</details>

<details>

<summary>Как работает распознавание голосовых сообщений</summary>

{% hint style="info" %}
При включенном Recognition:

* AI преобразует голос в текст
* понимает смысл сообщения
* отвечает так, как если бы пользователь написал текст
{% endhint %}

{% hint style="info" %}
Это позволяет автоматизировать работу с голосовыми сообщениями без ручной расшифровки.
{% endhint %}

</details>

<details>

<summary>Как работает распознавание изображений</summary>

{% hint style="info" %}
AI может:

* определять содержимое изображения
* распознавать текст
* понимать контекст скриншотов и интерфейсов
* извлекать конкретные данные
{% endhint %}

</details>

<details>

<summary>Tasks (Instructions)</summary>

{% hint style="info" %}
Tasks - это инструкции для AI, что именно искать на изображении.

Они помогают повысить точность распознавания и задать нужный контекст.
{% endhint %}

{% hint style="info" %}
Для добавления нажмите `Add task` и укажите инструкцию.

Примеры:

* Find user ID from Exnova
* Find product name on the image
* Find user's country on 1Win
{% endhint %}

</details>

<details>

<summary>Functions</summary>

{% hint style="info" %}
Functions позволяют выполнять действия на основе найденной информации.

Например, записывать данные в Custom Fields.
{% endhint %}

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2256 (5).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Для добавления функции нужно указать:

* Action - действие, например `Write`
* Field - кастомное поле
* Value - тип данных, например `ID`, `Country`, `Amount`
* Prompt - что именно нужно найти
{% endhint %}

{% hint style="info" %}
Пример настройки:

* Task: Find user ID from Exnova
* Action: Write
* Field: Exnova ID
* Value: ID
* Prompt: User ID from Exnova
{% endhint %}

{% hint style="info" %}
В результате AI найдёт ID на изображении и автоматически запишет его в нужное поле.
{% endhint %}

</details>

<details>

<summary>Пример сценария</summary>

{% hint style="info" %}
Пример работы:

* пользователь отправляет скриншот
* AI распознаёт нужные данные
* сохраняет их в Custom Fields
* диалог продолжается по сценарию
{% endhint %}

</details>

### Где удобно использовать AI Recognition:

{% hint style="success" %}
AI Recognition особенно полезен, когда пользователи отправляют:

* голосовые сообщения
* скриншоты
* подтверждения
* документы и медиа для проверки
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
