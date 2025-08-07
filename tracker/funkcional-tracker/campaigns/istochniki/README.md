# Источники

## Для добавления сорсов пикселя перейдите в раздел трекера Campaigns - Sources



{% hint style="info" %}
После создания кампании вы получите ссылку на залив, которую затем вы вставите в пиксель
{% endhint %}

Виды источников: \
\
1\) Facebook - источник Фейсбук

{% hint style="success" %}
При выборе типа источника Facebook, вам необходимо&#x20;

* Добавить Pixel ID и Pixel Access Token
* Выбрать добавленный вами Proxy
* Для настройки ФБ изучить Маппинг ивенты (слева - наше отображение, справа - ивент, который уходит в ФБ)\
  \
  Вы получите ссылку на лендинг, которую вы затем вставите в пиксель
{% endhint %}

Маппинг ивенты (Сопоставление событий)&#x20;

* page view - в фб уйдет ивент ViewContent
* click -  в фб уйдет ивент Lead
* subscribe - в фб уйдет ивент Subscribe
* contact -  в фб уйдет ивент Contact
* registration -  в фб уйдет ивент CompleteRegistration
* sale - в фб уйдет ивент Purchase
* value - в фб передастся сумма {cost}
* currency - в фб передастся валюта {currency}

{% hint style="info" %}
Для РД создаете event = resale, выбираете куда привязать. Тогда будет отбиваться рд отдельно (можете привязывать к любому из незанятых дефолтными)
{% endhint %}



2\) Telegram - источник Телеграм канал (выбираете, если залив напрямую на канал)\


{% hint style="success" %}
При выборе типа источника Telegram, вам необходимо&#x20;

* Cоздать Телеграм канал
* Вставить инвайт ссылку вашего телеграм канала \
  \
  Для отслеживания приходящей аудитории вам необходимо использовать инвайт ссылки вашего ТГ канал.&#x20;
{% endhint %}

3\) Public Telegram - тип источника открытый Телеграм канал \


{% hint style="success" %}
У вас сгенерируется внутренний Internal invite ID, его никуда вставлять не нужно
{% endhint %}

4\) Custom - кастомный источник \


{% hint style="success" %}
* Используется если нужен лендинг без ФБ
* &#x20;Используется для тестов&#x20;
{% endhint %}

&#x20;1\. Для начала нажмите на кнопку Создать кампанию

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/e4f3e6cc-8b22-4240-b786-fa9adf8c007d/user_cropped_screenshot.jpeg?tl_px=872,0\&br_px=2592,401\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=871,168)

2\. Выберите Sources

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/c73860af-1eaa-4587-befa-b7e415c7f9ad/user_cropped_screenshot.jpeg?tl_px=0,37\&br_px=1719,998\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=331,276)

3\. Нажмите Add Source

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/a3de5640-ed1d-4d3e-8c32-a6db861df065/user_cropped_screenshot.jpeg?tl_px=0,195\&br_px=1711,1156\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=79,278)

4\. Добавьте название (Name) - внутреннее обозначение&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/30f8ecb8-18bb-4f7d-a32a-459378ba3e0c/user_cropped_screenshot.jpeg?tl_px=0,238\&br_px=1644,1199\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=184,291)

5\. Выберите Provider

{% hint style="warning" %}
**Если заливаете сразу на бота**, то нужно будет выбрать бота, и **в сорсах выбрать тип Facebook или Telegram bot**
{% endhint %}

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/c8e06ee2-eb14-4f19-b11a-a57d8faefd79/user_cropped_screenshot.jpeg?tl_px=0,403\&br_px=1687,1365\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=167,312)

6\. Вставьте Пиксель ID и пиксель access token&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/fc9049aa-7508-44a8-8469-e87c20091972/user_cropped_screenshot.jpeg?tl_px=0,187\&br_px=1719,1148\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=356,277)

7\.  Выберите добавленный вами Proxy. Proxy создается для отправки вами уникальных запросов.

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/bd4cf52e-821b-4d0a-b589-237a2a5c4cf8/user_cropped_screenshot.jpeg?tl_px=0,309\&br_px=1618,1271\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=332,345)

8\.  В разделе Mapping Events слева вы будете видеть внутренне обозначение Chatterfy и справа ивенты, которые передаются ФБ&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-13/1eb0afd6-9ab7-470b-bd2d-bbc468976935/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1577,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=274,209)

