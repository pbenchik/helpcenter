---
icon: brain-circuit
---

# AI Reply

> ### AI Reply - это блок, который генерирует ответы с помощью нейросети во время общения с пользователем.

Он создает сообщения, похожие на ответы человека, учитывая вашу легенду, инструкции, правила и условия выполнения задач.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2139 (6).png" alt=""><figcaption></figcaption></figure></div>

### Подробнее:

<details>

<summary>1. Settings (Настройки)</summary>

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (50).png" alt=""><figcaption></figcaption></figure></div>

#### Title

{% hint style="info" %}
Название шага.\
Используется для удобной навигации внутри flow.
{% endhint %}

***

#### Delay

{% hint style="info" %}
Задержка перед выполнением шага.\
Во время задержки ИИ не отвечает
{% endhint %}

***

#### Finish Status

{% hint style="info" %}
Статус диалога. Указывать его необязательно, так как AI Reply работает автоматически.

<mark style="color:$warning;">После ответа ИИ диалог по умолчанию переходит в статус waiting и ожидает сообщение пользователя.</mark>\
Если ответ пользователя соответствует условиям из Requirements, система автоматически переведёт его на следующий шаг.
{% endhint %}

***

#### Важно!

{% hint style="danger" %}
* В AI Reply чаще всего не требуется вручную задавать Finish Status
* Логика перехода строится через Requirements, а не через статус
{% endhint %}

***

#### Hide keyboard

{% hint style="info" %}
Скрывает клавиатуру из предыдущего шага.
{% endhint %}

***

#### Is start step of flow

{% hint style="info" %}
Отмечает шаг как стартовый.
{% endhint %}

***

#### Skip the transition to next step

{% hint style="info" %}
Отключает автоматический переход на следующий шаг.

Используется вместе со статусом `waiting`.

Если опция включена:

* шаг не переключится автоматически
* система останется на текущем шаге
* будет ожидать ответ пользователя
* пуши продолжат отправляться по расписанию
{% endhint %}

***

</details>

<details>

<summary>2. AI Reply (Логика ИИ)</summary>

{% hint style="info" %}
<mark style="color:orange;">Goal</mark> - это задача, которую ИИ должен выполнить на этом шаге. В данном шаге вы закладываете основные инструкции и цель общения ИИ с клиентом, которую ИИ должен достичь во время текущего степа (этапа диалога).

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
<mark style="color:orange;">Requirements</mark> - это важный блок, который отвечает за условия перехода клиента по воронке. Здесь нужно кратко и четко указать, какое условие должно быть выполнено для перехода на этот шаг.

*

    <figure><img src="../../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>
* <mark style="color:$warning;">В требованиях указывайте только условие для перехода на следующий шаг, без лишних задач. Пишите так, чтобы ответ на условие всегда был "ДА" или "НЕТ".</mark>
*   Пример:

    YES - набор условий, когда YES

    NO - набор условий, когда точно сказать NO (опционально)
* Если при тестировании бот часто пропускает шаги и продолжает диалог без выполнения условия, попробуйте улучшить требования. Помните, что при переходе по воронке учитывается и цель, и требование, но требование играет главную роль.
* В случае, если Вы используете AI Routings - данный блок не будет использоваться
{% endhint %}

{% hint style="info" %}
<mark style="color:orange;">Legend</mark> - легенда, которая добавляется на конкретный степ (этап) воронки. Обычно добавляется информация, которую вы хотите чтобы клиент получил только на нужном степе.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure></div>
* Не дублируйте одну и ту же информацию и в легенду на шаге, и в легенду в AI Settings. Если есть информация, которая нужна на каждом шаге, добавляйте её именно в AI Settings - Global Legend.
{% endhint %}

{% hint style="info" %}
Reply Addition Info - это дополнительные вводные для ИИ при создании финального сообщения. Их формулируйте на "ты", например: <mark style="color:$warning;">"Никогда не здоровайся со мной"</mark> или "<mark style="color:$warning;">Никогда не упоминай Aviator"</mark><mark style="color:orange;">.</mark>

*

    <figure><img src="../../../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

{% hint style="info" %}
<mark style="color:orange;">Skip transition blocking on first run</mark> - полезный функционал, когда нам необходимо что бы ИИ пропустил юзера в случае подходящего ответа под Requirements (условия) и не генерировал из этого блока (просто убедился что условие выполнено)

<img src="../../../../.gitbook/assets/image (62).png" alt="" data-size="original">

* <mark style="color:green;">Чекбокс включен</mark> - перед блоком AI Reply у нас есть блок Send message, где мы спрашиваем у пользователя какую-то информацию. Если его ответ соответствует требованиям, он переходит на следующий шаг без сообщения от ИИ. Если ответ не подходит, пользователь остается на текущем шаге, пока не выполнит условие.
* <mark style="color:red;">Чекбокс не включен</mark> - перед блоком AI Reply у нас есть блок Send message, где мы спрашиваем у пользователя какую-то информацию. Если его ответ соответствует требованиям, пользователь все равно получит сообщение от ИИ перед переходом на следующий шаг.
* Это полезно, когда мы хотим предоставить пользователю дополнительную информацию на основе его ответа, даже если условие для перехода уже выполнено.
{% endhint %}

</details>

<details>

<summary>Где посмотреть примеры настройки?</summary>

{% hint style="info" %}
Если вы хотите увидеть, как AI Reply настраивается на практике, вы можете открыть готовые примеры внутри Chatterfy.
{% endhint %}

{% hint style="info" %}
* ### Для этого:
* #### Перейдите в компанию Chatterfy
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (51).png" alt=""><figcaption></figcaption></figure></div>
* #### Откройте space Demo<br>
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/unknown (16).jpeg" alt=""><figcaption></figcaption></figure></div>
* #### Выберите любого бота из списка
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (52).png" alt=""><figcaption></figcaption></figure></div>
* #### Перейдите в Flow Settings
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/unknown (18).jpeg" alt=""><figcaption></figcaption></figure></div>

Там вы найдете готовые flow с уже настроенными AI Reply шагами.

Это поможет быстрее понять, как правильно выстраивать диалог и формулировать условия.
{% endhint %}

</details>

<details>

<summary>3. Push Messages (Пуши)</summary>

{% hint style="info" %}
* Global push messages - из глобальных настроек
* Step push messages - настраиваются внутри шага
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (53).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

</details>

### Важная логика работы:

{% hint style="warning" %}
* AI Reply срабатывает только при входящем сообщении пользователя
* Переход на следующий шаг происходит при выполнении Requirements
* Goal влияет на поведение ИИ, но не на переход напрямую
{% endhint %}

### Основные возможности:

{% hint style="info" %}
С помощью AI Reply вы можете:

* вести живой диалог с пользователем
* собирать информацию
* квалифицировать лидов
* гибко реагировать на ответы
* управлять переходами по воронке
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
