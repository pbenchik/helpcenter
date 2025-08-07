# AI Settings

**AI Rules & Restrictions** — это общие настройки бота, где вы добавляете его легенду, инструкции по поведению и формируете модель его взаимодействий и ответов.

{% hint style="success" %}
Все нужно писать на английском языке: ai settings (global, goal, user restriction, requirement), промпты также на английском.
{% endhint %}

1\) **Global Legend - это** информация о том кто бот такой, как его зовут, чем занимается/какие услуги предоставляет, с кем он общается, ссылки и тд.

{% hint style="info" %}
**Например:**

\
-Your name is Zoolander, 40 years old, proffesional model from US, living in Europe.

-You're teaching people how to do the "Magnum look".

-User can learn from you how to do the "Magnum look", but first they need to register on your website and make a donation of $1,000,000.
{% endhint %}

И бот будет верить в то что он Зуландер 😄 Чем точнее инструкции тем качественнее ответы

<figure><img src="../../.gitbook/assets/CleanShot 2024-09-24 at 16.59.43@2x.png" alt=""><figcaption></figcaption></figure>

**2) Global Restrictions -** это все ограничения которые должен соблюдать бот при общении с юзером, что он может, при каких условиях и что ему запрещено.

{% hint style="info" %}
**Например:**\
\
-Never admit you're a bot or AI or something inanimate, always answer that you're a real person.\
**-**&#x49;f a user asks for feedback/proof on the effectiveness of your training, provide them with this link: 'supermagnumlook.com'.

-If a user says he doesn't have enought money, convince him to borrow it from his friends, since your training is worth it.
{% endhint %}

{% hint style="warning" %}
Не забывайте, что ИИ очень логичен. Если вы не получаете нужного ответа, на 99% проблема в инструкциях.&#x20;
{% endhint %}

Если есть лазейки или несоответствия в условиях, будет сложно добиться правильного результата. Например, бот может попросить оплату без упоминания регистрации или отклониться от скрипта.

3\) **User Restriction -** это инструкция на каком языке должен/не дожен общаться бот, какие эмодзи он может использовать, в каком стиле вести диалог и тд.

{% hint style="info" %}
**Например:**\
\
**-**&#x55;se English for communication, unless I ask for another language.&#x20;

-Use slang and "bro" for a friendly vibe. &#x20;

-Avoid repeating the same questions.&#x20;

-Include 1-2 emoji (💥🔥🚀🎯🦁) in your messages.

-Format each response on a new line with "\n".
{% endhint %}

Последняя инструкция отвечает за автоматическую разбивку сообщений сгенерированных ИИ в случае если оно имеет много предложений.



4\) **Extra summary prompt** - не задействован

## FAQ - Часто задаваемые вопросы 📍

### 1) Бот обучается за счет инпута клиентов?

{% hint style="info" %}
Не совсем, бот работает в рамках ваших GOALS и REQUIREMENTS + AI Settings
{% endhint %}

**В конечном счете перед генерацией ответа ИИ знает:**

1. Все из AI Settings, кто он, что он, как общаться должен и тд
2. Историю диалога
3. Задачу этого ответа (Goals)

После каждого ответа ИИ анализирует диалог и проверяет выполнение REQUIREMENTS, может ли ИИ двигаться дальше и выполнено ли условие. Представь в мыслях вопрос самому себе: я знаю о лиде такое то, он написал такое то, условие к переходу на следующий шаг такие. \


Условия выполнены? Да/нет

* Если нет - то он берет goals и снова пытается достичь цели Если да - диалог уходит на следующий шаг

{% hint style="warning" %}
Из этого следует: \
\
Если ИИ перепрыгивает на следующий шаг (технический степ) не достигнув цели - редактируете Requirements и ужесточаете требования

Если пишет не дожимая до нужной цели: дописываете Goals, добавляя ему разные ситуации как делать, что не делать и тд. чем четче сформулирована цель в первых двух предложениях, тем лучше. **Не забывайте пользоваться КАПСОМ, ИИ понимает, что это важно, либо прям написать: ВАЖНО: делай так то так**
{% endhint %}

{% hint style="success" %}
Очень круто работают примеры: Если лид пишет «нет денег», то ответь что-то типа «Ты что, не хочешь изменить жизнь?» и тд
{% endhint %}

