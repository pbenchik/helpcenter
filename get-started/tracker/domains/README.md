---
icon: gears
---

# Domains

> ### Раздел Domains нужен для подключения доменов и поддоменов в Tracker.

Они используются в ссылках кампаний, лендингах и трекинге событий.

### &#x20;Что и как можно подключить:

{% tabs %}
{% tab title="Домен" %}
{% hint style="info" %}
Подходит, если вы хотите использовать основной адрес сайта.

Обычно настройка состоит из трёх шагов:

1. Добавить домен в Cloudflare.
2. Настроить SSL.
3. Добавить домен в Chatterfy.
{% endhint %}

Видеоинструкция:

{% embed url="https://youtu.be/zcJyh-e2o4k" %}

<a href="kak-dobavit-domen-v-cloudflare.md" class="button secondary" data-icon="cloud">Как добавить домен в Cloudflare</a> <a href="kak-nastroit-ssl.md" class="button secondary" data-icon="lock">Как настроить SSL</a>&#x20;

<a href="kak-dobavit-domen-v-chatterfy.md" class="button secondary" data-icon="plus">Как добавить домен в Chatterfy</a>
{% endtab %}

{% tab title="Поддомен" %}
{% hint style="info" %}
Подходит, если основной домен уже подключён и нужен отдельный адрес, например `offer.example.com`.

Обычно настройка состоит из трёх шагов:

1. Создать DNS-запись поддомена в Cloudflare.
2. Проверить SSL.
3. Добавить поддомен в Chatterfy.
{% endhint %}

**Видео-инструкция:**&#x20;

{% embed url="https://youtu.be/bHK-fuIVYTU" %}

<a href="kak-dobavit-poddomen-v-cloudflare.md" class="button secondary" data-icon="plus">Как добавить поддомен в Cloudflare</a> <a href="kak-nastroit-ssl.md" class="button secondary" data-icon="lock">Как настроить SSL</a>&#x20;

<a href="kak-dobavit-domen-v-chatterfy.md" class="button secondary" data-icon="plus">Как добавить домен в Chatterfy</a>
{% endtab %}
{% endtabs %}

### Зачем это нужно:

Подключенный домен или поддомен используется для:

* открытия лендингов
* генерации ссылок кампаний
* корректной работы трекинга

Домен можно назначить конкретным байерам, чтобы разделять доступ и управление.

{% hint style="info" %}
Если нужен основной адрес сайта, используйте домен.

Если нужен отдельный адрес внутри уже подключённого сайта, используйте поддомен.
{% endhint %}
