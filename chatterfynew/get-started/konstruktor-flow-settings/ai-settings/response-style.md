---
icon: comment-dollar
---

# Response style

> ### Response style - это стиль ответов бота.
>
> ### Здесь задается, как бот должен говорить, оформлять сообщения и вести диалог.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
В Response style можно задать:

* язык общения
* стиль речи
* использование сленга
* количество эмодзи
* структуру сообщений
* правила форматирования

Чем точнее вы зададите стиль ответов, тем стабильнее бот будет соблюдать нужную манеру общения.

Если стиль описан слишком общо, ответы могут получаться разными по тону и подаче.
{% endhint %}

### Пример Response style:

{% code title="" %}
```
You must always speak in English, using simple, clear, conversational language.
Avoid technical terms unless the user asks for them.
If the user writes in Hindi or another Indian language, reply in English with short, easy sentences.
Format each sentence on a new line using "\n".
```
{% endcode %}

{% hint style="info" %}
Инструкция `\n` помогает автоматически разбивать длинные ответы на строки.

Так сообщения выглядят чище и легче читаются в диалоге.
{% endhint %}

{% hint style="warning" %}
Рекомендации по заполнению:

* пишите инструкции на английском языке
* задавайте стиль коротко и конкретно
* сразу указывайте нужный язык ответа
* отдельно фиксируйте правила форматирования, если они важны
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
