# Как подключить AI

## Чтобы подключить AI вам необходимо создать АИ степы (этапы) во флоу&#x20;

1. **Нажмите "Create Step" (Создать степ)**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-09-30/b424982b-589a-443e-8229-18273a76c77f/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1249,762\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=359,209)

**2. Выберите тип степа - AI Reply**&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-09-30/02924198-bccf-456e-bc1d-3f58652d1fbb/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1210,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=468,393)

**3. Введите название, задайте цель и добавьте условия степа**&#x20;

* **Title** — это название блока, которое помогает ИИ лучше ориентироваться в диалоге. Старайтесь формулировать его так, чтобы оно четко отражало цель шага.&#x20;
* **Goal** — это задача, которую ИИ должен выполнить на этом шаге. В данном шаге вы закладываете основные инструкции и цель общения ИИ с клиентом.
* **Requirements** — это важный блок, который отвечает за **условия перехода клиента** по воронке.&#x20;
* **Legend -** это легенда и инструкции для вашего ИИ. Легенда поясняет кто ваш бот, чем ваш бот занимается, как он будет полезен для клиента и тд.
* **Reply Addition Info** — это дополнительные вводные для ИИ при создании финального сообщения.
* **Skip transition blocking on first run** - полезный функционал, когда нам необходимо что бы ИИ пропустил юзера в случае подходящего ответа под Requirements (условия) и не генерировал из этого блока (просто убедился что условие выполнено)

<figure><img src="../../.gitbook/assets/ai  (1).png" alt=""><figcaption></figcaption></figure>

**Push messages:**

* Global push messages - включение глобальных пушей, подробнее о настройке тут: [Global Push](../nastroiki-skripta/pushi/global-push.md).
* Step push messages - добавление пушей по заданному времени, подробнее о настройке тут: [Step Push.](../nastroiki-skripta/pushi/step-push.md)\

* **Delay ms** - задержка после выполнения степа. Во время действия задержки - все сообщения от пользователя будут проигнорированы.
* **Finish Status** - в **AI Reply** блоке используется только в специфичных ситуациях, стандартно остается пустым.

**4. Нажмите "Cохранить"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-09-30/0ed84e98-6476-461c-97b2-4101af684d7c/user_cropped_screenshot.jpeg?tl_px=0,399\&br_px=1302,1361\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=404,714)

