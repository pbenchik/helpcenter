---
description: Готовые шаблоны интеграций в трекере
---

# Update 29.04.2025

Раньше при интеграции у партнёров часто возникало много вопросов — что настроить, где подключить, как всё правильно запустить. Чтобы упростить процесс и сэкономить вам время, мы решили добавить готовые интеграции: всё уже продумано за вас, достаточно просто подключиться.

{% hint style="warning" %}
Некоторые интеграции пока ещё в разработке, но мы заранее подготовили для вас примеры правильной настройки.&#x20;
{% endhint %}

### ИНСТРУКЦИЯ ПО СОЗДАНИЮ КАСТОМНОЙ ИНТЕГРАЦИИ (если готовой ещё нет)

Если нужной вам интеграции в списке пока нет — не переживайте. Вы можете настроить всё вручную.



1\)  Откройте трекер. Когда окажетесь внутри, найдите в меню раздел **«Интеграции»** и перейдите туда.

<figure><img src="../../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>

2\) На этапе настройки укажите параметр, в который в вашей партнёрке будет записываться наш **clickid**.\
\
Это важно: без этого параметра мы не сможем корректно отслеживать конверсии и передавать данные.

<figure><img src="../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure>

3\) Создайте конфигурации постбеков (ваши ссылки).

Обычно делают три постбек-ссылки:

* для регистрации (**Registration**)

(вам необходимо самостоятельно задать ивенты - для регистрации registration)

* для первого депозита (**First Deposit**)

(для ФД первого депозита - sale)

* и для повторных депозитов (**Recurring Deposit**)

&#x20;(для РД - resale или sale + tid)\


<figure><img src="../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>

Чтобы увидеть сами ссылки, просто нажмите на значок **`>`** рядом с нужным полем — там и будет спрятана ваша готовая ссылка.



* Registration - вы получили готовую ссылку, которую нужно вставить в партнерку.

[https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=registration\&clickid=sub1](https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=registration\&clickid=sub1)

Если ваша партнёрка передаёт дополнительную информацию о клиентах — например, **ID пользователя** или **гео** вы можете настроить, какие именно данные хотите забирать.

Для этого нужно прописать:

1. **Ключ кастомного поля** - кастомное поле, которое вы создали внутри Chatterfy.
2. **Параметр** — откуда именно в партнёрке брать значение

<figure><img src="../../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**ПРИМЕР:**\
\
Пишите `fields.userid` — и указываете, что он подтягивается из `{user_id}` партнёрки.
{% endhint %}



* First Deposit  - вы получите ссылку, но сразу вставлять её в партнёрку нельзя.&#x20;

Сначала ccылку нужно правильно **самостоятельно** **преобразовать** — настроить все параметры так, чтобы партнёрка понимала, что за событие вы передаёте.

{% hint style="info" %}
Вы получите: \
\
&#x20;[https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=first\_deposit\_\&clickid={sub1}](https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=first_deposit_\&clickid={sub1})
{% endhint %}

\
Дальше — важно:\
**вам нужно самостоятельно преобразовать ссылку** под свою партнёрку.

{% hint style="success" %}
Пример готовой преобразованной ссылки:\


[https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?](https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=first_deposit_\&clickid={sub1})[tracker.event=sale\&clickid={sub1}\&tracker.cost={amount}\&tracker.currency=usd](https://api.chatterfy.ai/api/postbacks/6d1f4e36-b910-4fa1-98f0-11a2df93f054/tracker-postback?tracker.event=sale\&clickid={sub1}\&tracker.cost={amount}\&tracker.currency=usd)
{% endhint %}

Здесь:

`{amount}` — сумма депозита,

`{currency}` — валюта операции.

Эти параметры могут отличаться в зависимости от вашей партнёрки.



* Recurring Deposit  - вы получите ссылку, **но сначала её нужно правильно преобразовать**

{% hint style="info" %}
Вы получите: \
\
[https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=recurring\_deposit\_\&clickid={sub1}](https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=recurring_deposit_\&clickid={sub1})
{% endhint %}

Дальше — важно:\
**вам нужно самостоятельно преобразовать ссылку** под свою партнёрку

{% hint style="success" %}
Пример готовой преобразованной ссылки:\
\
[https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=resale\&clickid={sub1}\&tracker.tid={event\_id}](https://api.chatterfy.ai/api/postbacks/48d0524a-3abb-4cd5-82b8-404fa1cb4f7e/tracker-postback?tracker.event=resale\&clickid={sub1}\&tracker.tid={event_id})
{% endhint %}



3\) Далее переходим в раздел создания ссылки \
\
`Link name` - Registration (внутреннее название вашей ссылки) \
`Base URL` - вставьте ссылку которую вам дала партнерка (ссылка которую вы даете лиду)&#x20;

В разделе **Final URL with Parameters** вы получите готовую ссылку, в которой уже будут стоять все необходимые параметры.

В эту ссылку вы можете добавлять любые параметры, нужные вам, например:\
\
https://api.chatterfy.ai?sub4=\{{tracker.clickid\}}\&fields.userid={user\_id} - в данном случае мы из партнерки может автоматически забрать ID клиента и записать его в кастомное поле внутри СРМ&#x20;

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

### ИНСТРУКЦИЯ ПО НАСТРОЙКЕ ГОТОВЫХ ИНТЕГРАЦИЙ&#x20;

{% hint style="info" %}
Разберем на примере IGaming, везде где написано soon - значит, что интеграция еще в разработке
{% endhint %}

1\) Нажимаем на интеграцию 1win

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

2\) На этапе настройки укажите параметр, в который в вашей партнёрке будет записываться наш **clickid (в данном примере - sub4)**

<figure><img src="../../.gitbook/assets/image (101).png" alt=""><figcaption></figcaption></figure>

2\) Конфигурации постбеков в данном случае создавать не нужно - они уже заранее настроены. Открываем доступные ссылки и забираем готовые — просто вставляем их в партнёрку.\


<figure><img src="../../.gitbook/assets/image (109).png" alt=""><figcaption></figcaption></figure>

3\) Далее нам нужно получить готовую ссылку, которую нужно передать лидам. \
\
Для этого переходите в раздел **Ссылки регистрации (Registration links)**, вставьте свою ссылку (ее вам выдала партнерка) — готово, в поле **Готовая ссылка с параметрами (Final URL with Parameters)** в получаете готовую ссылку, которую будете выдавать клиентам внутри нашей CRM\
\
В эту ссылку вы можете добавлять любые параметры, нужные вам, например:\
\
https://api.chatterfy.ai?sub4=\{{tracker.clickid\}}\&fields.userid={user\_id} - в данном случае мы из партнерки может автоматически забрать ID клиента и записать его в кастомное поле внутри СРМ&#x20;

<figure><img src="../../.gitbook/assets/image (110).png" alt=""><figcaption></figcaption></figure>
