---
icon: right-left-large
---

# Push Messages

> ### Как работают push messages

{% hint style="info" %}
* Каждый следующий пуш отправляется после предыдущего
* Delay работает между пушами:
* второй пуш отправится через указанное время после первого
* третий - после второго
* Пуши отправляются только если пользователь не отвечает
{% endhint %}

### Типы пушей:

{% hint style="info" %}
Доступны те же типы, что и в Send Message:

* Text - текст
* Media - изображения и видео
* Document - файлы
* Video note — кружочки
* Voice - голосовые сообщения
{% endhint %}

### Push Messages (Пуши):

{% hint style="info" %}
Здесь настраиваются сами пуши.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (57).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

***

### Global push messages:

{% hint style="info" %}
Использование глобальных пушей из настроек бота.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2256 (17).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

***

### Step push messages:

{% hint style="info" %}
Пуши, которые настраиваются вручную внутри шага.

Добавляются через кнопку Add push.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (59).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



***

### Пример использования:

{% hint style="info" %}
Сценарий: пользователь не ответил после первого сообщения

1 пуш (через 10 минут):\
"Вы еще с нами? 😊"

2 пуш (через 1 час):\
"Я могу помочь вам с регистрацией"

3 пуш (через 1 день):\
"Последнее напоминание - предложение еще актуально"
{% endhint %}

***

### Важная логика работы:

{% hint style="warning" %}
* Если пользователь ответил → пуши прекращаются
* Пуши не отправляются во время Delay
* Шаг используется как отдельный блок для догрева
{% endhint %}

***

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
