---
hidden: true
---

# 1win Postbacks

Настройка постбеков 1win нужна для автоматического получения данных о регистрации, депозитах и повторных депозитах, включая суммы операций.



1\. В первую очередь вам необходимо перейти в раздел трекера. Нажмите на значок Facebook

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-02/416a7f41-ddb0-4a69-82a7-8a1a29cf2cf8/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1719,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=499,14)

2\. Внутри трекера выберите раздел Postbacks и нажмите на него&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-02/0140dc96-3bc4-4f13-813b-4eeba1aacdb7/user_cropped_screenshot.jpeg?tl_px=541,0\&br_px=2261,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,95)

3\. Затем нажмите "Create Postback"

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-02/7098f520-dc64-470d-945b-42a3c1d7e34a/user_cropped_screenshot.jpeg?tl_px=1047,211\&br_px=2767,1172\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=804,277)

4\. Далее введите информацию создаваемого постбэка

* Name - внутреннее обозначение (Например: 1Win)
* Affiliate Network - на данный момент внутри платформы представлены 2 партнерки 1Win и Binomo. Если ваша партнерка не представлена, то просто выберите Custom&#x20;
* Campaign - если выбрать, то постбеки будут уникальные только для определенного выбранного кампейна \
  Лучше не выбирать, чтобы постбэки для всех кампейнов были общие

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-02/29be82a1-f0b0-4b07-8b8c-0fa8bc298d9e/user_cropped_screenshot.jpeg?tl_px=390,0\&br_px=2110,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,205)

5\. Нажмите создать постбеки&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-02/6d2535fd-c860-4f3b-ac81-b24c64970fe3/user_cropped_screenshot.jpeg?tl_px=82,359\&br_px=1801,1321\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,282)

11\. После того как вы создадите постбеки внутри Chatterfy вы получите 3 ссылки:



* **Registration** - ссылка для постбэка регистрации
* **First Deposit** - (ФД) ссылка для постбэка первого депозита&#x20;
* **Deposit** - (РД) ссылка для постбэка повторного редепозита



![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-02/81939d86-48c9-4ea9-b62b-8e1db7443255/user_cropped_screenshot.jpeg?tl_px=990,438\&br_px=2710,1400\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=653,285)

Затем заберите эти 3 ссылки к себе в партнерку и активируйте их. После активации вам нужно настроить передачу кликайди клиента в продукт и вернуть назад. \
\
Рассмотрим как это сделать на примере, ссылки регистрации:\
\
1\) Вы клиенту выдаете ссылку на регистрацию,  в которую подставите сабы вашей партнерки\


{% hint style="warning" %}
У 1Win нет поля кликайди, обычно подставляется sub1, sub2, sub3 и тд
{% endhint %}

**Ваша ссылка на регистрацию будет выглядеть вот так (домен замените на свой):**\
&#x20;[https://1wgbch.top/casino/play/aviator?open=register\&sub1=\{{tracker.clickid\}}](https://1wgbch.top/casino/play/aviator?open=register\&sub1=\{{chat.tracker.clickid\}})



2\) Постбеки, созданные внутри Chatterfy, вам необходимо вставить внутри партнерки в соответствующие поля (Регистрация/Первый депозит/Повторный депозит)\


<figure><img src="../../.gitbook/assets/image (221).png" alt=""><figcaption></figcaption></figure>



3\) Благодаря этому, кликайди всех клиентов после регистрации запишется в поле sub1. После выполнения действия 1Win сообщит нам, что клиент с этим кликайди выполнил то или иное действие.

