---
icon: user-magnifying-glass
---

# Управление пользователями внутри Space

> ### Управление пользователями внутри Space

{% hint style="info" %}
Раздел нужен для управления участниками конкретного Space.

Здесь вы добавляете пользователей, назначаете им роли и управляете доступом к CRM и ботам.

Если пользователя ещё нет в компании, сначала <a href="../users/kak-priglasit-polzovatelei.md" class="button secondary">пригласите его.</a>
{% endhint %}

{% hint style="info" %}
Что важно знать:

* доступ к CRM и ботам появляется только после добавления в Space
* роль на уровне компании и роль внутри Space работают отдельно
* одного и того же пользователя можно добавлять в разные Spaces с разными ролями
{% endhint %}

### Где находится **Space**

**Company →  Spaces → выберите нужный Space.**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (98).png" alt=""><figcaption><p>Управление участниками внутри Space</p></figcaption></figure></div>

{% hint style="info" %}
Интерфейс

Основной экран показывает список участников Space и их роли.
{% endhint %}

### Что можно сделать в разделе

{% hint style="success" %}
* добавить нового участника в Space
* назначить или изменить роль
* ограничить доступ к разделам Space
* удалить участника из Space
{% endhint %}

{% hint style="success" icon="question" %}
Как добавить пользователя в Space

<details>

<summary>Пошаговая инструкция</summary>

* Откройте нужный Space

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (98).png" alt=""><figcaption></figcaption></figure></div>

* Нажмите Add user

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (99).png" alt=""><figcaption></figcaption></figure></div>

* Выберите пользователя из списка

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (100).png" alt=""><figcaption></figcaption></figure></div>

* Назначьте роль в Space

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown (101).png" alt=""><figcaption></figcaption></figure></div>

</details>
{% endhint %}

{% hint style="danger" %}
Права, выданные в Space, действуют только внутри этого Space.

Они не меняют роль пользователя на уровне компании.
{% endhint %}

### Роли в Space

Ниже перечислены роли, которые можно выдать пользователю внутри Space.

***

<details>

<summary>Owner</summary>

{% hint style="success" %}
Создатель Space.

Права:

* полный доступ ко всем разделам Space
* управление участниками и их ролями
{% endhint %}

</details>

<details>

<summary>Admin</summary>

{% hint style="success" %}
Администратор Space.

Права:

* полный доступ внутри Space
* управление участниками Space
{% endhint %}

{% hint style="danger" %}
Ограничения:

* не может удалить владельца Space (Owner)
{% endhint %}

</details>

<details>

<summary>Manager</summary>

{% hint style="success" %}
Роль для руководителей и аналитиков.

Права:

* управление CRM внутри Space
* настройка ботов
* создание и редактирование скриптов продаж
{% endhint %}

</details>

<details>

<summary>Operator</summary>

{% hint style="success" %}
Роль для сотрудников, которые общаются с лидами.

Права:

* работа с чатами
{% endhint %}

{% hint style="danger" %}
Ограничения:

* нет доступа к настройкам ботов
* нет доступа к скриптам продаж
*
{% endhint %}

</details>

<details>

<summary>Hide Operator</summary>

{% hint style="success" %}
Оператор с анонимизацией данных лида.

Особенности:

* имя лида заменяется на `ChatterfyID`
* &#x20;скрывается `USERNAME`
{% endhint %}

</details>

<details>

<summary>Controller</summary>

{% hint style="success" %}
Роль для контроля качества.

Права:

* просмотр и анализ чатов
* просмотр статистики по операторам
{% endhint %}

</details>

<details>

<summary>Viewer</summary>

{% hint style="success" %}
Роль только для просмотра.
{% endhint %}

{% hint style="danger" %}
Ограничения:

* нельзя отправлять сообщения
* нельзя менять настройки
{% endhint %}

</details>

***

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
