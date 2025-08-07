# Кастомные поля

Кастомные поля — это функционал, который вы можете добавлять и самостоятельно редактировать в настройках бота.&#x20;

**Вы можете добавлять переменные для любой информации, необходимой вам от клиента!!!**

<figure><img src="../../../.gitbook/assets/CleanShot 2024-09-24 at 16.48.09@2x.png" alt=""><figcaption></figcaption></figure>



## Как создать кастомные поля?&#x20;

1. Перейдите в раздел конструктора бота&#x20;
2. Нажмите на Bot Settings

<figure><img src="../../../.gitbook/assets/image (118).png" alt=""><figcaption></figcaption></figure>

3. Перейдите в раздел Custom Fields (Кастомные поля) и нажмите Add field (Добавить поле)

<figure><img src="../../../.gitbook/assets/image (120).png" alt=""><figcaption></figcaption></figure>

Вам необходимо заполнить **3 колонки:**&#x20;

* слева - **Custom Field KEY**  (уникальное значение, **названия повторяться не могут**)
* посередине - **Name**  (внутреннее обозначение, которое будет отображаться в меню чата)&#x20;
* cправа - **тип поля**



**Типы полей**, доступные к добавлению:

<figure><img src="../../../.gitbook/assets/image (121).png" alt=""><figcaption></figcaption></figure>

* Text - текст&#x20;
* Long text - длинный текст
* Link - ссылка&#x20;
* Number - номер (подходит для заполнения ID)
* Date - дата&#x20;
* Select - выбор поля (можете выбрать только одно; либо 1 либо 2)&#x20;
* Multiselect - множественный выбор полей; и 1 и 2 и 3 и 4 и 5)

<figure><img src="../../../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

4. Не забудьте нажать Сохранить!
5. Перейдем в страницу чатов&#x20;

<figure><img src="../../../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure>

Ваши созданные поля будут отображаться в карточке клиента, где вы сможете заполнять любую необходимую вам информацию

## Инструкция по записи кастомной информации о клиенте&#x20;



Если вам **необходимо записать кастомную информацию о клиенте**, например сумма последнего депозита, ID клиента.&#x20;

{% hint style="success" %}
Вам нужно **в постбеке трекера,** который вы **добавляете в партнерку** **добавить fields.key параметра=параметр из партнерки**&#x20;
{% endhint %}

**Например, постбек для FD**&#x20;

[https://api.chatterfy.ai/api/postbacks/51edc052-f7a2-4650-8085-d04abb38de5e/tracker-postback?clickid={clickid}\&tracker.event=sale\&tracker.cost={cost}\&tracker.currency=usd\&fields.last\_deposit={cost}\&fields.user\_id={user\_id}](../../../chatterfy.ai/update-log/update-06.10.2024.md)

Таким образом,  **пользователю запишется ивент sale**, а **в кастом филды** пользователя **запишется параметры last\_deposit и user\_id**

