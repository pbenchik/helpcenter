---
icon: almost-equal-to
---

# Proxy

> ### В разделе Proxy подключаются прокси-серверы для отправки серверных событий.

Прокси помогает отправлять запросы с отдельного IP. Это снижает риск блокировок и повышает стабильность.

### Когда нужен Proxy:

{% hint style="info" %}
Proxy особенно полезен при работе с:

* Facebook
* другими рекламными источниками
* сценариями, где важна стабильная серверная отправка событий
{% endhint %}

### Поддерживаемые типы:

{% hint style="info" %}
* **HTTP**
* **HTTPS**
{% endhint %}

{% hint style="danger" %}
`SOCKS` не поддерживается. Если указать такой тип, события отправляться не будут.
{% endhint %}

### Как создать Proxy:

{% tabs %}
{% tab title="Инструкция" %}
{% stepper %}
{% step %}
{% hint style="info" %}
Откройте Tracker → Proxy

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}


{% endstep %}

{% step %}
{% hint style="info" %}
Нажмите Create proxy

*

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (2).jpeg" alt=""><figcaption></figcaption></figure></div>


{% endhint %}
{% endstep %}

{% step %}
#### Заполните параметры

{% hint style="info" %}
Укажите:

* **Name** — внутреннее название proxy
* **Host** — IP-адрес proxy
* **Port** — порт подключения
* **Username** — логин
* **Password** — пароль
{% endhint %}
{% endstep %}

{% step %}
#### Нажмите Save

{% hint style="info" %}
После сохранения proxy появится в списке и станет доступен в настройке Sources.
{% endhint %}
{% endstep %}
{% endstepper %}

### Как проверить Proxy:

В системе есть встроенная проверка подключения.

{% stepper %}
{% step %}
#### Откройте список Proxy
{% endstep %}

{% step %}
#### Нажмите кнопку проверки рядом с нужным proxy

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2168.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
#### Дождитесь результата

{% hint style="info" %}
Система покажет, работает ли подключение.
{% endhint %}
{% endstep %}
{% endstepper %}

### Возможные статусы:

{% hint style="info" %}
**The proxy is working** — proxy работает корректно
{% endhint %}

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (1).png" alt=""><figcaption><p>Рабочий proxy</p></figcaption></figure></div>

{% hint style="info" %}
**The proxy isn't working** — соединение отсутствует или данные указаны неверно
{% endhint %}

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (2).png" alt=""><figcaption><p>Ошибка проверки proxy</p></figcaption></figure></div>
{% endtab %}

{% tab title="Видеоинструкция" %}
{% embed url="https://www.youtube.com/watch?feature=youtu.be&v=yb9j6W2k4fc" %}
{% endtab %}
{% endtabs %}

### Если Proxy не работает:

{% hint style="info" %}
Проверьте:

* правильность `Host`
* правильность `Port`
* логин и пароль
* доступность сервера
{% endhint %}

{% hint style="info" %}
Если ошибка сохраняется, замените proxy на другой.
{% endhint %}

### Важно:

{% hint style="info" %}
* Proxy не обязателен, но часто полезен.
* Один proxy можно использовать в нескольких кампаниях.
* Страна proxy не критична.
* Важнее стабильное соединение и высокий uptime.
* Проверяйте статус proxy регулярно, чтобы не терять события.
{% endhint %}

{% include "../../../.gitbook/includes/na-glavnuyu.md" %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
