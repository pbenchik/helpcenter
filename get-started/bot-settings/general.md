---
icon: table-pivot
---

# General

> ### General — это основная вкладка настроек бота или лички.

Здесь управляют статусом бота, базовой информацией, таймзоной и текущим space.

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248.png" alt=""><figcaption></figcaption></figure></div>

**General используют для:**

* запуска и остановки бота
* изменения имени, описания и тегов
* настройки часового пояса
* переноса бота в другой space
{% endhint %}

{% hint style="warning" %}
**Изменения в этой вкладке влияют на базовую работу бота.**

Перед архивированием или переносом проверьте, что это не сломает текущие процессы.
{% endhint %}

### Как работает General:

{% hint style="info" %}
**Во вкладке собраны основные параметры бота.**

Здесь можно:

* активировать бота через **Activate**
* остановить работу через **Stop**
* убрать бота из активной работы через **Archive**
* изменить имя и описание
* проверить `username`
* добавить или обновить теги
* задать таймзону
* выбрать другой space
{% endhint %}

### Важно:

<details>

<summary>1. Main settings</summary>

{% hint style="info" %}
**В верхнем блоке настраивается основная информация о боте.**

Доступные действия:

* **Activate** — активировать бота
* **Stop** — остановить бота
* **Archive** — архивировать бота
* изменить имя бота или лички
* посмотреть `username`
* добавить или изменить описание
* указать теги бота
*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (2).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

{% hint style="warning" %}
После `Archive` бот уходит из активной работы.

Используйте этот статус только если бот больше не нужен в текущем space.
{% endhint %}



</details>

<details>

<summary>2. Timezone</summary>

{% hint style="info" %}
**В блоке Timezone задаётся часовой пояс бота.**

Система использует его во всех действиях, связанных со временем.

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (3).png" alt=""><figcaption></figcaption></figure></div>


{% endhint %}

{% hint style="info" %}
**Таймзона влияет на:**

* задержки в шагах
* отложенные действия
* временные условия в сценариях
* логику, завязанную на дате и времени
{% endhint %}

{% hint style="warning" %}
**Если таймзона указана неверно, задержки и условия могут срабатывать не в то время.**

Проверьте её перед запуском автоматизаций.
{% endhint %}



</details>

<details>

<summary>3. Space</summary>

{% hint style="info" %}
**В этом блоке бот переносится в другой space.**

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (4).png" alt=""><figcaption></figcaption></figure></div>

**Для этого:**

1. Откройте список в поле **Space**.
2. Выберите нужный space.
3. Сохраните изменение.
{% endhint %}

{% hint style="warning" %}
**После переноса меняется рабочий контекст бота.**

Проверьте доступы, команду и нужные настройки в новом space.
{% endhint %}



</details>

### Когда использовать General:

{% hint style="success" %}
**Используйте эту вкладку, когда нужно:**

* изменить базовые данные бота
* включить или остановить бота
* обновить теги и описание
* настроить корректную таймзону
* перенести бота в другой space
{% endhint %}

{% include "../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
