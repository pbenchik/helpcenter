---
icon: water-arrow-up
---

# Steps Conversion

> ### Steps Conversion - это раздел для анализа воронки прохождения пользователей по шагам.

{% hint style="info" %}
С его помощью можно:

\- видеть движение пользователей внутри flow

\- находить шаги с сильной просадкой

\- сравнивать конверсию между этапами

\- тестировать эффективность разных сценариев
{% endhint %}

### Что показывает Steps Conversion:

{% hint style="info" %}
После создания воронки отображается:

* количество пользователей на каждом шаге
* конверсия между шагами
* процент потерь между этапами
* визуальная воронка
* таблица с детальной статистикой
{% endhint %}

{% hint style="info" %}
Это помогает понять, где пользователи перестают двигаться дальше и какие шаги требуют доработки.
{% endhint %}

### Как создать воронку:

{% stepper %}
{% step %}
{% hint style="info" %}
*   #### **Перейдите в Steps Conversion и нажмите Create new funnel**

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/unknown (72).jpeg" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **В поле Funnel name укажите название**

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (77).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
*   #### **В блоке Funnel задайте последовательность шагов**

    <div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (78).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* #### **При необходимости добавьте новые этапы через New step**
{% endhint %}
{% endstep %}

{% step %}
{% hint style="info" %}
* #### **Проверьте порядок шагов и нажмите Save**
{% endhint %}
{% endstep %}
{% endstepper %}

### Подробнее:

<details>

<summary>Как задавать шаги воронки</summary>

{% hint style="info" %}
Для каждого этапа указывается:

* Flow — из какого flow берётся шаг
* Step — конкретный шаг внутри flow
{% endhint %}

{% hint style="info" %}
Пример:

* Main flow → Start
* Main flow → Question
* Main flow → Offer
{% endhint %}

{% hint style="warning" %}
Шаги должны идти в логическом порядке движения пользователя.
{% endhint %}

</details>

<details>

<summary>Как читать воронку</summary>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (17).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
В визуальной части:

* каждый столбец — отдельный шаг
* уменьшение ширины показывает потери между этапами
* отображается процент перехода между шагами
{% endhint %}

{% hint style="info" %}
Ниже отображается таблица:

* Step name — название шага
* Data — количество пользователей
* % — изменение относительно предыдущего шага
{% endhint %}

</details>

<details>

<summary>Сравнение воронок</summary>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (79).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Можно сравнивать две воронки:

* Funnel — основная воронка
* Funnel 2 — вторая воронка для сравнения
{% endhint %}

{% hint style="info" %}
После этого:

* воронки отображаются рядом
* показывается разница в конверсии
* можно сравнивать эффективность разных сценариев
{% endhint %}

{% hint style="warning" %}
**Ограничения:**

* можно сравнивать не более двух воронок одновременно
* для добавления второй воронки используйте Compare funnels
{% endhint %}

</details>

<details>

<summary>Редактирование воронки</summary>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2257.png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2251 (18).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
В меню воронки доступны:

* Edit — редактирование воронки
* Open in fullscreen — открыть на весь экран
* Save image — сохранить изображение
* Delete — удалить воронку
{% endhint %}

</details>

<details>

<summary>Выбор периода</summary>

<div data-with-frame="true"><figure><img src="../../.gitbook/assets/Frame 2248 (76).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Воронка строится за выбранный период.

Доступные варианты:

* Today
* 7 days
* 14 days
* 30 days
* 90 days
{% endhint %}

{% hint style="info" %}
Также можно выбрать конкретные даты через календарь.
{% endhint %}

{% hint style="warning" %}
Выбранный период влияет на все показатели воронки и отображаемую статистику.
{% endhint %}

</details>

<details>

<summary>Важные особенности</summary>

{% hint style="warning" %}
* воронка строится на основе шагов `Step`, а не тегов
* если пользователь не дошёл до следующего шага, он не учитывается дальше
* резкое падение между шагами означает, что этап требует доработки
* чем плавнее переходы, тем лучше работает сценарий
{% endhint %}

</details>

### Где удобно использовать Steps Conversion:

{% hint style="success" %}
Steps Conversion удобно использовать, когда нужно:

* анализировать поведение пользователей
* находить слабые места в сценарии
* улучшать конверсию между шагами
* тестировать разные варианты flow
* оптимизировать путь пользователя
{% endhint %}
