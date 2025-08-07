---
description: ОБНОВЛЕНИЕ ФУНКЦИОНАЛА INLINE BUTTONS
---

# Update 24.12.2024

Inline Buttons - cоздание кнопок внутри диалога, используется на степе Send Message

{% hint style="info" %}
**БЫЛО:** создание линейной воронки, добавление в кнопки только ссылок и query (вызов сообщения в поле диалога)&#x20;
{% endhint %}



{% hint style="success" %}
**СТАЛО:** Теперь от выбора кнопки будет зависить следующий шаг в конструкторе. Мы добавили два типа кнопок: Change Step и Run Step&#x20;
{% endhint %}

\
\
**Change Step** - переведет клиента на заданную вами воронку (Flow) и этап (step) после нажатия на кнопку. \
\
`Например, в сообщении будет кнопка - Ссылка на регистрацию, клиент на нее нажмет и автоматически перейдет на созданный вами внутри воронки флоу Регистрации и степ Ссылка на регистрацию`\
\
**Run Step** - кнопка с помощью которой можно вызывать send message степ не переключаясь на него\
\
`Например кнопка Info, которая вызывает степ с какой-то базовой информацией, отправит ее, но на сам степ Info клиента не переведет`\
\
**Подробное описание всех типов кнопок Inline Buttons:**&#x20;

1\) **URL** - кнопка, которая переведет клиента по добавленной вами ссылке. Пример ссылки: hhtps://register.com

2\) **WebApp** - кнопка, которая откроет сайт прямо в Телеграмме \
\
3\) **Query** - кнопка, при нажатии на которую вставит добавленный текст в поле отправки сообщения

4\) **Сhange Step** - кнопка перевода клиента на заданный этап воронки

5\) **Run Step** -  кнопка с помощью которой можно вызывать send message степ не переключаясь на него.

## Инструкция по добавлению нового типа кнопок&#x20;

Добавление Change Step

1\. Откройте конструктор и перейдите на степ типа Send Message

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/09e1092c-20f3-44d7-b009-5b475474f9c5/ascreenshot.jpeg?tl_px=428,220\&br_px=2148,1181\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,277)

2\. Нажмите на добавление сообщения поле Manual Messages&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/b4dd7861-c65b-45a0-82da-9c6061f9f0ce/user_cropped_screenshot.jpeg?tl_px=853,0\&br_px=2573,961\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,112)

3\. Нажмите добавить сообщение (Add Message)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/133133f5-bd6f-49a9-9ecd-0476c6e0c8e2/user_cropped_screenshot.jpeg?tl_px=678,455\&br_px=2398,1417\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,458)

4\. Нажмите на  добавление типа сообщения

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/3529e77d-7af7-4bd5-a98d-20379b1d7253/user_cropped_screenshot.jpeg?tl_px=694,451\&br_px=2414,1413\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,336)

5\. Выберите тип Inline Buttons

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/d256e407-84ca-49e0-86b2-61215d106fce/user_cropped_screenshot.jpeg?tl_px=650,416\&br_px=2370,1377\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,276)

6\. Нажмите добавить новую кнопку (add new button)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/615ac599-284a-46a2-aa77-4d7fb4e8df1d/user_cropped_screenshot.jpeg?tl_px=703,434\&br_px=2423,1395\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,277)

7\. Добавьте описание кнопки (caption) и затем на саму кнопку&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/74d106c9-c284-408d-8ac5-7115577f6d2e/user_cropped_screenshot.jpeg?tl_px=936,447\&br_px=2656,1409\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,290)

8\. При выборе типа кнопки нажмите на Change Step

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/0c669cb2-d1e5-4c86-b6c5-690374ed2893/user_cropped_screenshot.jpeg?tl_px=712,418\&br_px=2432,1380\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,313)

9\. Затем выберите Flow (воронку) и Step (этап) воронку на который хотите перевести клиента при нажатии на кнопку&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/0ec6b588-7094-4c45-8c44-b22db25c0f58/user_cropped_screenshot.jpeg?tl_px=668,347\&br_px=2388,1308\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,276)

10\. Нажмите сохранить

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/edfab79c-c80e-49c5-a110-848d2d80c8e8/user_cropped_screenshot.jpeg?tl_px=875,445\&br_px=2595,1406\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,277)

Теперь при нажатии на вашу кнопку клиент автоматически перейдет на воронку Main Flow и степ Registration info&#x20;





### Инструкция по добавлению Run Step



1\. Перейдите на степ Send Message, нажмите добавить сообщение и выберите тип Inline buttons. Затем нажмите на Add new button (Добавить новую кнопку)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/486e7334-0dd1-4164-b6ae-b2f0d7c59f93/user_cropped_screenshot.jpeg?tl_px=1053,336\&br_px=2773,1297\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=531,277)

2\. Нажмите на созданную кнопку и откройте ее&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/9f24a5b8-f383-4047-95d2-d0735f7a76bf/user_cropped_screenshot.jpeg?tl_px=1076,403\&br_px=2796,1364\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=542,276)

3\. Задайте название кнопки (оно будет отображаться для клиента). В Button type (типе кнопок) выберите Run Step

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/2bbaf65c-3318-4a4b-9495-d46e714ded45/user_cropped_screenshot.jpeg?tl_px=739,442\&br_px=2459,1404\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=523,369)

4\. Выбираем флоу (воронку) и степ (этап воронки)

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/83570806-8c14-4b51-9df0-706378ea7303/user_cropped_screenshot.jpeg?tl_px=724,436\&br_px=2444,1398\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,287)

5. В данном случае выбираем воронку Main Flow и Run Step - Retention



![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/7c02fd48-f6c2-4719-a4a3-714ae896f038/user_cropped_screenshot.jpeg?tl_px=849,443\&br_px=2569,1405\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,362)

8\. Нажмите сохранить

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/9e9c3101-f6c4-45d9-90bb-792c02bd8b4e/user_cropped_screenshot.jpeg?tl_px=856,436\&br_px=2576,1398\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,537)



{% hint style="success" %}
**Разбор примера:** Клиент находится на степе **About work,** как только он нажмет на созданную кнопку Run Step ему **автоматически отправится сообщение** **со степа Retention, но клиент не перейдет на него.** \
\
Дальше продолжится следующий степ воронки **Ready to start?** после About work&#x20;
{% endhint %}



![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-12-25/027d6bbe-6f24-4471-ae69-bcb3d85280b1/user_cropped_screenshot.jpeg?tl_px=482,449\&br_px=2202,1411\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=524,319)
