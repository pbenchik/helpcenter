---
icon: list-check
---

# Роли Company

> #### Роли Company определяют, какие разделы и действия доступны сотруднику.

От выбранной роли зависит доступ к компании, Space, CRM и Tracker.

### Что регулируют роли:

{% hint style="info" %}
Через роли обычно настраивают:

* доступ к разделам компании
* уровень управления пользователями
* доступ к CRM и ботам
* доступ к Tracker и кампаниям
{% endhint %}

### Как работают роли в системе:

{% stepper %}
{% step %}
#### Сотрудника приглашают в компанию

{% hint style="warning" %}
Сначала пользователь получает доступ на уровне **Company**.
{% endhint %}
{% endstep %}

{% step %}
#### Ему назначают подходящую роль

{% hint style="warning" %}
Роль определяет, какие разделы он увидит и что сможет делать внутри системы.
{% endhint %}
{% endstep %}

{% step %}
#### При необходимости выдают доступ в Space и Tracker

{% hint style="warning" %}
Одной роли недостаточно, если сотруднику ещё нужен доступ к конкретным рабочим пространствам или кампаниям.
{% endhint %}
{% endstep %}
{% endstepper %}

### Основные роли Company:

<details>

<summary>Owner</summary>

{% hint style="info" %}
Создатель компании.

Права:

* полный доступ ко всем разделам системы
* управление пользователями, Spaces и настройками
* доступ к биллингу и системным данным
{% endhint %}

{% hint style="success" %}
Имеет доступ ко всему.
{% endhint %}

</details>

<details>

<summary>Admin</summary>

{% hint style="info" %}
Администратор компании с почти полным доступом.

Может:

* управлять пользователями и доступами
* настраивать рабочие разделы системы
* контролировать общую работу компании
{% endhint %}

{% hint style="danger" %}
Ограничение: не может удалить владельца компании.
{% endhint %}

{% hint style="success" %}
Имеет доступ ко всему, кроме удаления владельца компании.
{% endhint %}

</details>

<details>

<summary>Manager</summary>

{% hint style="info" %}
Роль для сотрудников с расширенным рабочим доступом.

может:

* настраивать ботов
* редактировать воронки
* создавать сценарии
* управлять CRM
{% endhint %}

{% hint style="danger" %}
Не может:

* Просматривать Logs.
* Экспорт и скачивание данных.
* Просмотр логов.
{% endhint %}

{% hint style="success" %}
Имеет доступ ко всему, кроме раздела Logs.
{% endhint %}

</details>

<details>

<summary>Operator (CRM)</summary>

{% hint style="info" %}
Базовая роль для операторов CRM.

Может:

* работать с чатами
* вести переписку с лидами
* использовать CRM-интерфейс
{% endhint %}

{% hint style="danger" %}
Не может:

* редактировать ботов
* настраивать воронки
* Просматривать аналитику
* Просматривать logs
{% endhint %}

{% hint style="success" %}
Имеет доступ к разделам

* Messenger
* Users
* Mailings
{% endhint %}

</details>

<details>

<summary>Hide Operator (CRM)</summary>

{% hint style="info" %}
Анонимная версия роли Operator.

Особенности:

* имя лида скрыто
* `Telegram ID` скрыт
* аватар пользователя размыт
* отображается только `ChatterfyID`
{% endhint %}

{% hint style="danger" %}
Не может:

* редактировать ботов
* настраивать воронки
* Просматривать аналитику
* Просматривать logs
{% endhint %}

{% hint style="success" %}
Имеет доступ к разделам

* Messenger
{% endhint %}

{% hint style="warning" %}
Чаще всего роль используют в retention-командах.
{% endhint %}

</details>

<details>

<summary>Controller</summary>

{% hint style="info" %}
Роль для аналитики, контроля и аудита.

Он может:

* просматривать чаты
* редактировать чаты
* анализировать статистику
{% endhint %}

{% hint style="danger" %}
Не может :

* Изменять sale stage
* Изменять status
* Изменять flow и step
* Вносить информацию в Custom Data
* Отправлять сообщения
* Удалять диалоги
* Скачивать диалоги
* Удалять сообщения
{% endhint %}

{% hint style="success" %}
Имеет доступ к разделам:

* Messenger
* Users
* Mailings
{% endhint %}

</details>

<details>

<summary>Viewer</summary>

{% hint style="info" %}
Роль с минимальным доступом.

Может:

* просматривать интерфейс
{% endhint %}

{% hint style="danger" %}
Не может:

* писать сообщения
* работать с аналитикой
{% endhint %}

</details>

### Роли Tracker:

<details>

<summary>Buyer</summary>

{% hint style="info" %}
Роль для работы с Tracker.

Видит:

* только свои кампании, которые на него назначены
{% endhint %}

{% hint style="warning" %}
Buyer обычно назначается под одного Team Lead.
{% endhint %}

</details>

<details>

<summary>Buyer Team Lead</summary>

{% hint style="info" %}
Роль для управления группой байеров.

Может:

* видеть все кампании своих байеров
* редактировать кампании
* анализировать статистику
* управлять байерами
{% endhint %}

</details>

{% hint style="info" %}
Базовый принцип простой: сначала выдаётся роль на уровне Company, затем при необходимости открывается доступ к Space и Tracker.
{% endhint %}

{% hint style="warning" %}
Не выдавайте роли `Owner`, `Admin` или `Manager` всем сотрудникам без необходимости.
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
