---
description: Назначение и преимущества бизнес-ботов в Телеграм
---

# Привязка Business Telegram Bot

\
\
Chatterfy представляет интеграцию бизнес-ботов в Telegram. Этот шаг открывает перед пользователями новые возможности автоматизации и взаимодействия с клиентами.&#x20;

### Почему бизнес-боты интегрируются в личные чаты? <a href="#pochemu-biznes-boty-integriruyutsya-v-lichnye-chaty" id="pochemu-biznes-boty-integriruyutsya-v-lichnye-chaty"></a>

У пользователей есть возможность привязать Телеграм-бота, который будет обрабатывать сообщения и отправлять ответы. Это не новое решение, однако для подписчиков тарифа Телеграм Премиум доступны дополнительные возможности, такие как привязка Телеграм-бота к личному аккаунту премиум и настройка автоматических ИИ ответов.

**Вот пример:** Бот внутри личного чата с клиентом может мгновенно отправить подробное описание/инструкцию, предоставить доп информацию. И все это без необходимости участия оператора.

###

### Какие отличия?&#x20;

Business Telegram Bot - это обычный бот от имени лички, у которого есть ряд особенностей: \
\
✅  Есть 24 на отправку сообщений лиду\
&#x20;(после 24 часов нужен ответ от клиента, чтобы продолжить отправку сообщений)\
✅  Лимиты объективно выше чем на личках

{% hint style="warning" %}
Единственное что история только с момента запуска, то есть бот не сможет подтянуть историю предыдущих чатов
{% endhint %}

###

### Инструкция по добавлению Бизнес бота Телеграм



1\. Перейдите в главное меню. Нажмите кнопку Создать бота

<figure><img src="../../../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

2\. В типе бота выберите - Бизнес Телеграм бот. Выберите спейс и модель обработки ИИ&#x20;

<figure><img src="../../../.gitbook/assets/image (389).png" alt=""><figcaption></figcaption></figure>

Выберите модели обработки для:&#x20;

* **System AI Summary model** - (как ИИ думает) используется для сбора информации содержащейся в инструкциях бота и сообщений из диалога
* **System AI Summary Router model** - используется только в [**AI Router**](https://help.chatterfy.ai/nastroika/tipy-shagov-v-skripte/ai-router) (когда мы используем функционал для разветвления воронки) для определения по какой ветке продвигать диалог в зависимости от ответа юзера.
* **System AI Reply model** - (от чего зависит ответ) используется для финальной генерации ответа на основании **AI Summary**&#x20;

Перейдите по ссылке, чтобы узнать подробнее о доступных моделях и какую лучше выбрать: [AI модели](../../../konstruktor-skriptov/podklyuchenie-ai/kak-vybrat-model-ai.md)

{% hint style="info" %}
Run Immediately - автоматический запуск (активация) бота
{% endhint %}

3. Добавьте описание бота&#x20;

<figure><img src="../../../.gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure>

4. Вставьте бот токен&#x20;

<figure><img src="../../../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>

## Добавление бота в Телеграм бизнес режим



1. Скопируйте ник @бота

<figure><img src="../../../.gitbook/assets/image (168).png" alt=""><figcaption></figcaption></figure>

2\. Перейдите в настройки вашего Телеграм аккауна

3\. Нажмите на Телеграм Бизнес

<figure><img src="../../../.gitbook/assets/image (169).png" alt=""><figcaption></figcaption></figure>

4\. Пролистайте вниз и выберите Чатботы

<figure><img src="../../../.gitbook/assets/image (170).png" alt=""><figcaption></figcaption></figure>

5\. Вставьте ссылку или же ник @своего бота

<figure><img src="../../../.gitbook/assets/image (171).png" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
**ЕСЛИ ПРИ ДОБАВЛЕНИИ ВОЗНИКЛА ОШИБКА, ВАМ НЕОБХОДИМО ВКЛЮЧИТЬ БИЗНЕС РЕЖИМ ДЛЯ БОТА!**&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

1\.  Перейдите в BotFather, нажмите на меню

2\. Выберите/mybots



<figure><img src="../../../.gitbook/assets/image (173).png" alt=""><figcaption></figcaption></figure>

3\. Нажмите на настройки бота

4\. Активируйте бизнес режим для бота



<figure><img src="../../../.gitbook/assets/image (174).png" alt=""><figcaption></figcaption></figure>



5\. Нажмите Активировать&#x20;

{% hint style="warning" %}
**ЕСЛИ ВЫ ВСЕ ЕЩЕ НЕ МОЖЕТЕ ДОБАВИТЬ БОТА, ПЕРЕЗАПУСТИТЕ ПРИЛОЖЕНИЕ ТЕЛЕГРАММ!!!**
{% endhint %}

### ПРИМЕР ПОЛЬЗОВАНИЯ&#x20;

1\. Клиент написал на личку&#x20;

<figure><img src="../../../.gitbook/assets/image (175).png" alt=""><figcaption></figcaption></figure>

2\. Автоматически запустится диалог и первое сообщение по заданной нами в конструкторе воронке и клиенту ответит бот

<figure><img src="../../../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

> Все сообщения, которые клиент напишет в личку, появляются в боте в Chatterfy&#x20;

