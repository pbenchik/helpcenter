---
icon: clock
---

# Delay

> ### Delay - это шаг, который позволяет выполнить следующий переход в конкретное время.

{% hint style="info" %}
**Delay помогает запускать следующий шаг по времени, которое вы задаёте вручную. Время рассчитывается по таймзоне бота.**

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (17).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="info" %}
**Используется для:**

* <mark style="color:$primary;">запуска действий в конкретное время</mark>
* <mark style="color:$primary;">построения логики flow по расписанию</mark>
* <mark style="color:$primary;">управления таймингом сценария</mark>
* <mark style="color:$primary;">отложенного перехода к следующему шагу</mark>
{% endhint %}

### Основные возможности:

{% hint style="info" %}
**С помощью Delay вы можете:**

* <mark style="color:$primary;">выполнять действия в конкретное время</mark>
* <mark style="color:$primary;">управлять расписанием сценария</mark>
* <mark style="color:$primary;">выстраивать последовательность шагов по времени</mark>
* <mark style="color:$primary;">контролировать момент следующего перехода</mark>
{% endhint %}

### Структура шага:

<details>

<summary>1. Settings (Настройки)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (19).png" alt=""><figcaption></figcaption></figure></div>

**Title**\
<mark style="color:$primary;">Название шага.</mark>\
<mark style="color:$primary;">Используется для удобной навигации внутри flow.</mark>

***

**Finish Status**\
<mark style="color:$primary;">Статус диалога после выполнения шага.</mark>\
<mark style="color:$primary;">Варианты:</mark>

* <mark style="color:$primary;">**nothing**</mark> <mark style="color:$primary;">- переход к следующему шагу</mark>
* <mark style="color:$primary;">**auto**</mark> <mark style="color:$primary;">- автоматическое продолжение диалога</mark>
* <mark style="color:$primary;">**waiting**</mark> <mark style="color:$primary;">- ожидание ответа пользователя</mark>
* <mark style="color:$primary;">**manual**</mark> <mark style="color:$primary;">- перевод в ручной режим</mark>
* <mark style="color:$primary;">**blocked**</mark> <mark style="color:$primary;">- блокировка диалога</mark>
* <mark style="color:$primary;">**finished**</mark> <mark style="color:$primary;">- завершение диалога</mark>

***

**Hide keyboard**\
<mark style="color:$primary;">Скрывает клавиатуру из предыдущего шага.</mark>

***

**Is start step of flow**\
<mark style="color:$primary;">Отмечает шаг как стартовый.</mark>

***

Skip the transition to next step

<mark style="color:$primary;">Отключает автоматический переход на следующий шаг.</mark>

<mark style="color:$primary;">Используется в связке со статусом waiting.</mark>

<mark style="color:$primary;">Если опция включена:</mark>

* <mark style="color:$primary;">шаг не переключится автоматически</mark>
* <mark style="color:$primary;">система останется на текущем шаге</mark>
* <mark style="color:$primary;">будет ожидать ответ пользователя</mark>
{% endhint %}



</details>

<details>

<summary>2. Delay (Время выполнения)</summary>

{% hint style="info" %}
<mark style="color:$primary;">Здесь задаётся точное время выполнения шага.</mark>

*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (20).png" alt=""><figcaption></figcaption></figure>

<mark style="color:$primary;">Указывается конкретное время, а не задержка от предыдущего шага.</mark>

<mark style="color:$primary;">Формат:</mark> <mark style="color:$primary;">`часы : минуты`</mark>
{% endhint %}



</details>

<details>

<summary>Пример использования</summary>

{% hint style="info" %}
**Сценарий 1: отправка сообщения утром**

<mark style="color:$primary;">Delay → 10:00</mark>\
<mark style="color:$primary;">→ сообщение отправится в 10:00 по таймзоне бота</mark>

***

**Сценарий 2: запуск действия вечером**

<mark style="color:$primary;">Delay → 18:30</mark>\
<mark style="color:$primary;">→ шаг выполнится в 18:30 по таймзоне бота</mark>
{% endhint %}



</details>

<details>

<summary>Важная логика работы</summary>

{% hint style="warning" %}
**Delay работает с учётом таймзоны бота.**

<mark style="color:$primary;">Перед настройкой проверьте timezone в Bot Settings → General → Timezone.</mark>

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (18).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

### Важно перед началом:

{% hint style="warning" %}
<mark style="color:$primary;">Шаг выполняется в указанное время.</mark>\
<mark style="color:$primary;">До наступления этого времени сценарий приостанавливается.</mark>\
<mark style="color:$primary;">После наступления времени происходит переход к следующему шагу.</mark>\
<mark style="color:$primary;">Время всегда рассчитывается по таймзоне бота.</mark>
{% endhint %}

{% hint style="success" %}
**Используйте этот шаг, когда нужно:**

* <mark style="color:$primary;">выполнить действие в конкретное время</mark>
* <mark style="color:$primary;">настроить сценарий по расписанию</mark>
* <mark style="color:$primary;">контролировать тайминг воронки</mark>
* <mark style="color:$primary;">запускать действия в нужный момент</mark>
{% endhint %}

{% columns fullWidth="false" %}
{% column width="50%" %}
{% hint style="info" %}
**Старт и обзор**

* <a href="../../../dobro-pozhalovat/o-produkte/" class="button secondary" data-icon="table">О продукте</a>
* <a href="../../../dobro-pozhalovat/arkhitektura-sistemy/" class="button secondary" data-icon="sitemap">Архитектура системы</a>
* <a href="../../../bystryi-start/" class="button secondary" data-icon="rocket">Быстрый старт</a>
{% endhint %}

{% hint style="info" %}
**Аналитика и управление**

* <a href="../../../analytics/" class="button secondary" data-icon="chart-line">Analytics</a>
* <a href="../../../tracker/" class="button secondary" data-icon="chart-line">Tracker</a>
* <a href="../../../administrirovanie-company/" class="button secondary" data-icon="buildings">Администрирование</a>
* <a href="/broken/spaces/AxluUgdTFxFU08qksWVa/pages/yonwUmMhqke1c4edMh5B" class="button secondary" data-icon="circle-question">FAQ и решение проблем</a>
{% endhint %}
{% endcolumn %}

{% column width="50%" %}
{% hint style="info" %}
**Работа в платформе**

* <a href="../../../crm/" class="button secondary" data-icon="comments">CRM</a>
* <a href="../../" class="button secondary" data-icon="arrow-progress">Конструктор (Flow Settings)</a>
* <a href="../../../bot-settings/" class="button secondary" data-icon="robot">Bot Settings</a>
{% endhint %}

{% hint style="info" %}
**Частые вопросы**

* <a href="../../../../faq-i-reshenie-problem/tipy-oshibok/oshibka-403.md" class="button secondary" data-icon="message-xmark">Бот не отвечает</a>
* <a href="../../../../faq-i-reshenie-problem/tipy-oshibok/oshibka-400.md" class="button secondary" data-icon="triangle-exclamation">Нет ClickID</a>
* <a href="../../../bystryi-start/sozdanie-i-podklyuchenie-bota/tipy-botov-v-chatterfy.md" class="button secondary" data-icon="robot">Какой тип бота выбрать?</a>
* <a href="../../../../faq-i-reshenie-problem/chastye-voprosy/kak-skryt-chaty-mezhdu-operatorami.md" class="button secondary" data-icon="comment-xmark">Пуши не работают</a>
{% endhint %}
{% endcolumn %}
{% endcolumns %}
