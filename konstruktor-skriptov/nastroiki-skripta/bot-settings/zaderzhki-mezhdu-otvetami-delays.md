---
description: Delays - настройка основной задержки перед ответом юзеру.
---

# Задержки между ответами (Delays)

<figure><img src="../../../.gitbook/assets/CleanShot 2024-09-24 at 16.55.54@2x.png" alt=""><figcaption></figcaption></figure>

* **Response time for the lead** - это время, которое пройдет после последнего сообщения от пользователя до запуска степа.
* **AI Reply answer speed** - это задержка для Ai Reply, от момента получения последнего сообщения до отправки ответа пользователю (т.е. Response time for the lead + задержка на работу ai)

{% hint style="success" %}
**например**, в **Response time for the lead** стоит 1 минута, а на **AI Reply answer speed** 1 минута 20 секунд, то это **Response time for the lead + 20 секунд**
{% endhint %}

* &#x20;**Send message answer** - это задержка для Send Message, от момента получения последнего сообщения до отправки ответа пользователю
* **Typing speed** - скорость набора текста ИИ

{% hint style="info" %}
Чтобы ИИ самостоятельно отправлял сообщения с задержкой в 5-10 секунд, установите более низкую скорость набора текста (Typing Speed) в настройках.
{% endhint %}
