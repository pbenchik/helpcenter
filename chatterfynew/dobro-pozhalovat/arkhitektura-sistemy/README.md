---
description: В этой статье вы поймете как устроена система Chatterfy
icon: boxes-stacked
---

# Архитектура системы

Каждый раздел отвечает за свою часть работы: управление компанией, рабочие пространства, CRM и трекинг трафика.

Chatterfy состоит из нескольких основных разделов.

{% hint style="info" %}
Понимание этой структуры помогает быстрее ориентироваться в интерфейсе и правильно настраивать систему.
{% endhint %}

### Как устроена система

Это базовая логика работы в Chatterfy.

#### Как это работает

Сначала на уровне **Company** настраивают компанию.

Внутри неё создают **Spaces**, а команда работает в **CRM** и **Tracker**.

#### Шаги

1. Управляют компанией в **Company**
2. Создают рабочие пространства в **Spaces**
3. Работают с лидами и чатами в **CRM**
4. Анализируют трафик и конверсии в **Tracker**

### Company

Раздел для управления компанией на общем уровне.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/image 32635.png" alt=""><figcaption></figcaption></figure></div>

#### Что здесь настраивают

* **Пользователи** — управление доступом сотрудников
* **Роли** — права доступа внутри компании
* **Spaces** — рабочие пространства
* **Billing** — баланс и платежи
* **Logs** — системные действия

#### Связанная страница

* [Company - управление компанией](company-upravlenie-kompaniei.md)

### Spaces

Рабочие пространства помогают разделять команды и проекты.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure></div>

#### Когда использовать

* Несколько направлений
* Разные команды
* Отдельные источники трафика

#### Связанная страница

* [Spaces - рабочие пространства](spaces-rabochie-prostranstva.md)

### CRM

CRM используется для работы с лидами и клиентами.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure></div>

#### Что здесь делает команда

* Ведёт переписку
* Меняет статусы
* Назначает менеджеров
* Смотрит историю и данные по лиду

#### Связанная страница

* [CRM - работа с клиентами](crm-rabota-s-klientami.md)

### Tracker

Tracker нужен для анализа рекламы и событий.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure></div>

#### Что показывает

* Источники трафика
* События и конверсии
* Эффективность кампаний

#### Связанная страница

* [Tracker - отслеживание трафика](tracker-otslezhivanie-trafika.md)

{% hint style="info" %}
Базовая логика системы простая: **Company** → **Spaces** → работа команды в **CRM** и **Tracker**.
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
