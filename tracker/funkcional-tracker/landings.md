# Landings

## Для создания лендинга для начала откройте основное меню и перейдите в раздел трекера&#x20;



1\. Перейдите в раздел трекера&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-10-16/54ef55d6-020a-4889-9a8c-8b824a301d41/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1719,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=520,12)

2\. Нажмите на Landings (Лендинги)&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-10-16/f7323c1b-7aeb-4394-9afb-cb1de2f6eb21/user_cropped_screenshot.jpeg?tl_px=130,0\&br_px=1850,876\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,74)

3\. Для создания нового лендинга нажмите "Create Landings" (Создать лендинг)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-10-16/c384e700-79c8-4b17-9998-dd9c33efc4f6/user_cropped_screenshot.jpeg?tl_px=746,0\&br_px=2466,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=926,225)

4\. В разделе General (общая настройка), задайте:\


* Name = (внутреннее обозначение)
* Description = описание, которое будет отображаться&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-10-16/5aa04d23-0a14-4853-9575-7a8515ca11f6/user_cropped_screenshot.jpeg?tl_px=0,22\&br_px=1719,983\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=150,276)

5\. Для настройки страницы перейдите в Page Settings&#x20;

* Title = название&#x20;
* Members text = условное обозначение (например, слово "subscribers")
* Members count = количество участников&#x20;
* Download text = авто кнопка в верхнем углу экрана&#x20;
* Open button text = текст кнопки перехода

<figure><img src="../../.gitbook/assets/image (266).png" alt=""><figcaption></figcaption></figure>

6\.  В Custom Code вы можете использовать:

* CSS = добавление блоков и передвижение кнопок&#x20;
* JS = добавление динамики, внедрение трекера на страницу (просмотр промежуточных действий пользователя на странице)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-10-16/23d76a6d-ccff-432f-91a9-3759fae4d688/user_cropped_screenshot.jpeg?tl_px=0,7\&br_px=1719,968\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=428,277)

Затем нажмите "Save" (Сохранить)  ✅



### Для превью готового лендинга вернитесь в раздел Page Settings (Настроек страницы)

<figure><img src="../../.gitbook/assets/Screenshot 2025-03-25 at 02.02.03.png" alt=""><figcaption></figcaption></figure>

### Добавление кастомного лендинга&#x20;



Теперь вы можете легко привязать свой собственный лендинг – всего за пару кликов!

1\. Перейдите в раздел Трекера&#x20;

<figure><img src="../../.gitbook/assets/image (246).png" alt=""><figcaption></figcaption></figure>

2\. Нажмите на Landings&#x20;

<figure><img src="../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3\. Нажмите на кнопку справа сверху "Create Landing" (Создать лендинг)

<figure><img src="../../.gitbook/assets/image (248).png" alt=""><figcaption></figcaption></figure>

4\. Внутри создания лендинга в поле **Name** введите название вашего лендинга **(внутреннее обозначение)**



<figure><img src="../../.gitbook/assets/image (249).png" alt=""><figcaption></figcaption></figure>

5\. Перейдите в раздел Page Settings и выберите Custom

<figure><img src="../../.gitbook/assets/image (250).png" alt=""><figcaption></figcaption></figure>

6\. Нажмите на Upload Archive и **загрузите Архив zip**



{% hint style="warning" %}
Для работы с кастомными лендингами необходимо загрузить архив в формате ZIP, содержащий файл **index.html !!!**
{% endhint %}

{% hint style="info" %}
Необходимо добавить кнопку для перехода в Telegram, указав атрибут **tracker** у соответствующего элемента.&#x20;

И таких элементов может быть сколько угодно, а именно теперь можно хендлить любое количество кнопок
{% endhint %}

```
<a tracker>test</a>
```

<figure><img src="../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>



## FAQ - Часто задаваемые вопросы 📍



### 1) Как настроить обработку ссылки ботом?



{% hint style="info" %}
Если вы вручную создали инвайт-ссылку в канал и вставили её в лендинг, чтобы бот обработал эту ссылку, нужно создать источник в кампании с типом _telegram_ и указать эту инвайт-ссылку.
{% endhint %}

{% hint style="warning" %}
Если тип источника (Source)  _Facebook,_ то инвайт-ссылки создаются с нашей стороны.&#x20;
{% endhint %}



### 2) Есть ли возможность добавления мультикнопок?&#x20;



{% hint style="warning" %}
На данный момент апдейт еще не вышел, подождите пока мы реализуем поддержку мультикнопок 😉
{% endhint %}
