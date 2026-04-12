---
icon: chart-simple-horizontal
---

# Condition

> ### Condition - это шаг, который позволяет делать разнообразные гибкие условия переходов на другие шаги.

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2260 (8).png" alt=""><figcaption></figcaption></figure></div>

**Condition** - это шаг, который позволяет разделять пользователей по условиям и направлять их по разным веткам сценария.\
Используется для:

* построения логики воронки
* сегментации пользователей
* персонализации сценариев
* обработки различных сценариев поведения
{% endhint %}

### Важно:

<details>

<summary>1. Settings (Настройки)</summary>

{% hint style="info" %}
**Title**\
Название шага.\
Используется для удобной навигации внутри flow.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>2. Conditions (Условия)</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (27).png" alt=""><figcaption></figcaption></figure></div>

Здесь настраиваются условия перехода пользователя по flow.
{% endhint %}



</details>

<details>

<summary>По каким условиям можно переводить лидов:</summary>

{% hint style="info" %}
· <mark style="color:blue;">Tags</mark> - теги

· <mark style="color:blue;">Custom Field</mark> - кастомные поля

· <mark style="color:blue;">Tracker Field</mark> - трекерные поля

· <mark style="color:blue;">Current time</mark> - текущее время. Время определяется по часовому поясу бота, которое устанавливается в его настройках, раздел Bot Settings - General;

· <mark style="color:blue;">Total Deposit</mark> - сумма депозитов лида;

· <mark style="color:blue;">Tracker Events</mark> - события. Можно сделать проверку на наличие или отсутствие того или иного события у лида;

· <mark style="color:blue;">FD Amount</mark> - сумма первого депозита;

· <mark style="color:blue;">RD Amount</mark> - сумма повторных депозитов.

*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (23).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>В данном шаге доступны следующие переменные:</summary>

{% hint style="info" %}
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (24).png" alt=""><figcaption></figcaption></figure></div>
* <mark style="color:blue;">is</mark> - есть точное совпадение;
* <mark style="color:blue;">has</mark> - если есть значение;
* <mark style="color:blue;">any</mark> - любое значение;
* <mark style="color:blue;">not</mark> - не имеет значения;
* <mark style="color:blue;">more than</mark> - больше чем;
* <mark style="color:blue;">less than</mark> - меньше чем;
* <mark style="color:blue;">range include</mark> - диапазон включает;
* <mark style="color:blue;">range exclude</mark> - диапазон исключает.
{% endhint %}



</details>

<details>

<summary>Пример на Current time:</summary>

{% hint style="info" %}
У Вас есть два обработчика, у одного из которых график работы с 12:00 до 00:00, а у другого обработчика график с 00:00 до 12:00.

Можно создать два шага с назначением обработчиков и в шаге Condition сделать два условия:

* <mark style="color:blue;">1. Для того, кто работает днем - Current time - range exclude - 00:00 - 12:00</mark>
* <mark style="color:purple;">2. Для того, кто работает ночью - Current time - range include - 00:00 - 12:00</mark>
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (25).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>Add condition</summary>

{% hint style="info" %}
Добавляет новое условие в выбранную ветку.\
В одну ветку можно добавить несколько условий.
{% endhint %}



</details>

<details>

<summary>Filter by</summary>

{% hint style="info" %}
*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (28).png" alt=""><figcaption></figcaption></figure>
* Тип данных, по которому будет происходить проверка:
* Tags - фильтрация по тегам пользователя
* Custom Field - фильтрация по кастомным полям
* Tracker Field - фильтрация по данным из трекера
* Current time - фильтрация по времени
* Total Deposit - общая сумма депозитов пользователя
* Tracker Events - параметры из трекера
* FD Amount - сумма первого депозита
* RD Amount - сумма повторных депозитов
{% endhint %}



</details>

<details>

<summary>В зависимости от выбранного типа доступны разные операторы:</summary>

{% hint style="info" %}
* is - совпадает
* has - содержит
* any - любой из
* not - не равно
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (29).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>Для числовых значений:</summary>

{% hint style="info" %}
* is - равно
* not - не равно
* more than - больше
* less than - меньше
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (30).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}



</details>

<details>

<summary>Для времени:</summary>

{% hint style="info" %}
* range include - входит в диапазон
* range exclude - вне диапазона
*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (31).png" alt=""><figcaption></figcaption></figure>
{% endhint %}



</details>

<details>

<summary>Enter value</summary>

{% hint style="info" %}
Поле для ввода значения:

Используется для:

* Custom Field
* Tracker Field
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (32).png" alt=""><figcaption></figcaption></figure></div>

В это поле вводится значение, с которым будет происходить сравнение.
{% endhint %}



</details>

<details>

<summary>Пример использования</summary>

{% hint style="info" %}
Сценарий 1: разделение по депозиту

***

**Шаг 1:** Total Deposit → more → 0 → если сумма депозитов пользователя больше 0, он будет переведён на указанный шаг

***

**Шаг 2:** Total Deposit → is → 0 → если у пользователя нет депозита, он будет переведён на указанный шаг

***

**Сценарий 1: проверка времени**

Current time → range include → 10:00–20:00\
→ перевод пользователя на указанный шаг, если текущее время находится в этом промежутке

***

**Сценарий 2: работа с тегами**

Tags → has → interested\
→ если у пользователя есть тег interested, он будет переведён на указанный шаг

***
{% endhint %}



</details>

### Важно перед началом:

{% hint style="warning" %}
Перед использованием шага необходимо понимать, какие данные вы будете использовать в условиях:\
теги, кастомные поля, события, депозиты и т.д.
{% endhint %}

### Основные возможности:

{% hint style="info" %}
С помощью Condition вы можете:

* разделять пользователей по разным веткам
* задавать несколько условий внутри одной ветки
* комбинировать различные типы данных
* строить сложную логику сценария
{% endhint %}

### Важная логика работы:

{% hint style="warning" %}
* Условия внутри одной ветки работают по принципу AND или OR
* Пользователь должен соответствовать всем условиям ветки
* Пользователь попадает только в одну ветку
* Если ни одно условие не подошло - диалог перейдет в статус manual
*

    <div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (33).png" alt=""><figcaption></figcaption></figure></div>
{% endhint %}

### Когда использовать Condition:

{% hint style="success" %}
Используйте этот шаг, когда нужно:

* разделить пользователей по разным шагам
* настроить разные сценарии
* персонализировать сообщения
* управлять логикой воронки
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
