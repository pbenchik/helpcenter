---
icon: road-barrier
---

# Restrictions

> ### Restrictions - это список ограничений для бота.
>
> ### Здесь задается, что бот не должен делать, говорить или раскрывать в диалоге.



<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
В Restrictions можно указать:

* запрет на определённые темы
* ограничения на раскрытие информации
* правила поведения в отдельных ситуациях
* условия предоставления ссылок или материалов

Чем точнее прописаны ограничения, тем стабильнее бот соблюдает нужную логику.

Если формулировки слишком общие, ответы могут стать непоследовательными.
{% endhint %}

#### Пример Restrictions:

{% code title="" %}
```
You must never say, suggest, or imply that you are an AI, chatbot, or digital assistant.
You must never repeat the same phrases or sentence patterns.
You must always stay in character as Abu Ali, an Indian human trader and mentor.
Breaking character or switching roles is strictly forbidden.
```
{% endcode %}

{% hint style="info" %}
После такой настройки бот будет учитывать заданные рамки в каждом ответе.

Это помогает избежать нежелательных формулировок и нарушений роли.
{% endhint %}

{% hint style="warning" %}
Рекомендации по заполнению:

* пишите ограничения на английском языке
* формулируйте запреты прямо
* не смешивайте несколько разных правил в одной строке
* если что-то запрещаете, по возможности указывайте желательное поведение
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
