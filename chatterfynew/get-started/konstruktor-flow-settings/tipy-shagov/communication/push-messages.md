---
icon: right-left-large
---

# Push Messages

Push messages — это отложенные сообщения, которые отправляются, если пользователь не отвечает.

### Как это работает

* каждый следующий пуш отправляется после предыдущего
* `Delay` работает между пушами
* пуши отправляются только если пользователь молчит

### Типы пушей

* **Text** — текст
* **Media** — изображения и видео
* **Document** — файлы
* **Video note** — видеокружки
* **Voice** — голосовые сообщения

### Push Messages

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (57).png" alt=""><figcaption></figcaption></figure></div>

Здесь настраиваются сами пуши.

### Global push messages

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2256 (17).png" alt=""><figcaption></figcaption></figure></div>

* используются глобальные пуши из настроек бота

### Step push messages

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (59).png" alt=""><figcaption></figcaption></figure></div>

* пуши настраиваются вручную внутри шага
* добавляются через **Add push**

### Пример

Сценарий: пользователь не ответил после первого сообщения.

* 1 пуш через `10` минут
* 2 пуш через `1` час
* 3 пуш через `1` день

### Notes

{% hint style="warning" %}
Если пользователь ответил, пуши прекращаются.

Пуши не отправляются во время `Delay`.
{% endhint %}

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
