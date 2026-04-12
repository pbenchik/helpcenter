---
icon: head-side-circuit
---

# AI Settings

> ### AI Settings - это раздел общих настроек бота.
>
> ### Здесь задается его роль, правила поведения и стиль общения с пользователями.

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure></div>
*   Эти настройки формируют личность бота, ограничения в диалоге и формат ответов.

    Именно они напрямую влияют на качество коммуникации с пользователем.
{% endhint %}

{% hint style="warning" %}
Все инструкции в AI Settings должны быть написаны на английском языке.

Это относится к следующим полям:

* Global legend
* Restrictions
* Response style

Это правило также действует для любых других промптов внутри AI Settings.
{% endhint %}

### Как AI Settings учитывает эти настройки

{% hint style="info" %}
1. Учитывает AI Settings - роль бота, поведение и стиль общения.
2. Учитывает историю диалога - прошлые сообщения пользователя и бота.
3. Учитывает промпты текущего шага AI Reply - цель и инструкции для конкретного ответа.

<mark style="color:$warning;">На основе этих данных ИИ формирует сообщение пользователю.</mark>
{% endhint %}

{% hint style="info" %}
После нового сообщения пользователя ИИ анализирует диалог и проверяет:

* выполнены ли условия <mark style="color:$warning;">Requirements</mark>
* срабатывают ли правила <mark style="color:$warning;">AI Routing</mark>

После этого система либо продолжает диалог на текущем шаге, либо переводит пользователя дальше.
{% endhint %}

{% hint style="info" %}
Для детальной настройки отдельных блоков используйте:

&#x20;<a href="global-legend.md" class="button secondary">Global legend</a><a href="restrictions.md" class="button secondary">Restrictions</a> <a href="response-style.md" class="button secondary">Response style</a> <a href="../tipy-shagov/communication/ai-reply.md" class="button secondary">AI Reply</a>
{% endhint %}

### Важные инструкции можно усиливать внутри текста:

{% hint style="warning" %}
Например:

`IMPORTANT: Always guide the user to register before discussing payment.`

Также можно использовать <mark style="color:$warning;">**CAPS**</mark>, если нужно показать высокий приоритет правила.
{% endhint %}

{% hint style="info" %}
Приоритет инструкций зависит от их порядка.

Модель обрабатывает текст сверху вниз.

Правила, которые стоят ближе к началу блока, обычно сильнее влияют на поведение бота.
{% endhint %}

### Улучшение работы ИИ:

{% hint style="info" %}
ИИ лучше работает, когда инструкции содержат конкретные примеры поведения.

Пример:

`If the user says "I don't have money", respond with: "Do you really want to miss the chance to change your life?"`

Чем конкретнее формулировка, тем стабильнее ответы.
{% endhint %}

{% hint style="info" %}
Не оставляйте правило только в форме запрета.

Лучше сразу указывать, какое поведение должно быть вместо него.

Не рекомендуется:

`Do not say you don't know the answer.`

Лучше писать так:

`Do not say you don't know the answer. Instead, suggest checking the information together or offer to clarify the question.`
{% endhint %}

{% hint style="success" %}
Такой подход делает поведение бота более предсказуемым.

ИИ понимает не только, что запрещено, но и какой ответ считается правильным.

Это помогает избежать пустых, слабых или неуверенных ответов.
{% endhint %}

### Подробнее про настройки AI Settings:

{% hint style="info" %}
<a href="global-legend.md" class="button secondary">Global legend</a><a href="restrictions.md" class="button secondary">Restrictions</a> <a href="response-style.md" class="button secondary">Response style</a> <a href="../tipy-shagov/communication/ai-reply.md" class="button secondary">AI Reply</a>
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
