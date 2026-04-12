---
icon: arrow-progress
---

# Create New Flow

> ### **Create New Flow** помогает быстро создать новый flow или перенести готовую структуру из другого бота.

### Важно перед началом:

{% hint style="warning" %}
**Перед созданием нового flow заранее определите:**

* нужен ли вам пустой flow или копия существующего
* из какого space и бота нужно делать импорт
* нужно ли переносить AI Settings и global push messages
{% endhint %}

### Основные возможности:

{% hint style="info" %}
**С помощью Create New Flow вы можете:**

* быстро запускать новые сценарии
* использовать готовые flow как шаблон
* копировать рабочую AI-конфигурацию
* сокращать время на настройку нового бота
{% endhint %}

### Способы создания flow:

<details>

<summary>Create flow</summary>

{% hint style="info" %}
**Чтобы создать новый flow вручную:**

* нажмите кнопку в левой верхней части раздела **Flow Settings**
*

    <figure><img src="../../.gitbook/assets/Frame 2248 (5).png" alt=""><figcaption></figcaption></figure>
* введите название нового flow
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (6).png" alt=""><figcaption></figcaption></figure></div>
* нажмите **Save**

**После сохранения система создаст новый пустой flow.**
{% endhint %}



</details>

<details>

<summary>Import flow</summary>

{% hint style="info" %}
**Import flow** позволяет перенести flow из другого бота или space.

Чтобы выполнить импорт:

* выберите space компании, из которого хотите перенести flow
* откройте нужный space
* выберите бота или личный аккаунт
* отметьте нужный flow
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (7).png" alt=""><figcaption></figcaption></figure></div>
* **запустите импорт**
{% endhint %}



</details>

<details>

<summary>Import AI Settings</summary>

{% hint style="info" %}
**Import AI Settings** переносит **Global Bot Settings** и **AI Settings** выбранного бота.

Используйте этот вариант, если:

* новому боту нужны такие же AI-настройки
* вы хотите быстро скопировать логику поведения бота
* не нужно настраивать роль и стиль общения заново
{% endhint %}



</details>

<details>

<summary>Import global push messages</summary>

{% hint style="info" %}
**Import global push messages** переносит глобальные push messages из другого бота.

Это удобно, если:

* у вас уже есть готовая схема пушей
* нужно быстро повторить настройки в новом боте
* важно сохранить одинаковую логику догрева

Подробнее: [Push](/broken/spaces/AxluUgdTFxFU08qksWVa/pages/OD3xjP4kv5pdIaw4u22M)
{% endhint %}

{% hint style="info" %}
**Используется для:**

* создания нового flow с нуля
* импорта готового flow из другого space
* переноса AI Settings из другого бота
* копирования global push messages
{% endhint %}

{% hint style="info" %}
**Через это окно вы можете:**

* создать пустой flow и задать ему имя
* импортировать уже готовую воронку
* ускорить запуск нового бота за счёт копирования настроек
{% endhint %}



</details>

### Важная логика работы:

{% hint style="warning" %}
* **Create flow** создаёт пустой сценарий
* Import flow переносит структуру выбранного flow
* Import AI Settings не переносит сам flow
* Import global push messages копирует только глобальные пуши
{% endhint %}

### Когда использовать Create New Flow:

{% hint style="success" %}
Используйте этот инструмент, когда нужно:

* создать новую воронку с нуля
* скопировать готовую воронку в другой бот
* быстро перенести AI-настройки
* повторно использовать global push messages
{% endhint %}

{% columns fullWidth="false" %}
{% column width="50%" %}
{% hint style="info" %}
**Старт и обзор**

* <a href="../dobro-pozhalovat/o-produkte/" class="button secondary" data-icon="table">О продукте</a>
* <a href="../dobro-pozhalovat/arkhitektura-sistemy/" class="button secondary" data-icon="sitemap">Архитектура системы</a>
* <a href="../bystryi-start/" class="button secondary" data-icon="rocket">Быстрый старт</a>
{% endhint %}

{% hint style="info" %}
**Аналитика и управление**

* <a href="../analytics/" class="button secondary" data-icon="chart-line">Analytics</a>
* <a href="../tracker/" class="button secondary" data-icon="chart-line">Tracker</a>
* <a href="../administrirovanie-company/" class="button secondary" data-icon="buildings">Администрирование</a>
* <a href="/broken/spaces/AxluUgdTFxFU08qksWVa/pages/yonwUmMhqke1c4edMh5B" class="button secondary" data-icon="circle-question">FAQ и решение проблем</a>
{% endhint %}
{% endcolumn %}

{% column width="50%" %}
{% hint style="info" %}
**Работа в платформе**

* <a href="../crm/" class="button secondary" data-icon="comments">CRM</a>
* <a href="./" class="button secondary" data-icon="arrow-progress">Конструктор (Flow Settings)</a>
* <a href="../bot-settings/" class="button secondary" data-icon="robot">Bot Settings</a>
{% endhint %}

{% hint style="info" %}
**Частые вопросы**

* <a href="../../faq-i-reshenie-problem/tipy-oshibok/oshibka-403.md" class="button secondary" data-icon="message-xmark">Бот не отвечает</a>
* <a href="../../faq-i-reshenie-problem/tipy-oshibok/oshibka-400.md" class="button secondary" data-icon="triangle-exclamation">Нет ClickID</a>
* <a href="../bystryi-start/sozdanie-i-podklyuchenie-bota/tipy-botov-v-chatterfy.md" class="button secondary" data-icon="robot">Какой тип бота выбрать?</a>
* <a href="../../faq-i-reshenie-problem/chastye-voprosy/kak-skryt-chaty-mezhdu-operatorami.md" class="button secondary" data-icon="comment-xmark">Пуши не работают</a>
{% endhint %}
{% endcolumn %}
{% endcolumns %}
