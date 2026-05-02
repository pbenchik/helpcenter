---
icon: chart-simple-horizontal
---

# Condition

Condition позволяет разделять пользователей по условиям и направлять их по разным веткам сценария.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2260 (8).png" alt=""><figcaption></figcaption></figure></div>

### How it works

Condition используется для:

* построения логики воронки
* сегментации пользователей
* персонализации сценариев
* обработки разных сценариев поведения

### Settings

Короткие настройки шага для навигации внутри flow.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure></div>

* **Title** — название шага. Используется для удобной навигации внутри flow

### Conditions

Здесь настраиваются условия перехода пользователя по flow.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (27).png" alt=""><figcaption></figcaption></figure></div>

#### Filter types

Выберите тип данных, по которому будет выполняться проверка.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (23).png" alt=""><figcaption></figcaption></figure></div>

* **Tags** — теги
* **Custom Field** — кастомные поля
* **Tracker Field** — трекерные поля
* **Current time** — текущее время по часовому поясу бота из **Bot Settings → General**
* **Total Deposit** — сумма депозитов лида
* **Tracker Events** — события. Можно проверить наличие или отсутствие события
* **FD Amount** — сумма первого депозита
* **RD Amount** — сумма повторных депозитов

#### Filter by

Этот блок задаёт тип данных для проверки.

<figure><img src="../../../../.gitbook/assets/Frame 2248 (28).png" alt=""><figcaption></figcaption></figure>

* **Tags** — фильтрация по тегам пользователя
* **Custom Field** — фильтрация по кастомным полям
* **Tracker Field** — фильтрация по данным из трекера
* **Current time** — фильтрация по времени
* **Total Deposit** — общая сумма депозитов пользователя
* **Tracker Events** — параметры из трекера
* **FD Amount** — сумма первого депозита
* **RD Amount** — сумма повторных депозитов

#### Operators

Доступные операторы зависят от выбранного типа данных.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (24).png" alt=""><figcaption></figcaption></figure></div>

* `is` — есть точное совпадение
* `has` — если есть значение
* `any` — любое значение
* `not` — не имеет значения
* `more than` — больше чем
* `less than` — меньше чем
* `range include` — диапазон включает
* `range exclude` — диапазон исключает

**For tags and fields**

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (29).png" alt=""><figcaption></figcaption></figure></div>

* `is` — совпадает
* `has` — содержит
* `any` — любой из
* `not` — не равно

**For numeric values**

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (30).png" alt=""><figcaption></figcaption></figure></div>

* `is` — равно
* `not` — не равно
* `more than` — больше
* `less than` — меньше

**For time**

<figure><img src="../../../../.gitbook/assets/Frame 2248 (31).png" alt=""><figcaption></figcaption></figure>

* `range include` — входит в диапазон
* `range exclude` — вне диапазона

#### Enter value

Поле для ввода значения, с которым будет происходить сравнение.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (32).png" alt=""><figcaption></figcaption></figure></div>

Используется для:

* **Custom Field**
* **Tracker Field**

#### Add condition

Добавляет новое условие в выбранную ветку.

* В одну ветку можно добавить несколько условий

### Steps / Instructions

1. Добавьте шаг **Condition** в flow.
2. Откройте блок **Conditions**.
3. Выберите **Filter by**.
4. Укажите оператор.
5. Введите значение, если это нужно.
6. При необходимости нажмите **Add condition**.
7. Подключите ветку к следующему шагу.

### Examples

Ниже примеры, как использовать шаг в реальных сценариях.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (25).png" alt=""><figcaption></figcaption></figure></div>

#### Current time

У вас есть два обработчика:

* один работает с `12:00` до `00:00`
* второй работает с `00:00` до `12:00`

Можно создать два шага с назначением обработчиков и в **Condition** задать такие условия:

* для дневного обработчика — `Current time → range exclude → 00:00 → 12:00`
* для ночного обработчика — `Current time → range include → 00:00 → 12:00`

#### Other examples

* `Total Deposit → more than → 0` — если сумма депозитов пользователя больше `0`, он будет переведён на указанный шаг
* `Total Deposit → is → 0` — если у пользователя нет депозита, он будет переведён на указанный шаг
* `Current time → range include → 10:00–20:00` — переводит пользователя на указанный шаг, если текущее время находится в этом промежутке
* `Tags → has → interested` — если у пользователя есть тег `interested`, он будет переведён на указанный шаг

### Notes

Перед настройкой определите, какие данные будут участвовать в условиях.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (33).png" alt=""><figcaption></figcaption></figure></div>

* Условия внутри одной ветки работают по принципу `AND` или `OR`
* Пользователь должен соответствовать условиям ветки
* Пользователь попадает только в одну ветку
* Если ни одно условие не подошло, диалог перейдёт в статус `manual`
* Используйте шаг, когда нужно разделить пользователей по разным шагам, настроить разные сценарии, персонализировать сообщения или управлять логикой воронки

{% include "../../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
