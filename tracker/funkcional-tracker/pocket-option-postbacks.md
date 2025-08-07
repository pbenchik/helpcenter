---
description: Настройка интеграции с Pocket Option
---

# Pocket Option Postbacks

Эта инструкция поможет вам шаг за шагом настроить отправку постбеков из Pocket Option в Chatterfy. Постбеки позволяют автоматически отслеживать действия пользователей: регистрацию, подтверждение email и внесение депозита.\
\
Перед тем как настраивать постбеки в Pocket Option, нужно сначала создать интеграцию в Chatterfy.

#### Настройка интеграции в Chatterfy

1. Зайдите в личный кабинет **Chatterfy**.
2. Перейдите в раздел **Трекер → Интеграции**.
3. Найдите и выберите интеграцию **PocketOption RevShare**.
4. Нажмите кнопку **Configure**.

<figure><img src="../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

5. В настройках укажите, в какой параметр в Pocket вы будете передавать наш `click_id`. Чаще всего используется `click_id`.

<figure><img src="../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure>

**Создайте 3 конфигурации:**

* **registration** — регистрация пользователя
* **conf** — подтверждение email
* **resale** — депозит

Вот примеры ссылок, которые нужно использовать:

<table><thead><tr><th>Событие</th><th>Назначение</th><th width="433.2666015625">Ссылка для вставки в Pocket</th></tr></thead><tbody><tr><td><code>registration</code></td><td>Регистрация пользователя</td><td><code>https://api.chatterfy.ai/api/postbacks/7878f1d1-3693-4d08-9c91-fa8a834e7abc/tracker-postback?tracker.event=registration</code></td></tr><tr><td><code>conf</code></td><td>Подтверждение email-адреса</td><td><code>https://api.chatterfy.ai/api/postbacks/7878f1d1-3693-4d08-9c91-fa8a834e7abc/tracker-postback?tracker.event=conf</code></td></tr><tr><td><code>resale</code></td><td>Совершение депозита</td><td><code>https://api.chatterfy.ai/api/postbacks/7878f1d1-3693-4d08-9c91-fa8a834e7abc/tracker-postback?tracker.event=resale&#x26;currency=usd</code></td></tr></tbody></table>



Скопируйте эти ссылки — они понадобятся на следующем этапе.



Теперь переходим к личному кабинету **Pocket Option**, где нужно создать по одному постбеку на каждое событие.



**Пример: настройка события registration**&#x20;

1. Откройте раздел постбеков в Pocket Option.
2. Нажмите **добавить постбек**.
3. В поле **URL** вставьте соответствующую ссылку (в нашем примере — ссылка для события `registration`).

{% hint style="info" %}
Не забудьте, что для каждого нового события нужно создавать новый постбек&#x20;
{% endhint %}

4. Заполните остальные поля в соответствии с примером на скриншоте.

<figure><img src="../../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure>

После этого Pocket Option выдаст вам **партнёрскую ссылку для клиента (скопируйте ее как указано на скриншоте ниже)**.&#x20;

<figure><img src="../../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

Затем в **Chatterfy**, в разделе **Трекер → Интеграции**, вставьте полученную ссылку в поле **Registration links**, следуя примеру ниже.

В результате вы получите **готовую ссылку с автоматически подставленным макросом**. Эту ссылку вы сможете использовать в своих скриптах для корректной передачи `click_id`.

<figure><img src="../../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

Обратите внимание, как вставлять click\_id:



* Если параметр один:\
  `?click_id={{tracker.clickid}}`
* Если параметров несколько, добавляйте через `&`:\
  Пример: \
  [`https://pocketcustomer.com/register?utm_campaign=764984&utm_source=affiliate&code=JOINHERE123&click_id={{tracker.clickid}}`\
  ](https://pocketcustomer.com/register?utm_campaign=764984\&utm_source=affiliate\&code=JOINHERE123\&click_id=\{{tracker.clickid\}})



2. **Настройка события `conf`**

Настраивается аналогично скриншоту предоставленному ниже:

<figure><img src="../../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure>

3.  **Настройка события `resale`**

    Так же, как и два предыдущих. Только используйте соответствующую ссылку с параметром `currency=usd`:



`https://api.chatterfy.ai/api/postbacks/7878f1d1-3693-4d08-9c91-fa8a834e7abc/tracker-postback?tracker.event=resale&currency=usd`

<figure><img src="../../.gitbook/assets/image (400).png" alt=""><figcaption></figcaption></figure>

#### ✅ ФИНАЛЬНЫЙ ЭТАП - САМЫЙ ВАЖНЫЙ !!!&#x20;

#### Проверка после настройки:

* Совершите тестовую регистрацию.
* Убедитесь, что события отображаются в Chatterfy (Tracker - Postback Logs).
* Если что-то не работает — проверьте правильность вставки click\_id и соответствие ссылок.
