---
icon: indent
---

# Notifications

**Notifications** отправляют уведомления о событиях в диалогах бота.

Они помогают оповещать команду о чатах, которые требуют ручной проверки.

### Видео

{% embed url="https://youtu.be/pYCUUyoCDtA" %}

### Как это работает

Чтобы получать уведомления, нужно подключить Telegram-чат к боту или личке.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (8).png" alt=""><figcaption></figcaption></figure></div>

После сохранения уведомления начнут отправляться в указанный чат.

### Подготовьте чат

Сначала выберите чат, куда будут приходить уведомления.

<div align="center" data-full-width="false" data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (158).png" alt=""><figcaption></figcaption></figure></div>

#### Steps / Instructions

1. Создайте или выберите нужный Telegram-чат.
2. Убедитесь, что чат подходит для уведомлений команды.

### Получите Telegram ID

Для подключения нужен `Telegram ID` выбранного чата.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (9).png" alt=""><figcaption></figcaption></figure></div>

#### How it works

Формат `Telegram ID` зависит от типа подключения:

* если это бот, ID указывается с минусом: `-2894347`
* если это личка, ID указывается без минуса: `2894347`

#### Steps / Instructions

1. Добавьте `@username_to_id_bot` в нужный чат.
2. Отправьте команду `/start`.
3. Скопируйте ID чата из ответа бота.

#### Notes

* Нужен именно ID чата.

### Добавьте ID в настройки

Теперь нужно сохранить `Telegram ID` в настройках бота.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2255.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2254.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2253.png" alt=""><figcaption></figcaption></figure></div>

#### Steps / Instructions

1. Откройте нужного бота в платформе.
2. Перейдите в **Bot Settings**.
3. Откройте раздел **Notifications**.
4. Вставьте `Telegram ID`.

### Настройте условия отправки

После добавления `Telegram ID` выберите, при каком событии отправлять уведомление.

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2252.png" alt=""><figcaption></figcaption></figure></div>

#### Steps / Instructions

1. Добавьте параметр, при котором должно отправляться уведомление.
2. Сохраните изменения.

#### Notes

* После сохранения уведомления начнут отправляться в указанный чат.

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
