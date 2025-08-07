# Custom Delay

КАСТОМНАЯ ЗАДЕРЖКА

Теперь ты сможешь выбрать конкретное время, в которое ты хочешь, чтобы выполнился степ (таймзона настраивается в настройках бота). Добавление кастомного времени задержки выполнения степа внутри конструктора делается через новый степ Custom Delay 🔘

{% hint style="danger" %}
**БЫЛО:** До обновления, прежде чем отправить сообщение вам приходилось самостоятельно высчитывать задержку, а именно через сколько часов/минут/секунд отправится сообщение
{% endhint %}

{% hint style="success" %}
**CТАЛО:** Теперь мы упростили фукнционал :)

Все что вам нужно сделать это добавить степ Custom Delay и указать конкретное время, когда вы хотите, чтобы отправилось сообщение! ✨
{% endhint %}

🔗 Выбираешь степ Custom Delay 🔗 Выбираешь время выполнения 🔗 Добавляешь следующий степ, например, Send Message (Пуш2)

#### Разберем на конкретном примере <a href="#razberem-na-konkretnom-primere" id="razberem-na-konkretnom-primere"></a>

1\. Для начала перейди в настройки бота, чтобы добавить таймзону

<figure><img src="../../../.gitbook/assets/image (319).png" alt=""><figcaption></figcaption></figure>

2. Нажми на Bot Settings (Настройки бота)

<figure><img src="../../../.gitbook/assets/image (320).png" alt=""><figcaption></figcaption></figure>

3. Выбери нужную тебе таймзону

<figure><img src="../../../.gitbook/assets/image (321).png" alt=""><figcaption></figcaption></figure>

4. В данном примере выбиарем UTC +03:00 Europe/Moscow

<figure><img src="../../../.gitbook/assets/image (322).png" alt=""><figcaption></figcaption></figure>

5. Не забудь сохранить :)

<figure><img src="../../../.gitbook/assets/image (323).png" alt=""><figcaption></figcaption></figure>

6. Нажми на значок настроек, чтобы вернуться в поле конструктора

<figure><img src="../../../.gitbook/assets/image (324).png" alt=""><figcaption></figcaption></figure>

7. Нажми на кнопку Create Step

<figure><img src="../../../.gitbook/assets/image (325).png" alt=""><figcaption></figcaption></figure>

8. Выбери новый степ Custom Delay (Кастомная задержка)

<figure><img src="../../../.gitbook/assets/image (326).png" alt=""><figcaption></figcaption></figure>

9. Укажи название степа

<figure><img src="../../../.gitbook/assets/image (327).png" alt=""><figcaption></figcaption></figure>

10. В данном примере мы хотим указать конкретное время отправки для Пуша 2.

Кастомный степ задержки называем "Время выполнения Пуш2"



<figure><img src="../../../.gitbook/assets/image (328).png" alt=""><figcaption></figcaption></figure>

12. Переходим в меню Delay и указываем конкретное время в которое хотим, чтобы отправился наш Пуш2

<figure><img src="../../../.gitbook/assets/image (329).png" alt=""><figcaption></figcaption></figure>

13. Добавляем степ Custom Delay (Кастомную задержку) внутрь воронки перед степом Пуш2

<figure><img src="../../../.gitbook/assets/image (330).png" alt=""><figcaption></figcaption></figure>

Теперь Пуш2 отправится клиентам ровно в 15:30 по UTC +03:00 Europe/Moscow времени
