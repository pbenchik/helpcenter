---
description: Шаг для отправки готовых сообщений, медиа, файлов и пушей.
icon: envelope-circle-check
---

# Send message

**Send message** — это шаг для отправки готовых сообщений.

Здесь можно отправлять текст, медиа, файлы, голосовые, видеокружки и сообщения с кнопками.

### Как это работает

<div align="center" data-full-width="false" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2139 (5).png" alt=""><figcaption></figcaption></figure></div>

Шаг подходит для фиксированных сообщений, инструкций и догрева.

### Что можно отправлять

* **Text** — готовый текст
* **Prompt** — текст по вашему запросу
* **Media** — фото, видео, скриншоты
* **Document** — файлы и документы
* **Video Note** — видеокружки
* **Voice** — голосовые сообщения

### Settings

<img src="../../../../.gitbook/assets/Frame 2248 (45).png" alt="" data-size="original">

* **Title** — название шага
* **Delay** — задержка от предыдущего шага до отправки
* **Finish Status** — статус диалога после выполнения шага
* **Skip the transition to next step** — отключает автоматический переход
* **Hide keyboard** — скрывает клавиатуру у пользователя
* **Is start step of flow** — делает шаг стартовым

### Manual Messages

<img src="../../../../.gitbook/assets/Frame 2248 (46).png" alt="" data-size="original">

* **Inline Buttons** прикрепляются к сообщению
* **Keyboard** отображается снизу в чате
* сообщения отправляются по очереди
* можно комбинировать разные типы в одну цепочку
* **Pin message** закрепляет сообщение в диалоге

### Push Messages

* **Global push messages** — используются глобальные пуши бота
* **Step push messages** — пуши настраиваются внутри текущего шага
* каждый следующий пуш отправляется после предыдущего
* если пользователь ответил, пуши останавливаются

### Notes

{% hint style="warning" %}
Если вы используете статус `waiting` и пуши, включите **Skip the transition to next step**.
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
