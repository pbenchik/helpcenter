# Send Webhook

**Send webhook -** это функционал отправки информации из Chatterfy в любые внешние сервисы посредством отправки webhooks.&#x20;

{% hint style="info" %}
Чтобы добавить отправку вебхуков, вам необходимо добавить новый шаг **Send webhook.**
{% endhint %}

1\. Нажмите на кнопку "Create step"

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-09-30/82057b28-94f1-4eed-82f6-1711fe36476a/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1306,870\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=365,217)

2. Нажмите на кнопку Send Webhook

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-09-30/11e296e2-c430-4fa4-b0fa-d61afc3055a4/user_cropped_screenshot.jpeg?tl_px=0,152\&br_px=1145,1114\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=555,485)

<figure><img src="../../../.gitbook/assets/Screen Shot 2024-08-14 at 7.58.04 PM.png" alt=""><figcaption></figcaption></figure>

* **Доступные переменные для отправки:**

{username} - Имя пользователя в телеграмм. (текстовое значение)

{chatId} - ChatID пользователя в телеграм. (числовое значение)

{stepKey} - Ключ шага, на котором находится пользователь (текстовое значение)

{createdAt} - Время начала диалога (2024-03-10T17:49:32.806Z)&#x20;

{KEYCUSTOMFIELD} - Ключ из ваших кастомных полей. Замените KEYCUSTOMFIELD на ваш KEY кастомного поля, который можно найти в Bot Settings

{tracker.KEYTRACKERFIELD} - Ключ из ваших трекер филдов. Например, {tracker.clickid}



{% hint style="info" %}
Примеры отправок webhooks
{% endhint %}

{% hint style="success" %}
```
https://keitaro.yoursite.com/25123a/postback?subid={tracker.clickid}&username={username}&chatid={chatId}&startdialogue={createdAt}
```
{% endhint %}

* **В этом вебхуке мы передаем параметры в keitaro по формату:**

subid={tracker.clickid} - передаем для Keitaro clickid юзера, который был задан для этого пользователя трекером&#x20;

username={username} - имя пользователя телеграмма

chatid={chatId} - ID пользователя телеграмма

startdialogue={createdAt} - время начала диалога
