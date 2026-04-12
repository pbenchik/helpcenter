---
icon: laptop
---

# Auto actions- раздел campaing

> ### Auto Actions - это раздел Campaigns для автоматической обработки событий после postback.

{% hint style="info" %}
С его помощью можно:

* автоматически переводить пользователя на другой этап
* запускать изменение воронки после события
* обновлять статус диалога без участия менеджера
* связывать postback от продукта с логикой бота
{% endhint %}

### Видеоинструкция:

{% hint style="info" icon="laptop" %}
В видео показано, как работать с разделом Auto Actions внутри Campaigns.

Подойдёт, если нужно быстро понять логику выбора события, настройки действия и автоматического перевода пользователя в нужный `Flow`, `Step` и `Status`.

{% embed url="https://www.youtube.com/watch?v=fSAfJ_zMdAQ" fullWidth="false" %}
{% endhint %}

### Как работает Auto Actions:

{% hint style="info" %}
Здесь настраивается, что должно произойти с пользователем после получения конкретного события.
{% endhint %}

{% hint style="info" %}
Это нужно, чтобы автоматически двигать пользователя по воронке без ручных действий.
{% endhint %}

### Как настроить Auto Action:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Откройте Campaigns и выберите нужную кампанию**

    Перейдите в `Tracker → Campaigns`.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2159.png" alt=""><figcaption></figcaption></figure></div>

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2160.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Перейдите во вкладку Auto Actions**

    Откройте раздел `Auto Actions` внутри кампании.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2161.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Выберите событие**

    Укажите `Event`, при получении которого должно сработать действие.

    Обычно это событие приходит от продукта через postback.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2161 (2).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Заполните действие**

    Укажите:

    * `Flow`
    * `Step`
    * `Status`

    Эти поля определяют, как именно изменится состояние пользователя после события.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2161 (1).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **Сохраните настройку**

    Нажмите `Save`.

    После сохранения правило начнёт срабатывать автоматически.

    <div data-with-frame="true"><figure><img src="../../../.gitbook/assets/Frame 2162.png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Что настраивается в Auto Actions</summary>

{% hint style="info" %}
В этом разделе обычно задают:

* событие, при котором срабатывает правило
* `Flow`, в который нужно перевести пользователя
* `Step`, на который нужно перевести пользователя
* `Status`, который нужно установить диалогу
* логику автоматического перехода после postback
{% endhint %}

</details>

<details>

<summary>Что проверить перед настройкой</summary>

{% hint style="info" icon="exclamation" %}
Перед настройкой Auto Actions проверьте:

* интеграция с продуктом уже настроена
* в регистрационной ссылке передаётся макрос `{{tracker.clickid}}`
* в кампании выбран `DM bot`
{% endhint %}

</details>

<details>

<summary>Какую роль Auto Actions играет в системе</summary>

{% hint style="warning" %}
Сначала Tracker получает событие через postback.

Обычно это событие приходит после регистрации, депозита или другого действия в продукте.
{% endhint %}

{% hint style="warning" %}
Дальше Tracker ищет пользователя по `clickid`.

Без корректного `clickid` правило не сможет примениться к нужному пользователю.
{% endhint %}

{% hint style="warning" %}
После этого система применяет заданное правило.

Она может изменить `Flow`, `Step` и `Status` для выбранного пользователя.
{% endhint %}

</details>

<details>

<summary>Какие поля есть в Auto Actions</summary>

{% hint style="info" %}
Основные поля:

* `Event` — событие, при получении которого запускается правило
* `Flow` — воронка, в которую нужно перевести пользователя
* `Step` — конкретный шаг внутри выбранного Flow
* `Status` — статус диалога, который будет установлен автоматически
{% endhint %}

</details>

<details>

<summary>Что проверить после настройки</summary>

{% hint style="info" %}
После сохранения проверьте:

* событие реально приходит в Tracker
* у пользователя передаётся корректный `clickid`
* выбран правильный `Flow`
* выбран правильный `Step`
* статус диалога меняется в ожидаемый момент
{% endhint %}

</details>

### Где удобно использовать Auto Actions:

{% hint style="success" %}
Auto Actions удобно использовать, когда нужно:

* автоматически двигать пользователя по воронке
* запускать новые сценарии после регистрации или депозита
* синхронизировать postback с логикой бота
* ускорять обработку лидов без ручных действий
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
