---
icon: head-side-circuit
---

# AI Settings

_AI Settings_ — это раздел общих настроек бота.

Здесь задаются роль бота, ограничения и стиль общения.

### Как это работает

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure></div>

Эти настройки формируют личность бота, правила поведения и формат ответов.

{% hint style="warning" %}
Все инструкции в **AI Settings** должны быть написаны на английском языке.

Это относится к полям **Global legend**, **Restrictions** и **Response style**.
{% endhint %}

### Что учитывает система

1. **AI Settings** — роль, поведение и стиль общения.
2. Историю диалога — прошлые сообщения пользователя и бота.
3. Настройки шага [AI Reply](../tipy-shagov/communication/ai-reply.md).

После нового сообщения пользователя система проверяет:

* выполнены ли условия `Requirements`
* срабатывают ли правила [AI Routings](../ai-routings.md)

### Рекомендации по заполнению

* ставьте самые важные правила выше по тексту
* формулируйте инструкции коротко и конкретно
* добавляйте примеры нужного поведения
* не оставляйте правило только в форме запрета

Пример:

```
Do not say you don't know the answer.
Instead, suggest checking the information together or offer to clarify the question.
```

### Notes

{% hint style="info" %}
Важные инструкции можно усиливать формулировками вроде `IMPORTANT:` и конкретными примерами ответа.
{% endhint %}

### Связанные страницы

* [Global legend](global-legend.md)
* [Restrictions](restrictions.md)
* [Response style](response-style.md)
* [AI Reply](../tipy-shagov/communication/ai-reply.md)

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
