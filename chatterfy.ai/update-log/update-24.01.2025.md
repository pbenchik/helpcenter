# Update 24.01.2025

### Изменения в структуре статистики&#x20;



Мы внесли изменения в отображение данных в разделе статистики внутри бота/лички, представив новую систему группировки через меню папок. Это обновление делает анализ данных более удобным и структурированным, позволяя вам быстрее находить необходимую информацию.

{% file src="../../.gitbook/assets/Chatterfy Обновления 24.01.2025.MOV" %}

Теперь статистика разделена на несколько ключевых категорий:

**1)  Чаты** – отображает общую динамику диалогов, включая:&#x20;

* Общее количество чатов
* &#x20;Чаты за текущий день&#x20;
* Чаты за неделю (понедельник-воскресенье)&#x20;
* &#x20;Чаты за месяц

<figure><img src="../../.gitbook/assets/image (333).png" alt=""><figcaption></figcaption></figure>

**2)  Конверсия по степам** – инструмент для создания конверсионных воронок на основе этапов (степов), на которых находятся клиенты. Позволяет детально отслеживать эффективность каждого этапа взаимодействия.

<figure><img src="../../.gitbook/assets/image (334).png" alt=""><figcaption></figcaption></figure>

**3)  Конверсия по тегам** – создание конверсионных воронок на основе тегов, которые назначаются клиентам автоматически в процессе прохождения воронки или вручную.



<figure><img src="../../.gitbook/assets/image (335).png" alt=""><figcaption></figcaption></figure>



**4) Биллинг** – раздел, содержащий информацию о расходах, включая:&#x20;

* Статистику использования
* Среднюю стоимость чата за всё время&#x20;
* &#x20;Среднюю стоимость новых чатов
* &#x20;Итоговый биллинг за месяц

<figure><img src="../../.gitbook/assets/image (337).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**БЫЛО:** Вся статистика отображалась на одной общей странице
{% endhint %}

{% hint style="success" %}
**СТАЛО:** Вся информация теперь структурирована по папкам (сабгруппам), что облегчает анализ данных. Добавлена возможность создания конверсионных воронок по степам.
{% endhint %}



### Создание воронок конверсии по степам



Теперь можно детально анализировать, на каких конкретных шагах пользователи сталкиваются с трудностями и где наблюдаются основные потери в конверсии.



Какая разница между "Конверсией по тегам" и "Конверсией по степам"?

{% hint style="info" %}
**Конверсия по тегам** – используется для анализа общей конверсии, но не позволяет детально изучить просадку на отдельных этапах.&#x20;
{% endhint %}

{% hint style="warning" %}
**Конверсия по степам** – даёт возможность глубже проанализировать, как работают конкретные этапы воронки, выявляя проблемные зоны.
{% endhint %}

\
При настройке конверсионного графика необходимо заполнить три ключевых поля:

1. **Name** – название этапа конверсии&#x20;
2. **From Step** – начальный этап, с которого начинается анализ конверсии&#x20;
3. **To Step** – конечный этап, до которого ведётся расчёт



> ❗️ **ВАЖНО**❗️**Если указываются поля "From Step" и "To Step"**, **убедитесь, что между этими степами есть прямой переход.**&#x20;
>
> Также одно из полей "From Step" или "To Step" может остаться незаполненным.

Вы, используя конверсию по степам, будете анализировать переходы между степами.\
\
Пример перехода:

<figure><img src="broken-reference" alt=""><figcaption><p><br> (это может быть просто переход на какой-то степ или просто выход из какого-то степа)</p></figcaption></figure>



{% hint style="info" %}
Если у выбранных вами степов НЕ БЫЛО прямого перехода между начальным степом и конечным, то в аналитике будет 0
{% endhint %}



1. Перейдите в раздел Конверсия по степам. Нажмить Создать

<figure><img src="../../.gitbook/assets/image (339).png" alt=""><figcaption></figcaption></figure>

2. Введите название воронки

**Name** – название этапа конверсии&#x20;

**From Step** – начальный степ, с которого начинается анализ конверсии&#x20;

**To Step** – конечный этап, до которого ведётся расчёт

{% hint style="info" %}
Также одно из полей "From Step" или "To Step" может остаться незаполненным.
{% endhint %}

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2025-01-23/53629ddf-8922-44d9-b559-4fa7c50ef5f6/user_cropped_screenshot.jpeg?tl_px=14,0\&br_px=2766,1432\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=574,174)

4\. Нажмите на From Step - начальный cтеп, с которого начинается анализ конверсии&#x20;

{% hint style="info" %}
Одно из полей "From Step" или "To Step" может остаться незаполненным.
{% endhint %}

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2025-01-23/1fae4135-f687-48f0-b9ca-9c5c7d254626/user_cropped_screenshot.jpeg?tl_px=24,0\&br_px=2776,1308\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=762,249)

5\. Выберите To step - конечный этап, до которого ведётся расчёт.

{% hint style="info" %}
Одно из полей "From Step" или "To Step" может остаться незаполненным.
{% endhint %}

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2025-01-23/bdcdf6a9-9205-4a2b-b732-f660a57d0328/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=2716,1366\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=907,215)

6\. Вы также можете создавать АБ тесты воронок и сравнивать конверсии&#x20;

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2025-01-23/5e3370ea-a420-4661-bce0-ec8ecea18837/user_cropped_screenshot.jpeg?tl_px=41,0\&br_px=2794,1410\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=559,382)

