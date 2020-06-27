# Сущности для навыков Алисы (Яндекс.Диалоги)

Репозиторий содержит набор [пользовательских сущностей](https://yandex.ru/dev/dialogs/alice/doc/nlu-docpage/#granet_sntx__user-entities), которые можно использовать в Яндекс Диалогах (Алиса). Каждая сущность опубликована в отдельном файле в директории `entities`.

Надеюсь, совместными усилиями нам удастся создать библиотеку с качественными сущностями на все случаи жизни и сэкономить десятки часов при разработке новых навыков.

### Список сущностей
* FIGI (Financial Instrument Global Identifier) — российские ценные бумаги, торгующийся на Московской бирже: акции (обычные и привилегированные), глобальные депозитарные расписки.
* Lang: языки, доступные в API Яндекс.Переводчика.

### Как добавить новую сущность
1. Клонируйте репозиторий
2. Создайте файл с именем сущности и расширением `.entity` в директории `entities`. Полажуйста используйте только нижний регистр в названии файла. Например, файл с сущностью FIFI называется `figi.entity`.
3. Поместите [описание сущности](https://yandex.ru/dev/dialogs/alice/doc/nlu-docpage/#granet_sntx__user-entities) в файл. Рекомендуется использовать префикс `E` в названии сущности, например сущность `FIGI` опиывается вот так: `entity EFigi:`.
4. Добавьте описание сущности в список сущностей в файле `README.md`.
5. Создайте Pull Request.
