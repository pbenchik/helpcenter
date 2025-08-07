---
description: >-
  Здесь мы покажем вам инструкцию по созданию и подключению вашего первого
  Телеграм чат-бота.
---

# Привязка Telegram bot

## 1) Cоздайте Telegram бота

Найдите [**@Botfather**](https://t.me/BotFather) в **Telegram** и напишите ему команду **/newbot.**&#x20;

Придумайте имя и никнейм вашего бота. Загружаем для бота аватар, описание, био и другие настройки. Эти данные будут видны всем пользователям.&#x20;

Копируем **API Token** бота \
(Пример: 6858\*\*\*\*\*\*:AAEPteOdUl68W2QYF1AFD9A\_q6lXA\*\*\*\*\*\*)

***

## 2) Подключите бота в Chatterfy&#x20;

* Перейдите на [платформу Chatterfy](https://next.chatterfy.ai/bots) и нажмите создайте нового чат-бота

<figure><img src="../../../.gitbook/assets/image (356).png" alt=""><figcaption></figcaption></figure>

* Выберите тип **Standard Telegram Bot**&#x20;

{% hint style="info" %}
&#x20;**Standard Telegram Bot:** \
✅ автоматически принимает заявки в канал \
✅ может быть как инвайтом, так и ДМ ботом \
✅ возможность использования ИИ \
✅ возможность отправки сообщений вручную внутри СРM
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (357).png" alt=""><figcaption></figcaption></figure>

Укажите Спейс в котором бот будет размещен. Например, Space GamblingSpace\
\
Добавьте **Description** (внутреннее описание бота)

<figure><img src="../../../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure>

Выберите модели обработки для:&#x20;

* **System AI Summary model** - (как ИИ думает) используется для сбора информации содержащейся в инструкциях бота и сообщений из диалога
* **System AI Summary Router model** - используется только в [**AI Router**](https://help.chatterfy.ai/nastroika/tipy-shagov-v-skripte/ai-router) (когда мы используем функционал для разветвления воронки) для определения по какой ветке продвигать диалог в зависимости от ответа юзера.
* **System AI Reply model** - (от чего зависит ответ) используется для финальной генерации ответа на основании **AI Summary**&#x20;

Перейдите по ссылке, чтобы узнать подробнее о доступных моделях и какую лучше выбрать: [AI модели](../../../konstruktor-skriptov/podklyuchenie-ai/kak-vybrat-model-ai.md)

{% hint style="info" %}
Run Immediately - автоматический запуск (активация) бота
{% endhint %}



* Вставляем **API Token**

<figure><img src="../../../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Через **API Token** бот должен быть подключен **ТОЛЬКО** к нашему сервису, иначе могут возникнуть сбои и конфликты токенов. Не подключайте его к сторонним сервисам.
{% endhint %}

## 3) Запустите бота в Chatterfy

* После добавления скриптов воронки и проверки, **нажмите** **на значок шестеренки**. Вы перейдете во внутренние настройки функционала чат-бота.

<figure><img src="../../../.gitbook/assets/bot3 .png" alt=""><figcaption><p>Нажмите на значок шестеренки и вы перейдете в настройки бота </p></figcaption></figure>

* Нажмите **активировать**&#x20;

<figure><img src="../../../.gitbook/assets/bot 4.png" alt=""><figcaption><p>Нажмите на синюю кнопку, чтобы активировать бота</p></figcaption></figure>
