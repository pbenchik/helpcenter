# Update 20.12.2024

## Добавление кастомных переменных в боте

\
Теперь в настройках бота (Bot Settings) появилась возможность создавать кастомные переменные, которые можно использовать через макросы.



{% hint style="info" %}
**БЫЛО:**  Раньше, при импорте флоу из одного бота или лички в другую, приходилось тратить уйму времени, вручную менять ссылки в каждом шаге, рисковать ошибками и путаницей в параметрах. Это часто приводило к сбоям в работе и излишним затратам времени.
{% endhint %}



{% hint style="success" %}
**СТАЛО: Теперь достаточно всего лишь обновить саму переменную и больше не придется все ссылки вручную менять. Автоматизируй рутинные процесы, чтобы больше не тратить время впустую!!! Мы рады облегчить вам жизнь :)**&#x20;
{% endhint %}

### В макрос Variables ты можешь подставлять абсолютно любую информацию из карточки клиента, а именно кастомные филды, трекер дату и любую информацию о клиенте&#x20;

### Хотите подставлять ID клиента в сообщениях?&#x20;

Рассмотрим кейс добавления переменных из кастомных филдов в Bot variables



*   **Для начала ты записываете ID клиента в кастомные филды.** \
    \
    Следуйте инструкции как это сделать:&#x20;

    [Инструкция по записи кастомной информации о клиенте](../../crm-dlya-obsheniya/funkcional-crm/stranica-chatov/kastomnye-polya.md)
* **Далее перейдите в Bot Settings - Bot Variables**. **В поле ''Name" укажите кастомную переменную.**&#x20;

{% hint style="info" %}
**Например, variables. trader\_id**
{% endhint %}

* **В поле Value вставьте само значение переменной**

{% hint style="warning" %}
**Например, \{{fields.trader\_id\}}**
{% endhint %}

Чтобы подставить ID клиента на степе или же внутри диалогового окна, используйте **\{{variables.trader\_id\}}**



### Хотите подставлять ссылку на регистрацию в сообщениях?

1. Перейдите в раздел Bot Settings&#x20;
2. Пролистайте вниз, найдите поле Bot variables&#x20;
3. В поле ''Name" укажите кастомную переменную, например variables.regLink&#x20;
4. В поле Value вставьте само значение переменной, например [https://pp.com?clickid=\{{tracker.clickid\}}](https://pp.com/?clickid=\{{tracker.clickid\}})

{% hint style="success" %}
Вместо того, чтобы постоянно вставлять ссылку из примера выше в степах или сообщениях, можно использовать просто \{{variables.regLink\}}
{% endhint %}

## Инструкция по добавлению кастомных переменных (на примере ссылки регистрации)



1\. Перейдите в раздел Bot Settings&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-20/48da9f30-619e-4adb-8e64-9d4dc4adac6b/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1459,603\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=107,110)

2\. Пролистайте вниз, найдите поле Bot variables

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-20/dc619adc-8f96-4e00-bb80-623d01f09dd0/user_cropped_screenshot.jpeg?tl_px=749,475\&br_px=2469,1437\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,358)

3\. В поле ''Name" укажите кастомную переменную, например variables.regLink&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-20/4c61b314-6d1b-4bf7-9813-aca4446039fd/user_cropped_screenshot.jpeg?tl_px=759,471\&br_px=2479,1433\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=523,397)

5. В поле Value вставьте само значение переменной, например [https://pp.com?clickid=\{{tracker.clickid\}}](https://pp.com/?clickid=\{{tracker.clickid\}})

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-20/d651087d-1f01-4ebc-9771-dd200e339cd0/user_cropped_screenshot.jpeg?tl_px=1049,471\&br_px=2769,1433\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=553,418)

6\. Нажмите сохранить

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-20/4a2f306a-f5da-4fb8-af60-cd2f29499c72/user_cropped_screenshot.jpeg?tl_px=0,398\&br_px=1719,1360\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=222,528)

## Перейдите в страницу чатов и откройте диалоговое окно



1\. Проверьте настроенный вами параметр, вставив макрос в поле отправки сообщения

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-20/c3c40389-7e5e-497d-b4ff-ee215867b088/user_cropped_screenshot.jpeg?tl_px=515,462\&br_px=2235,1424\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,550)

2. Настроив все правильно, ваш макрос автоматически отправится как заданная переменная (в данном примере это ссылка на регистрацию)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-20/c86d349b-3f2a-460a-8fe6-8d8eab849f0e/user_cropped_screenshot.jpeg?tl_px=784,454\&br_px=2504,1416\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,459)
