# General

## В настройках General вы будете добавлять бота авто приемщика заявок в закрытый канал. Также, вы сможете выбрать тип залива (Campaign Traffic Type) на канал или сразу же на бота.

На данной странице вы настраиваете ботов, которые будут привязаны к вашей кампании и куда будет передаваться вся необходимая информация о пользователях собранная через трекер. Основной параметр для Трекера - Clickid, весь мэтчинг данных будет строиться на основании его.

1\. Откройте вашу кампанию (Campaigns) и перейдите в раздел General

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/549e7336-9f22-48f9-b1ac-c20937bc172c/user_cropped_screenshot.jpeg?tl_px=0,102\&br_px=1719,1063\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=240,277)

2\. Далее выберите тип залива (Campaign Traffic Type). На данный момент есть выбор двух типов:&#x20;

1\) Залив на канал (Channel)&#x20;

2\)Залив на бота (Bot)&#x20;

{% hint style="warning" %}
#### Залив на бота с оптимизацией может быть выполнен двумя способами: <a href="#zaliv-na-bota-s-optimizaciei-mozhet-byt-vypolnen-dvumya-sposobami" id="zaliv-na-bota-s-optimizaciei-mozhet-byt-vypolnen-dvumya-sposobami"></a>

1\) **Лид попадает сразу на бота** - в таком случае **ивенты начнутся с contact** (момента как лид нажал /start и запустил бота)

2\) **Лид попадает сначала на преленд** - **затем на бота** - в данном случае **будут передаваться ивенты, начиная с page view и click, сontact** и тд
{% endhint %}

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/8c015a92-ffce-469d-b8d6-c6a8d59993b1/user_cropped_screenshot.jpeg?tl_px=0,284\&br_px=1694,1245\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=943,281)

3\. Выбираете Invite Bot&#x20;

Выбираете одного из ваших Telegram Bot, который будет выступать в роли принимающего заявки в канал и бота пушера.&#x20;

{% hint style="danger" %}
Бота нужно сначала активировать и затем добавить админом в канал. Если речь о заливе на канал, бот приемщик заявок должен быть ТОЛЬКО один. \
**После того как добавите бота админом в канал перейдите в раздел General, канал для выбора отобразится автоматически**
{% endhint %}

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/1f8551f9-1399-452a-9d80-87369d9ed129/user_cropped_screenshot.jpeg?tl_px=0,260\&br_px=1692,1221\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=378,282)

4. Выберите канал из списка (Сhannel)

Выбираете канал, на который будут создаваться заявки на вступление в канал и инвайт бот будет их принимать. Перед выбором канала вам необходимо добавить вашего Invite Bot в администраторы канала с правом на принятие заявок на вступление.&#x20;

{% hint style="danger" %}
ВАЖНО! В вашем канале НЕ может быть несколько ботов принимающих заявки, удалите всех других ботов, только Invite bot указанный в прошлом шаге должен быть с правами администратора на принятие заявок. Любая заявка принятая другим ботов НЕ будет учитываться в трекере, ваш бот НЕ будет писать лиду.
{% endhint %}

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/cf1941ee-809e-48a6-9bd2-36c4d28bc505/user_cropped_screenshot.jpeg?tl_px=0,428\&br_px=1719,1390\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=297,281)

7\. Выберите начальную инвайт воронку (Flow) и первое приветсвенное сообщение (Start Step)\
\
**Start Flow** - какой Flow должен быть выбран у Invite Bot для каждого пользователя, который вступит в канал и бот ему напишет.

**Start Step** - какой Step в рамках выбранного флоу должен быть активирован для каждого лида (смотрите подсказку ниже)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/865cb8f4-419d-4cf1-a55e-860ed3c3ded9/user_cropped_screenshot.jpeg?tl_px=0,437\&br_px=1709,1399\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=106,534)

8\. Для передачи ивента contact выберите DM bot&#x20;

**DM bot** - аккаунт внутри Chatterfy (среди вашего списка подключенных ботов) в который будут приходить все события и данные о каждом пользователе. Проще говоря, аккаунт в котором вы будете обрабатывать лидов.

{% hint style="info" %}
DM bot может быть тот же бот, который принимал инвайт заявку. Если нужно, выберите другого бота/личку, куда хотите чтобы подтянулась трекер информация в карточку клиента
{% endhint %}

Также вы можете выбрать Start Flow и Start Step для вашего DM bot (не обязательно)

**Start Flow для DM bot** - какой Flow должен быть выбран у Personal Bot для каждого пользователя, который напишет в личку.

**Start Step для DM bot** - какой степ в рамках Flow будет первым, когда лид напишет в аккаунт обработки

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/15b96a41-d767-47ce-bf99-87ed65cf5021/user_cropped_screenshot.jpeg?tl_px=0,439\&br_px=1719,1401\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=279,493)



***

## Подсказка

<figure><img src="../../../.gitbook/assets/CleanShot 2024-09-28 at 16.19.05@2x.png" alt=""><figcaption></figcaption></figure>

1. Выбор Flow
2. Степ
3. Степ
4. Степ



## FAQ - Часто задаваемые вопросы 📍



### 1) Использование двух ботов в канале

#### Могу ли для пушей и приема заявок в канал использовать своего бота, но добавить второго, который будет стату тянуть к вам в трекер❓

{% hint style="success" %}
&#x20;👉 Нет. Это техническое ограничение ТГ, первый может написать только тот, кто принял заявку.
{% endhint %}



### 2) Почему я не могу выбрать моего бота для авто приема заявок в канал в трекере?

{% hint style="success" %}
Должно быть ваш бот не активирован, для начала активируйте его!&#x20;
{% endhint %}

