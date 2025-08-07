# Update 09.11.2024

### Теперь вы можете легко привязать свой собственный лендинг – всего за пару кликов!



{% hint style="info" %}
**Было:** Возможен был доступ только к добавлению стандартного лендинга Telegram.
{% endhint %}



{% hint style="success" %}
**Стало:** Можно добавить как кастомный лендинг с вашей графикой, так и стандартный лендинг Telegram.
{% endhint %}



## Инструкция по добавлению 👇



1\. Перейдите в раздел Трекера&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-11-10/6d623afa-1af1-4aa1-8fbc-a6c89ca282a5/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1719,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=500,9)

2\. Нажмите на Landings&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-11-10/26b20f76-d8b0-4ba3-909f-1f37f0ba3856/user_cropped_screenshot.jpeg?tl_px=136,0\&br_px=1856,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,78)

3\. Нажмите на кнопку справа сверху "Create Landing" (Создать лендинг)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-11-10/54137247-25d8-45eb-9d43-67a5f71853a0/user_cropped_screenshot.jpeg?tl_px=930,0\&br_px=2650,779\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=833,262)

4\. Внутри создания лендинга в поле **Name** введите название вашего лендинга **(внутреннее обозначение)**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-11-10/9c20ecc5-16b0-4689-b353-95cbae9086ae/user_cropped_screenshot.jpeg?tl_px=0,262\&br_px=1719,1223\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=267,277)

5\. Перейдите в раздел Page Settings и выберите Custom

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-11-10/89026335-6e7a-4af1-acd1-586fb71d9aab/user_cropped_screenshot.jpeg?tl_px=0,198\&br_px=1719,1159\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=463,277)

6\. Нажмите на Upload Archive и загрузите Архив zip



{% hint style="warning" %}
Для работы с кастомными лендингами необходимо загрузить архив в формате ZIP, содержащий файл **index.html !!!**
{% endhint %}



{% hint style="danger" %}
Необходимо добавить кнопку для перехода в Telegram, указав атрибут **"**&#x74;racke&#x72;**"** у соответствующего элемента. И таких элементов может быть сколько угодно, а именно теперь можно хендлить любое количество кнопок
{% endhint %}

Пример html элемента:&#x20;

```
<a tracker>test</a>

пустой атрибут tracker на любой элемент
```

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-11-10/35af05a8-3f4f-4305-a3fa-e0bd4d594528/user_cropped_screenshot.jpeg?tl_px=0,287\&br_px=1719,1248\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=265,277)



## FAQ - Часто задаваемые вопросы 📍



### 1) Как настроить обработку ссылки ботом?



Если вы вручную создали инвайт-ссылку в канал и вставили её в лендинг, чтобы бот обработал эту ссылку, нужно создать источник в кампании с типом _telegram_ и указать эту инвайт-ссылку.

{% hint style="success" %}
Чтобы бот обработал ссылку, укажите тип источника (Source)  как _Telegram_ в кампании и передайте эту ссылку.
{% endhint %}

{% hint style="success" %}
Если тип источника (Source)  _Facebook,_ то инвайт-ссылки создаются с нашей стороны.&#x20;
{% endhint %}



### 2) Есть ли возможность добавления мультикнопок?&#x20;



{% hint style="warning" %}
На данный момент апдейт еще не вышел, подождите пока мы реализуем поддержку мультикнопок 😉
{% endhint %}
