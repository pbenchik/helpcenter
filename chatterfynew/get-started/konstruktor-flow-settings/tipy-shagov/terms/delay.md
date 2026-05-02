---
icon: clock
---

# Delay

Delay выполняет следующий переход в конкретное время.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (17).png" alt=""><figcaption></figcaption></figure></div>

### How it works

Шаг запускает следующий переход по времени, которое вы задаёте вручную.

* время рассчитывается по таймзоне бота
* сценарий ждёт до указанного времени
* после этого происходит переход к следующему шагу

### Use cases

Delay подходит для:

* запуска действий в конкретное время
* построения логики flow по расписанию
* управления таймингом сценария
* отложенного перехода к следующему шагу

### Settings

Базовые настройки шага.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (19).png" alt=""><figcaption></figcaption></figure></div>

* **Title** — название шага. Используется для удобной навигации внутри flow
* **Finish Status** — статус диалога после выполнения шага:
  * `nothing` — переход к следующему шагу
  * `auto` — автоматическое продолжение диалога
  * `waiting` — ожидание ответа пользователя
  * `manual` — перевод в ручной режим
  * `blocked` — блокировка диалога
  * `finished` — завершение диалога
* **Hide keyboard** — скрывает клавиатуру из предыдущего шага
* **Is start step of flow** — отмечает шаг как стартовый
* **Skip the transition to next step** — отключает автоматический переход на следующий шаг. Обычно используется вместе со статусом `waiting`

Если **Skip the transition to next step** включён:

* шаг не переключится автоматически
* система останется на текущем шаге
* система будет ждать ответ пользователя

### Delay

Здесь задаётся точное время выполнения шага.

<figure><img src="../../../../.gitbook/assets/Frame 2248 (20).png" alt=""><figcaption></figcaption></figure>

* указывается конкретное время, а не задержка от предыдущего шага
* формат значения — `часы : минуты`

### Steps / Instructions

1. Добавьте шаг **Delay** в flow.
2. Откройте блок **Delay**.
3. Укажите точное время выполнения.
4. Проверьте таймзону бота в **Bot Settings → General → Timezone**.
5. Подключите следующий шаг.

### Examples

Примеры использования шага.

* `Delay → 10:00` — сообщение отправится в `10:00` по таймзоне бота
* `Delay → 18:30` — шаг выполнится в `18:30` по таймзоне бота

### Notes

Delay всегда работает с учётом таймзоны бота.

<div data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Frame 2248 (18).png" alt=""><figcaption></figcaption></figure></div>

* перед настройкой проверьте timezone в **Bot Settings → General → Timezone**
* шаг выполняется в указанное время
* до наступления этого времени сценарий приостанавливается
* после наступления времени происходит переход к следующему шагу
* используйте шаг, когда нужно выполнить действие в конкретное время, настроить сценарий по расписанию, контролировать тайминг воронки или запускать действия в нужный момент

### Related pages

#### Start and overview

* [О продукте](../../../../dobro-pozhalovat/o-produkte/)
* [Архитектура системы](../../../../dobro-pozhalovat/arkhitektura-sistemy/)
* [Быстрый старт](../../../bystryi-start/)

#### Analytics and management

* [Analytics](../../../analytics/)
* [Tracker](../../../tracker/)
* [Администрирование (Company)](../../../administrirovanie-company/)
* [FAQ и решение проблем](/broken/spaces/AxluUgdTFxFU08qksWVa/pages/yonwUmMhqke1c4edMh5B)

#### Work in the platform

* [CRM](../../../crm/)
* [Конструктор (Flow Settings)](../../)
* [Bot Settings](../../../bot-settings/)

#### Frequent questions

* [Ошибка 403](../../../../faq-i-reshenie-problem/tipy-oshibok/oshibka-403.md)
* [Ошибка 400](../../../../faq-i-reshenie-problem/tipy-oshibok/oshibka-400.md)
* [Типы ботов в Chatterfy](../../../bystryi-start/sozdanie-i-podklyuchenie-bota/tipy-botov-v-chatterfy.md)
* [Как скрыть чаты между операторами](../../../../faq-i-reshenie-problem/chastye-voprosy/kak-skryt-chaty-mezhdu-operatorami.md)
