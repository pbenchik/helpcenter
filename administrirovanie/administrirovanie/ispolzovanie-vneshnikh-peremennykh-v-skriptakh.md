# Использование внешних переменных в скриптах

В скриптах бота можно также использовать внешние переменные, такие как:

* Чат ID диалога из телеграма = {chatId} - Telegram chat id
* Дата начала диалога с ботом в Chatterfy = {createdAt} - Date & time when dialogue start
* key степа на котором сейчас находится чат  = {stepId} - StepKey from flow
* автоматический передаваемый постбеком ID = {trader\_id} - trader\_id
* автоматический передаваемый постбеком ID = {clickid} - clickid

Помимо этого возможно также использование имени юзера:

* \{{username\}} - юзернейм(логин) юзера в Telegram



{% hint style="info" %}
Например, можем создать ссылку для отправки юзеру (включив ее в промпт):\
[https://partner.com?sub1=\{{tracker.clickid\}}](https://partner.com/?sub1=\{{chat.tracker.clickid\}})
{% endhint %}
