---
icon: hashtag
---

# Change tag

> ### Change Tag - это шаг для добавления или удаления тегов у диалога.

Здесь можно менять теги пользователя после прохождения текущего шага.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2260 (3).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Change Tag используют для:

* сегментации пользователей
* построения логики воронки
* дальнейшей фильтрации и аналитики

Теги помогают передавать состояние пользователя между шагами сценария.
{% endhint %}

{% hint style="warning" %}
Перед использованием шага теги нужно заранее создать в разделе **Bot Settings → Tags**.

Без этого выбрать нужный тег в настройках шага не получится.
{% endhint %}

{% hint style="success" %}
**Assign - присвоить тег**

*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (60).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

{% hint style="danger" %}
**Remove - удалить тег**

*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (61).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

### Как работает Change Tag:

{% hint style="info" %}
После выполнения шага система сразу применяет выбранное действие к тегу.

Вы можете:

* присвоить тег пользователю
* удалить тег у пользователя
* комбинировать несколько действий в одном шаге
{% endhint %}

### Важно:

<details>

<summary>1. Settings (Настройки)</summary>

{% hint style="info" %}
В блоке **Settings** задаются общие параметры шага:

* **Title** — название шага
* **Delay** — задержка перед выполнением действия
* **Finish Status** — статус диалога после шага
* **Hide keyboard** — скрывает клавиатуру из предыдущего шага
* **Is start step of flow** — делает шаг стартовым
* **Skip the transition to next step** — отключает автоматический переход дальше
*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (62).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

{% hint style="info" %}
Во время `Delay`:

* сообщения пользователя игнорируются
* действие с тегом не выполняется
{% endhint %}

{% hint style="warning" %}
Если используется статус `waiting`, можно включить **Skip the transition to next step**.

Тогда шаг не переключится автоматически и система останется в текущем состоянии.
{% endhint %}

</details>

<details>

<summary>2. Tags (Работа с тегами)</summary>

{% hint style="info" %}
В этом блоке настраиваются действия с тегами.

Основные поля:

* **Action** — выбрать `Assign` или `Remove`
* **Choose tag** — выбрать тег из списка
* **Add tag** — добавить ещё одно действие в этом же шаге
*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (63).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

{% hint style="info" %}
Один шаг может выполнять сразу несколько действий.

Например:

* присвоить один тег
* удалить другой

Это удобно, если нужно быстро обновить состояние пользователя в воронке.

*

    <figure><img src="../../../../.gitbook/assets/Frame 2248 (64).png" alt=""><figcaption></figcaption></figure>
{% endhint %}

</details>

### Важная логика работы:

{% hint style="warning" %}
* Теги применяются сразу после выполнения шага
* Один шаг может изменять несколько тегов одновременно
* Теги часто используются в `Condition`
* Через теги удобно строить сегментацию и дальнейшие переходы
{% endhint %}

### Пример использования:

{% hint style="info" %}
Сценарий: пользователь подтвердил интерес.

* `Assign` → `interested`
* `Remove` → `not_interested`

Так вы сразу обновляете его состояние в логике воронки.
{% endhint %}

### Когда использовать Change Tag:

{% hint style="success" %}
Используйте этот шаг, когда нужно:

* сегментировать пользователей
* помечать этапы воронки
* передавать данные в логику сценария
* управлять дальнейшими переходами
{% endhint %}

{% include "../../../../.gitbook/includes/start-i-obzoro-produktearkhi....md" %}
