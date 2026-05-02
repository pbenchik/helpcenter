---
icon: comment-dollar
---

# Response style

_Response style_ задаёт стиль ответов бота.

Здесь определяется, как бот говорит, оформляет сообщения и ведёт диалог.

### Как это работает

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure></div>

Чем точнее задан стиль, тем стабильнее манера общения.

### Что можно задать

* язык общения
* стиль речи
* использование сленга
* количество эмодзи
* структуру сообщений
* правила форматирования

### Пример

{% code title="" %}
```
You must always speak in English, using simple, clear, conversational language.
Avoid technical terms unless the user asks for them.
If the user writes in Hindi or another Indian language, reply in English with short, easy sentences.
Format each sentence on a new line using "\n".
```
{% endcode %}

### Notes

{% hint style="info" %}
Инструкция `\n` помогает автоматически разбивать длинные ответы на строки.
{% endhint %}

{% hint style="warning" %}
Пишите инструкции на английском языке, задавайте стиль коротко и сразу фиксируйте язык ответа.
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
