---
icon: arrow-right-from-arc
---

# Как работает передача событий

> ### Процесс передачи событий состоит из нескольких этапов.

{% hint style="info" %}
* Пользователь приходит из рекламы
* Пользователь нажимает на рекламное объявление и переходит по ссылке кампании.
* В этот момент Chatterfy автоматически создаёт уникальный идентификатор clickid.
* clickid - это уникальный ID клика пользователя, который создаётся системой при первом переходе по ссылке. Этот идентификатор сохраняется в системе вместе с информацией о пользователе.
{% endhint %}

***

### Пользователь получает ссылку на регистрацию:

{% hint style="info" %}
* Во время общения в боте или личке пользователю отправляется ссылка на регистрацию.
* В эту ссылку добавляется специальный макрос \{{tracker.clickid\}}
*   Пример:\
    `https://partner.com/signup?sub1={{tracker.clickid}}`

    Когда ссылка отправляется пользователю через CRM, система автоматически подставляет значение clickid.
*   Пример итоговой ссылки:\
    `https://partner.com/signup?sub1=67wgwWkaR0`

    Таким образом партнёрская программа получает clickid, который был создан при первом переходе пользователя.
{% endhint %}

***

### Партнёрская программа отправляет postback:

{% hint style="info" %}
* Когда пользователь совершает действие (например регистрацию или депозит), партнёрская программа отправляет postback в Chatterfy.
* Пример: [https://api.chatterfy.ai/api/postbacks/.../tracker-postback?clickid=67wgwWkaR0\&tracker.event=registration](https://api.chatterfy.ai/api/postbacks/.../tracker-postback?clickid=67wgwWkaR0\&tracker.event=registration)
{% endhint %}

***

### Chatterfy записывает событие:

{% hint style="info" %}
* <mark style="color:$warning;">Получив postback, Chatterfy:</mark>\
  находит пользователя по clickid\
  определяет, по какой кампании он пришёл\
  записывает событие в систему
* <mark style="color:$warning;">Например:</mark>\
  registration - регистрация\
  sale - первый депозит\
  resale - повторный депозит
* <mark style="color:$warning;">После этого данные отображаются в:</mark>\
  Analytics\
  Dashboards\
  Logs\
  карточке клиента в разделе Events
{% endhint %}

{% include "../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
