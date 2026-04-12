---
icon: calendar-users
---

# Подключение Tracker

> ### Подключение Tracker нужно, чтобы начать отслеживать трафик и события внутри воронки. Tracker показывает путь пользователя от клика по ссылке до целевого действия в Telegram.

### Что даёт Tracker:

{% hint style="info" %}
С помощью Tracker вы можете:

* отслеживать источники трафика
* анализировать поведение пользователей
* видеть события и конверсии
* оценивать эффективность рекламных кампаний
* работать с аналитикой в одном интерфейсе
{% endhint %}

### Как подключается Tracker:

{% stepper %}
{% step %}
#### Подключается домен

{% hint style="warning" %}
Сначала добавляется домен, который будет использоваться в ссылках и кампаниях.
{% endhint %}
{% endstep %}

{% step %}
#### Создаётся лендинг

{% hint style="warning" %}
После этого выбирается стандартный лендинг или загружается свой.
{% endhint %}
{% endstep %}

{% step %}
#### Настраивается кампания

{% hint style="warning" %}
На этом этапе задаются источник трафика, параметры и правила кампании.
{% endhint %}
{% endstep %}

{% step %}
#### Подключается приёмщик лидов

{% hint style="warning" %}
Дальше нужно выбрать, куда будет попадать пользователь: в бота, канал или личный аккаунт.
{% endhint %}
{% endstep %}

{% step %}
#### Проверяется аналитика

{% hint style="warning" %}
После запуска трафика данные начинают появляться в статистике Tracker.
{% endhint %}
{% endstep %}
{% endstepper %}

### Основные этапы подключения:

<details>

<summary>Подключение домена</summary>

{% hint style="info" %}
Домен используется в трекинговых ссылках и кампаниях.

Без него нельзя корректно запустить трекинг.
{% endhint %}

* [Как работает Tracker](../tracker/kak-rabotaet-tracker.md)
* [Domains](../tracker/domains/)

</details>

<details>

<summary>Создание лендинга</summary>

{% hint style="info" %}
Для Tracker нужен лендинг, через который будет идти пользователь.

Можно использовать готовый шаблон или загрузить свой вариант.
{% endhint %}

* [Landings](../tracker/landings/)
* [Как создать landing](../tracker/landings/kak-sozdat-landing.md)

</details>

<details>

<summary>Настройка кампании</summary>

{% hint style="info" %}
Кампания связывает источник трафика, параметры и правила учёта событий.

Именно здесь задаётся логика трекинга.
{% endhint %}

* [Campaigns](../tracker/campaigns/)
* [Как создать кампанию](../tracker/campaigns/kak-sozdat-kampaniyu.md)

</details>

<details>

<summary>Подключение приёмщика лидов</summary>

{% hint style="info" %}
После кампании нужно выбрать канал, куда будет попадать пользователь.

Это может быть Telegram-бот, канал или личный аккаунт.
{% endhint %}

* [Как работает Tracker](../tracker/kak-rabotaet-tracker.md)
* [Создание и подключение бота](sozdanie-i-podklyuchenie-bota/)

</details>

<details>

<summary>Аналитика и интеграции</summary>

{% hint style="info" %}
После запуска трафика события и конверсии появляются в аналитике Tracker.

При необходимости можно подключить внешние интеграции и postback.
{% endhint %}

* [Analytics](../tracker/analytics/)
* [Integrations](../tracker/integrations/)

</details>

{% hint style="info" %}
Базовая логика подключения простая: домен → лендинг → кампания → приёмщик лидов → аналитика.
{% endhint %}

{% hint style="info" %}
Подразделы

* <a href="../tracker/kak-rabotaet-tracker.md" class="button secondary" data-icon="scroll">Как работает Tracker</a><a href="../tracker/domains/" class="button secondary" data-icon="globe">Подключение доменов</a><a href="../tracker/landings/" class="button secondary" data-icon="file-lines">Создание лендинга</a>
* <a href="../tracker/campaigns/" class="button secondary" data-icon="bullhorn">Создание кампании</a><a href="../tracker/integrations/" class="button secondary" data-icon="network-wired">Интеграции и postback</a><a href="../tracker/analytics/" class="button secondary" data-icon="chart-line">Аналитика Tracker</a>
{% endhint %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
