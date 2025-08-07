# Удаленная настройка CRM

## Auto Actions ивенты через postback

Auto Actions - это функционал позволяющий автоматизировать ваши воронки и полностью избавиться от обработчиков. Когда вы получите постбэк от продукта (например событие первого депозита от 1win) - для пользователя с тем clickid, который был указан при регистрации автоматически изменится шаг диалога и ИИ может продолжать общаться с лидом ЗНАЯ, что человек сделал депозит/регистрацию и тд.

Чтобы данный функционал работал, вам необходимо настроить Постбэки на продукте и ОБЯЗАТЕЛЬНО передавать clickid в партнерку. Без этого система НЕ будет знать, кому из диалогов нужно изменить шаг.

[Postbacks](https://help.chatterfy.ai/tracker/funkcional-tracker/postbacks)

## Пример реализации

<figure><img src="../../.gitbook/assets/image (299).png" alt=""><figcaption></figcaption></figure>

При поступлении постбэка с типом: "**sale**" - для лида автоматически изменится шаг на Flow RD, step FD, статус диалога Auto

При поступлении постбэка с типом: "**resale**" - для лида автоматически изменится шаг на Flow RD, шаг 2rd, статус Auto

При поступлении постбэка с типом: "**registration**" - для лида автоматически изменится шаг на Flow FD, шаг REG, статус Auto

<figure><img src="../../.gitbook/assets/image (300).png" alt=""><figcaption></figcaption></figure>

## Дополнительные возможности для повторных депозитов

Вы можете добавлять бесконечное множество действий, нажав на кнопку "Add action"

<figure><img src="../../.gitbook/assets/image (301).png" alt=""><figcaption></figcaption></figure>

Для события resale (повторный депозит) можно использовать числовое значение депозита, к примеру "resale#2" - это действие при ВТОРОМ повторном депозите, "resale#3" при третьем и тд.

Вы также можете добавлять кастомные действия, если продукт отдает такие события в постбэках, напримере бинарных опционов часто можно встретить событие "withdrawal", благодаря обработке которого вы можете изменить шаг диалога в тот момент, когда пользователь сделает вывод с платформы.

## Postbacks

Для получения данных из партнерки вам необходимо настроить постбеки. Здесь вы найдете пошаговую инструкцию

1. Перейдите в трекер и нажмите Postbacks (Постбеки
2. Чтобы создать постбек нажмите Create postback

<figure><img src="../../.gitbook/assets/image (303).png" alt=""><figcaption></figcaption></figure>

3. Введите Name, Affilliate network - на данный момент есть кастомы 1win и Binomo и нажмите создать.\
   \
   **Affiliate Network** - на данный момент внутри платформы представлены 2 партнерки 1Win и Binomo. Если ваша партнерка не представлена, то просто выберите Custom
4. **Campaign** - если выбрать, то постбеки будут уникальные только для определенного выбранного кампейна. Лучше не выбирать, чтобы постбэки для всех кампейнов были общие
5. Нажмите Create - создать постбэк

<figure><img src="../../.gitbook/assets/image (304).png" alt=""><figcaption></figcaption></figure>

## Постбеки в трекере (запись внешних данных)&#x20;

[Инструкция по созданию кастомных полей: Нажмите, чтобы перейти](https://help.chatterfy.ai/crm-dlya-obsheniya/funkcional-crm/stranica-chatov/kastomnye-polya)

Если вам **необходимо записать и достать с кастом филдов** **информацию о клиенте** можно через **fields.кастомную информацию о клиенте**, например сумма последнего депозита, ID клиента. &#x20;

{% hint style="success" %}
Вам нужно **в постбеке трекера,** который вы **добавляете в партнерку** **добавить fields.key параметра=параметр из партнерки**&#x20;
{% endhint %}

Например, постбек для FD&#x20;

[https://api.chatterfy.ai/api/postbacks/51edc052-f7a2-4650-8085-d04abb38de5e/tracker-postback?clickid={clickid}\&tracker.event=sale\&tracker.cost={cost}\&tracker.currency=usd\&fields.last\_deposit={cost}\&fields.user\_id={user\_id}](../../chatterfy.ai/update-log/update-06.10.2024.md)

Таким образом,  **пользователю запишется ивент sale**, а **в кастом филды** пользователя **запишется параметры last\_deposit и user\_id**



## Webhooks & Api

{% hint style="info" %}
**Для того, чтобы подключить к вашему сервису необходимо** п**олучить уникальную ссылку для WebHooks.**
{% endhint %}

1. **Откройте вашего бота**
2. Настройки скрипта (значок шестеренки)
3. Bot settings (слева в верхнем углу)
4. Нажмите "Add Webhook"
5. Нажмите "SAVE" внизу экрана для сохранения изменений

<figure><img src="../../.gitbook/assets/image (306).png" alt=""><figcaption></figcaption></figure>

Можно создать несколько ссылок на одного бота, это бывает полезно чтобы использовать несколько сервисов. Если у вас несколько ботов, каждая ссылка будет уникальна.

{% hint style="info" %}
Уникальная ссылка выглядит так: https://app.chatterfy.ai/api/bots/webhooks/\<POSTBACK\_ID>/updateDialog \


**ПРИМЕР:** [**https://app.chatterfy.ai/api/bots/webhooks/55833627-242e-4061-9b0a-30da3e9cf7d4/updateDialog**](https://app.chatterfy.ai/api/bots/webhooks/55833627-242e-4061-9b0a-30da3e9cf7d4/updateDialog)
{% endhint %}

* WebHooks позволяют изменять параметры диалогов, управлять переходами между шагами и добавлять теги
* **Для взаимодействия с чатами пользователей мы используем Telegram ChatID**

**`chatId=1227280`**

На месте "1227280" вы должны передать Telegram ChatID пользователя, которому необходимо внести изменения.

После того, как вы получили ссылку и научились работать с ключевым полем, **вы можете управлять диалогом при помощи вебхуков, используя переменные такие как:**

1. stepId
2. status=auto/manual/blocked
3. details.KEYCUSTOMFIELD=params

## Переключения шагов

Для переключения пользователя на конкретный шаг необходимо отправить:

— chatId — ID чата в Telegram

— stepId — ID шага в вашем боте, на который необходимо перевести диалог

{% hint style="info" %}
Отправлять параметры можно через **GET**.

**Пример: https://app.chatterfy.ai/api/bots/webhooks/\<POSTBACK\_ID>/updateDialog?chatId=1227280\&stepId=046050f6-38f6-4b18-b9fa-e6582f5352d0**
{% endhint %}

## Передача дополнительной информации в диалог

Используйте параметр (объект) fields.\[ключ поля] для добавления дополнительных данных в диалог.

**1) Пример 1** - **сохранение уникального refID из внешней системы**

https://app.chatterfy.ai/api/bots/webhooks/\<POSTBACK\_ID>/updateDialog?chatId=1227280\&details.refID=12345

{% hint style="info" %}
**ПРИМЕР:** https://app.chatterfy.ai/api/bots/webhooks/8f1el0ed-a1d2-4a9d-bc30-2e19f2062789/updateDialog?chatId=1227280\&fields.refID=12345
{% endhint %}

**2) Пример 2 - запись баланса пользователя**

https://app.chatterfy.ai/api/bots/webhooks/\<POSTBACK\_ID>/updateDialog?chatId=1227280\&fields.userBalance=5000

{% hint style="info" %}
**ПРИМЕР:** https://app.chatterfy.ai/api/bots/webhooks/8f1el0ed-a1d2-4a9d-bc30-2e19f2062789/updateDialog?chatId=1227280\&fields.userBalance=5000
{% endhint %}

## Использование сохраненных данных



Для использования данных в шаблонах, вставьте соответствующие переменные в двойные фигурные скобки.

{% hint style="warning" %}
Например, https://some.service.com/signup?refId=**\{{fields.refId\}} для генерации персонализированных ссылок.**
{% endhint %}

**Дефолтное использование параметров в ссылках**

**\{{chatId\}}** - Telegram ID

**\{{username\}}** - Telegram username

**\{{name\}}** - имя пользователя

**\{{createdAt\}}** - дата создания диалога

**\{{fields.key любого кастом филда\}}** - любой ваш кастом филд, созданный в Bot Settings

**\{{tracker.key любого трекер филда\}}** - любой параметр из трекер филд, добавленный в параметрах кампании в Трекере



{% hint style="info" %}
Например,**`https://some.service.com/signup?refId={{fields.refId}}`**
{% endhint %}



## Примеры



1\) Если пользователь открыл лендинг с utm параметром ad\_name=test, то у пользователя будет трекер филд ad\_name со значением test. **Затем вы сможете его использовать в общении с пользователем**, например `https://some.service.com/signup?ad_name={{tracker.ad_name}}.`&#x20;

Также, **каждый пользователь дополнительно имеет кликайди** - уникальный параметр для каждого пользователя. **Его значение можно получить, используя макрос \{{tracker.clickid\}}.**

2\) Если вы, например, **хотите** **отправить приветственное сообщение с именем пользователя,** то вы можете **создать степ Send Message** и **в тексте сообщения добавить текст** например Hello, \{{name\}}.

Частым примером использования параметров из чата является генерация ссылки на регистрацию в партнерке. Например, https://partner.com/signup?sub1=\{{tracker.clickid\}}. Таким образом вы предоставите пользователю ссылку на регистрацию в партнерку и запишите в sub1 наш clickid. Если, например, clickid пользователя =test123, то пользователь получит ссылку https://partner.com/signup?sub1=test123



{% hint style="danger" %}
**ИСКЛЮЧЕНИЕ !!!**

Если пользователь пришел в бота/личка вне кампании из трекера (например, открыл бота и нажал старт), то у данного лида не будет трекер даты и его нельзя будет трекать.
{% endhint %}



{% hint style="info" %}
**После отправки ID клиента, могу ли я проверить его в своей БД и переключить степ в зависимости от результата?**
{% endhint %}

**Вы можете в степе вебхук слать себе айди, которого нужно переключить.** Взяв нужный вам параметр, вы проверите нужно ли переключать степ или нет.

[**`https://test.com?chatId={fields.chatId}`**](https://test.com/?chatId={chatId}\&stepId={stepId})\
\
&#x20;Например, если пользователь имеет Telegram ID - 123, то вебхук отправится по адресу (URL) [**`https://test.com?chatId=123`**](https://test.com/?chatId={chatId}\&stepId={stepId}). &#x20;

Затем вы можете отправить запрос на созданный вебхук в боте `https://app.chatterfy.ai/api/bots/webhooks/<POSTBACK_ID>/updateDialog?chatId=123&stepId=`**`[степ на который нужно переключить пользователя]`**`&status=auto`

## Send Webhook



**Send webhook -** это функционал отправки информации из Chatterfy в любые внешние сервисы посредством отправки webhooks.&#x20;



{% hint style="info" %}
Чтобы добавить отправку вебхуков, вам необходимо добавить новый шаг **Send webhook.**
{% endhint %}

1\. Нажмите на кнопку "Create step"&#x20;

2.Нажмите на кнопку Send Webhook

<figure><img src="../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (309).png" alt=""><figcaption></figcaption></figure>

**Доступные переменные для отправки:**



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



## Добавление кастомных переменных в боте

\
Теперь в настройках бота (Bot Settings) появилась возможность создавать кастомные переменные, которые можно использовать через макросы.

1. Перейдите в раздел Bot Settings&#x20;
2. Пролистайте вниз, найдите поле Bot variables&#x20;
3. В поле ''Name" укажите кастомную переменную, например variables.regLink&#x20;
4. В поле Value вставьте само значение переменной, например [https://pp.com?clickid=\{{tracker.clickid\}}](https://pp.com/?clickid=\{{tracker.clickid\}})

{% hint style="success" %}
Вместо того, чтобы постоянно вставлять ссылку из примера выше в степах или сообщениях, можно использовать просто \{{variables.regLink\}}
{% endhint %}

