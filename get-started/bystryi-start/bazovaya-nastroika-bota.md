---
icon: server
---

# Базовая настройка бота

> ### Базовая настройка бота помогает подготовить бота к работе сразу после подключения. В этом разделе обычно проверяют основные параметры, от которых зависит работа команды и самого бота.

### Что настраивается в первую очередь:

{% hint style="info" %}
После создания бота обычно настраивают:

* часовой пояс
* статус бота
* рабочий Space
* внутреннее описание
{% endhint %}

### Как проходит базовая настройка:

{% stepper %}
{% step %}
#### Откройте Bot Settings → General

{% hint style="warning" %}
Все базовые параметры бота находятся в разделе **General**.
{% endhint %}
{% endstep %}

{% step %}
#### Проверьте ключевые настройки

{% hint style="warning" %}
На этом этапе обычно задают timezone, проверяют статус бота и при необходимости меняют Space.
{% endhint %}
{% endstep %}

{% step %}
#### Добавьте описание для команды

{% hint style="warning" %}
Внутреннее описание помогает быстрее ориентироваться, если в системе много ботов.
{% endhint %}
{% endstep %}
{% endstepper %}

### Основные настройки:

<details>

<summary>Timezone</summary>

{% hint style="info" %}
Здесь выбирается часовой пояс бота.

Это важно, если:

* боты работают в разных ГЕО
* команда ориентируется на локальное время
* нужно корректное отображение времени внутри системы
{% endhint %}

<div data-with-frame="true"><img src="../../.gitbook/assets/Frame 2149.png" alt=""></div>

{% hint style="info" %}
Вся информация внутри бота отображается согласно выбранной таймзоне.
{% endhint %}

</details>

<details>

<summary>Включение и выключение бота</summary>

{% hint style="info" %}
Бота можно включать и выключать в зависимости от задачи.

Когда бот выключен:

* он не работает
* плата за него не начисляется
{% endhint %}

<div data-with-frame="true"><img src="../../.gitbook/assets/Frame 2150.png" alt=""></div>

{% hint style="info" %}
При необходимости бота также можно архивировать.
{% endhint %}

</details>

<details>

<summary>Перемещение между Spaces</summary>

{% hint style="info" %}
Бота можно перенести в другой Space, если изменилась команда или проект.

Для этого:

* выберите новый Space
* сохраните изменения
{% endhint %}

<div data-with-frame="true"><img src="../../.gitbook/assets/Frame 2151.png" alt=""></div>

</details>

<details>

<summary>Описание бота</summary>

{% hint style="info" %}
Вы можете добавить внутреннее описание бота.

Оно помогает:

* не путаться между ботами
* фиксировать назначение бота внутри команды
* быстрее ориентироваться в списке проектов
{% endhint %}

<div data-with-frame="true"><img src="../../.gitbook/assets/Frame 2149 (1).png" alt=""></div>

{% hint style="info" %}
Описание видно только внутри Chatterfy.
{% endhint %}

</details>

{% hint style="info" %}
Базовая логика простая: сначала проверьте настройки в General, затем убедитесь, что бот активен и находится в нужном Space.
{% endhint %}

{% hint style="info" %}
Связанные страницы

* <a href="/broken/spaces/AxluUgdTFxFU08qksWVa/pages/JC3Y3E6CWfMjRVAr2wH4" class="button secondary" data-icon="tag">Название</a><a href="/broken/spaces/AxluUgdTFxFU08qksWVa/pages/uvw6TXs2BpGWBqU0HmGX" class="button secondary" data-icon="toggle-on">Статус</a><a href="/broken/spaces/AxluUgdTFxFU08qksWVa/pages/6g9jYBF0ToOLyzgYwFYp" class="button secondary" data-icon="clock">Timezone</a><a href="sozdanie-i-podklyuchenie-bota/" class="button secondary" data-icon="robot">Создание и подключение бота</a>
{% endhint %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
