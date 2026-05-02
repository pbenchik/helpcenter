---
icon: gears
---

# Domains

Раздел _Domains_ нужен для подключения доменов и поддоменов в Tracker.

Они используются в ссылках кампаний, лендингах и трекинге событий.

### Как это работает

Сначала домен или поддомен настраивается в Cloudflare.

Потом включается `HTTPS` и адрес добавляется в Chatterfy.

### Основной домен

Подходит, если вы хотите использовать основной адрес сайта.

{% embed url="https://youtu.be/zcJyh-e2o4k" %}

#### Шаги

1. [Добавьте домен в Cloudflare](kak-dobavit-domen-v-cloudflare.md)
2. [Настройте SSL](kak-nastroit-ssl.md)
3. [Добавьте домен в Chatterfy](kak-dobavit-domen-v-chatterfy.md)

### Поддомен

Подходит, если основной домен уже подключён и нужен отдельный адрес, например `offer.example.com`.

{% embed url="https://youtu.be/bHK-fuIVYTU" %}

#### Шаги

1. [Добавьте поддомен в Cloudflare](kak-dobavit-poddomen-v-cloudflare.md)
2. [Настройте SSL](kak-nastroit-ssl.md)
3. [Добавьте домен в Chatterfy](kak-dobavit-domen-v-chatterfy.md)

### Notes

{% hint style="info" %}
Если нужен основной адрес сайта, используйте домен. Если нужен отдельный адрес внутри уже подключённого сайта, используйте поддомен.
{% endhint %}

* Подключённый адрес используется для лендингов, ссылок кампаний и трекинга
* Домен можно назначить конкретным байерам
