---
description: В этой статье вы поймете как устроена система Chatterfy
icon: boxes-stacked
---

# Архитектура системы

> #### Каждый раздел отвечает за свою часть работы: управление компанией, рабочие пространства, CRM и трекинг трафика.
>
> Chatterfy состоит из нескольких основных разделов.

{% hint style="warning" %}
Понимание этой структуры помогает быстрее ориентироваться в интерфейсе и правильно настраивать систему.
{% endhint %}

### Как устроена система:

{% stepper %}
{% step %}
### Company

{% hint style="info" %}
На верхнем уровне находится **Company**.

Здесь управляют компанией, пользователями, биллингом и общими настройками.
{% endhint %}
{% endstep %}

{% step %}
### Spaces

{% hint style="info" %}
Внутри компании создаются **Spaces**.

Это отдельные рабочие пространства для команд, проектов или источников трафика.
{% endhint %}
{% endstep %}

{% step %}
### CRM

{% hint style="info" %}
Внутри рабочих процессов команда общается с клиентами через **CRM**.

Здесь находятся чаты, карточки лидов, фильтры, статусы и история взаимодействий.
{% endhint %}
{% endstep %}

{% step %}
### Tracker

{% hint style="info" %}
Для анализа трафика и конверсий используется **Tracker**.

Он показывает путь пользователя от клика до целевого действия.
{% endhint %}
{% endstep %}
{% endstepper %}

### Основные разделы системы:

<details>

<summary>Company</summary>

{% hint style="info" %}
Раздел для управления компанией на общем уровне.

Здесь настраиваются:

* Пользователи
* Роли
* Spaces
* Биллинг
* Системные логи
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image 32635.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

</details>

<details>

<summary>Spaces</summary>

{% hint style="info" %}
Рабочие пространства помогают разделять команды и проекты.

Это удобно, если у вас:

* Несколько направлений
* Разные команды
* Отдельные источники трафика
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

</details>

<details>

<summary>CRM</summary>

{% hint style="info" %}
CRM используется для работы с лидами и клиентами.

Здесь команда:

* Ведёт переписку
* Меняет статусы
* Назначает менеджеров
* Смотрит историю и данные по лиду
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

</details>

<details>

<summary>Tracker</summary>

{% hint style="info" %}
Tracker нужен для анализа рекламы и событий.

Он помогает:

* Отслеживать источники трафика
* Видеть события и конверсии
* Анализировать эффективность кампаний
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

</details>

{% hint style="info" %}
Базовая логика системы простая: **Company → Spaces → работа команды в CRM и Tracker**.
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
