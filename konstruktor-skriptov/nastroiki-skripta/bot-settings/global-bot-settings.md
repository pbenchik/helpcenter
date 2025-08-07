# Global bot settings

**Bot Settings** — это внутренние настройки и описание бота, которые систематизируют работу ИИ. В них можно добавить теги, настроить уровень креативности ответов ИИ, установить время задержки для отправки сообщений, привязать Telegram каналы и тд.&#x20;

{% hint style="success" %}
Все нужно писать на английском языке: ai settings (global, goal, user restriction, requirement), промпты также на английском.
{% endhint %}

## 1. Нажмите на значок ⚙️ для перехода в Global Bot Settings

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2024-09-29/818dffc6-d793-4eb2-927b-4f9bd7744a33/user_cropped_screenshot.jpeg?tl_px=0,0\&br_px=1719,525\&force_format=jpeg\&q=100\&width=1120.0\&wat=1\&wat_opacity=1\&wat_gravity=northwest\&wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/EAB308_standard.png\&wat_pad=84,76)

## 2.  Нажмите на кнопку "Activate", чтобы активировать бота.

<figure><img src="../../../.gitbook/assets/user_cropped_screenshot (5).jpeg" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Bot Tags** - теги бота (не диалогов). Иcпользуется исключительно для тегирования ботов  для их поиска/фильтрации
{% endhint %}

## 3. **Delays** - настройка основной задержки перед ответом юзеру.

<figure><img src="../../../.gitbook/assets/Screenshot 2024-09-30 at 02.59.56.png" alt=""><figcaption></figcaption></figure>

* **Response time for the lead** - это время, которое пройдет после последнего сообщения от пользователя до запуска степа
* **AI Reply answer speed** - это задержка для Ai Reply, от момента получения последнего сообщения до отправки ответа пользователю (т.е. Response time for the lead + задержка на работу ai)

{% hint style="info" %}
например, в Response time for the lead стоит 1 минута, а на AI Reply answer speed 1 минута 20 секунд, то это Response time for the lead + 20 секунд
{% endhint %}



* &#x20;**Send message answer** - это задержка для Send Message, от момента получения последнего сообщения до отправки ответа пользователю
* **Typing speed** - скорость набота текста ИИ

## 4. **Notications -** позволяет добавить функционал нотификаций для групп в TelegramComment

Подробнее: [Нотификации](notifikacii.md)

<figure><img src="../../../.gitbook/assets/noti.png" alt=""><figcaption></figcaption></figure>

## 5. **Webhooks & API**  - позволяет использовать вебхуки для внешних сервисов и выполнять определенные дейсвтия в конструкторе.

Подробнее: Входящие запросы (Postbacks)

<figure><img src="../../../.gitbook/assets/webhooks .png" alt=""><figcaption></figcaption></figure>

## 6. **Integrations** - функционал для интеграции со сторонними сервисами

Пример интеграции:&#x20;

<figure><img src="../../../.gitbook/assets/integrations.png" alt=""><figcaption></figcaption></figure>

## 7. **Custom Fields**&#x20;

**Custom Fields** позволяют вручную создавать кастомные (доп.) поля для переменных или других деталей диалога (например, UserID, ClickID, Deposit\_amount, комментарии и т.д.)

{% hint style="success" %}
Эти поля могут заполняться как вручную, так и автоматически, отображаться на правой панели диалога и использоваться для работы с лидами и аналитики.
{% endhint %}

<figure><img src="../../../.gitbook/assets/custome field .png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Для создания поля требуется:

* Уникальный ключ поля (любое уникальное название)
* Внутреннее имя поля которое будет отображаться всем сотрудникам
* Тип поля: Текст, Длинный текст, Ссылка, Номер
{% endhint %}

## 8. **Bot Pit Stop Settings** - условия перехода чата в мануал.

Включите ползунки, при получении которых, ваш диалог автоматически будет переводиться в мануал. Например, клиент отправил вам фото/видео/ аудио/ документ ➡️ диалог перейдет в мануал.

<figure><img src="../../../.gitbook/assets/bot pit stop.png" alt=""><figcaption></figcaption></figure>

## 9. **Bot tags** - теги воронки

{% hint style="success" %}
**Bot tags** — это ключевой инструмент для контроля воронки. Он позволяет создавать и редактировать теги для скриптов и этапов воронки. Также можно настроить автоматическое присвоение тегов диалогам на разных стадиях и строить отчеты на их основе.
{% endhint %}

<figure><img src="../../../.gitbook/assets/bot tag.png" alt=""><figcaption></figcaption></figure>

## 10. Assignment Managers



1. Откройте **Bot Settings** и перейдите в раздел **Assignment managers.**

{% hint style="success" %}
**Show only assigned chats for operator** - первая настройка активирует фильтрацию конкретных чатов только для присвоенного оператора
{% endhint %}



{% hint style="info" %}
**Hide not assign chats for operator** - вторая настройка дополнительно скрывает чаты без ассайна
{% endhint %}

