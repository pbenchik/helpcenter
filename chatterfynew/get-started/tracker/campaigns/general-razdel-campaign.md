---
icon: head-side-gear
---

# General - раздел campaign

Раздел _General_ нужен для настройки маршрута пользователя после клика.

Здесь вы выбираете точку входа в Telegram и стартовый сценарий.

### Видео

{% embed url="https://youtu.be/hYwNhUlfXJ0" fullWidth="false" %}

### Как это работает

Во вкладке **General** определяется, куда попадёт пользователь.

Здесь же задаются **Flow**, **Step** и **DM bot** для дальнейшей обработки.

### Шаги

1. выберите тип маршрута
2. укажите **Invite Bot** или **Bot**
3. при необходимости выберите **Channel**
4. задайте **Start Flow** и **Start Step**
5. укажите **DM bot**

### Поля

#### **Campaign traffic type**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure></div>

* `Channel` — пользователь сначала попадает в Telegram-канал
* `Bot` — пользователь сразу попадает в Telegram-бота

#### **Invite Bot / Bot**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure></div>

* **Invite Bot** нужен для типа `Channel`
* **Bot** нужен для типа `Bot`

#### **Channel**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure></div>

Поле доступно только для типа `Channel`.

#### **Start Flow** и **Start Step**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure></div>

* **Start Flow** — Flow, который запускается после перехода
* **Start Step** — первый Step выбранного Flow

#### **DM bot**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure></div>

**DM bot** принимает лида и помогает получить событие `contact`.

#### **Start Flow** и **Start Step** для **DM bot**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure></div>

Это отдельный сценарий для **DM bot**.

#### **Approval time**

Параметр **Approval time** задаёт задержку перед автоматическим принятием пользователя в канал.

### Notes

{% hint style="warning" %}
Для сценария `Channel` **Invite Bot** должен быть активирован и назначен администратором канала с правом принимать заявки.
{% endhint %}

* Следующие вкладки: [Sources](sources-razdel-campaign/), [Auto actions](auto-actions-razdel-campaing.md), [Parameters](parameters-razdel-campaing.md), [Test](test-razdel-campaign.md)

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
