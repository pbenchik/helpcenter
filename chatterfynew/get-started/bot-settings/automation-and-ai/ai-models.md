---
icon: hexagon-nodes
---

# AI Models

> ### AI Models - это раздел, где выбираются модели для логики бота и генерации ответов.

{% hint style="info" %}
С его помощью можно:

* отдельно выбирать модель для логики бота
* отдельно выбирать модель для генерации ответов
* балансировать качество, скорость и стоимость
* настраивать креативность ответов
*

    <figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

### Как работает AI Models:

{% hint style="info" %}
В Chatterfy AI выполняет две разные задачи:

* логика и память диалога
* генерация ответа пользователю
{% endhint %}

{% hint style="info" %}
Поэтому модели можно разделять.

Это помогает точнее настраивать поведение бота.
{% endhint %}

### Как открыть AI Models:

{% stepper %}
{% step %}
{% hint style="info" %}
* **Перейдите в Bot Settings**
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Откройте раздел Automation & AI**
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* **Выберите блок AI Models**
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>AI Summary and Router</summary>

{% hint style="info" %}
*

    <figure><img src="../../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

Эта модель отвечает за:

* логику переходов между шагами
* работу роутеров и развилок
* память и контекст диалога
* выбор следующего действия в сценарии
{% endhint %}

{% hint style="info" %}
Если бот выбирает не тот шаг или ломает логику воронки, чаще всего причина здесь.
{% endhint %}

</details>

<details>

<summary>AI Reply</summary>

{% hint style="info" %}
* ![](<../../../.gitbook/assets/image (21).png>)

Эта модель отвечает за конечный текст ответа.

Она учитывает:

* инструкции в [AI Settings](../../konstruktor-flow-settings/ai-settings/)
* промпты в шаге AI Reply
{% endhint %}

{% hint style="info" %}
Если логика работает нормально, но ответы слабые, сухие или неточные, стоит менять именно эту модель.
{% endhint %}

</details>

<details>

<summary>Following instructions or creativity</summary>

{% hint style="info" %}
*

    <figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

Этот параметр задаёт баланс между точностью и свободой формулировок.

* `0` — ответы более строгие и предсказуемые
* `1` — ответы более живые и вариативные
{% endhint %}

{% hint style="info" %}
Чем выше значение, тем больше свободы у модели при формулировке ответа.
{% endhint %}

</details>

<details>

<summary>Как выбрать модель</summary>

{% hint style="info" %}
Если бот ошибается в переходах, путает шаги или плохо держит контекст:

* усильте модель для AI Summary and Router
{% endhint %}

{% hint style="info" %}
Если логика работает правильно, но не нравится качество текста:

* смените модель для AI Reply
{% endhint %}

{% hint style="info" %}
Если нужен баланс по бюджету:

* оставьте сильную модель для логики
* используйте более простую модель для ответов
{% endhint %}

</details>

<details>

<summary>Важные особенности</summary>

{% hint style="warning" %}
**Важно:**

* для AI Summary and Router и AI Reply можно выбирать разные модели
* после смены модели лучше проверить логику и качество ответов на тестовых диалогах
* смена модели влияет на поведение бота, даже без изменения сценария
{% endhint %}

</details>

### Когда удобно использовать разные модели:

{% hint style="success" %}
Раздел AI Models особенно полезен, когда нужно:

* улучшить точность логики без удорожания ответов
* улучшить качество текста без перестройки воронки
* подобрать баланс между стоимостью и результатом
* сделать ответы более строгими или более креативными
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
