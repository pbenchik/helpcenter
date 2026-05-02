---
icon: laptop
---

# Auto actions- раздел campaing

Раздел _Auto Actions_ нужен для автоматической обработки событий после postback.

Здесь можно менять **Flow**, **Step** и **Status** без ручных действий.

### Видео

{% embed url="https://www.youtube.com/watch?v=fSAfJ_zMdAQ" %}

### Как это работает

Система получает событие через postback и ищет пользователя по `clickid`.

После этого правило переводит пользователя на нужный этап воронки.

### Шаги

#### 1. Откройте кампанию

Перейдите в `Tracker → Campaigns` и выберите нужную кампанию.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2159.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2160.png" alt=""><figcaption></figcaption></figure></div>

#### 2. Откройте вкладку **Auto Actions**

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2161.png" alt=""><figcaption></figcaption></figure></div>

#### 3. Выберите событие

Укажите `Event`, при котором должно сработать правило.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2161 (2).png" alt=""><figcaption></figcaption></figure></div>

#### 4. Заполните действие

Укажите:

* `Flow`
* `Step`
* `Status`

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2161 (1).png" alt=""><figcaption></figcaption></figure></div>

#### 5. Нажмите **Save**

После сохранения правило начнёт срабатывать автоматически.

<div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2162.png" alt=""><figcaption></figcaption></figure></div>

### Поля

* **Event** — событие, при котором запускается правило
* **Flow** — воронка, в которую нужно перевести пользователя
* **Step** — шаг внутри выбранного Flow
* **Status** — статус диалога, который система установит автоматически

### Notes

{% hint style="warning" %}
Без корректного `clickid` система не сможет найти пользователя и применить правило.
{% endhint %}

* Перед настройкой проверьте интеграцию с продуктом, макрос `{{tracker.clickid}}` в регистрационной ссылке и выбранный **DM bot**
* После сохранения проверьте, что событие приходит, а **Flow**, **Step** и **Status** меняются в нужный момент

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
