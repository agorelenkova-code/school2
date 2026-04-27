# Ответы на тестовые вопросы — Google Sheets
_Дата: 2026-04-27_

---

## Вопрос 1: Сколько у Ирины Комаровой учеников 9 класса?

**Короткий ответ:**
По Сводному мастеру (основной источник, явная колонка «Куратор»): **8 учеников** 9-го класса со статусом «обучается».
По личной таблице Комаровой (Классы 7-9): **10 строк** в 9-м классе — 2 из них (Лапшина Варвара, Нефёдова Дарья) в Сводный мастер не внесены. Обнаружено расхождение между источниками; для отчётности требуется сверка.

**Источник (основной):** Таблица 1 — Сводный мастер (Шумилова)
`1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ`

| ФИО | Класс | Строка | Ссылка |
|---|---|---|---|
| Саврасов Роман Алексеевич | 9А | 12 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A12:Z12 |
| Ковалёв Матвей Сергеевич | 9А | 28 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A28:Z28 |
| Яровой Платон Константинович | 9А | 38 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A38:Z38 |
| Петрова Мария Сергеевна | 9А | 49 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A49:Z49 |
| Рубцов Захар Владимирович | 9А | 51 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A51:Z51 |
| Бабичев Лев Андреевич | 9А | 56 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A56:Z56 |
| Шубин Илья Андреевич | 9А | 67 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A67:Z67 |
| Эсаулов Захар Сергеевич | 9А | 69 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A69:Z69 |

**Источник (дополнительный):** Таблица 2 — Классы 7-9 (Комарова)
`1vXmmNYBq4haCTK3Z-mDY_-FxW6PTWmpS39pFLyHAO9o`

Строки только в Таблице 2, отсутствующие в Сводном мастере:

| ФИО | Класс | Строка | Ссылка |
|---|---|---|---|
| Лапшина Варвара Михайловна | 9А | 12 | https://docs.google.com/spreadsheets/d/1vXmmNYBq4haCTK3Z-mDY_-FxW6PTWmpS39pFLyHAO9o/edit?gid=0&range=A12:Z12 |
| Нефёдова Дарья Викторовна | 9А | 14 | https://docs.google.com/spreadsheets/d/1vXmmNYBq4haCTK3Z-mDY_-FxW6PTWmpS39pFLyHAO9o/edit?gid=0&range=A14:Z14 |

**Основание:** Таблица 1 — фильтр по кол. D («Куратор» = «Ирина Комарова») + кол. B (Класс начинается с «9»), все найденные строки со статусом «обучается». Таблица 2 — фильтр по кол. B (Класс начинается с «9»); куратор следует из названия таблицы, а не из данных строк.

**Ограничения:**
- В Таблице 2 куратор не указан в строках — принадлежность Комаровой определена из названия файла.
- Лапшина и Нефёдова есть в Таблице 2, но отсутствуют в Таблице 1. Природа расхождения не установлена; требуется ручная сверка перед использованием в отчётности.

---

## Вопрос 2: Какие у нас сейчас многодетные семьи, где 3+ детей?

**Короткий ответ:**
По Таблице 5 (единственный источник с данными о составе семей): **8 многодетных семей** со статусом «многодетная (3+)». Все помечены как кандидаты на скидку 15%.

**Источник:** Таблица 5 — Семьи (Белов)
`1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8`

| Семья | Детей | Дети (класс, тариф) | Строка | Ссылка |
|---|---|---|---|---|
| Лапшин | 5 | Даниил (3А, Мини); Макар (6В, Стандарт); Полина (8А, Премиум); Варвара (9А, Премиум); Василиса (11Б, Годовой) | 2 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A2:Z2 |
| Дёмин | 4 | Арсений (6А, Стандарт); Ника (9Б, Премиум); Тимофей (11Б, Профи); Марфа (2А, Мини) | 3 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A3:Z3 |
| Нефёдов | 4 | Глеб (3Б, Мини); Тимур (6Б, Стандарт); Дарья (9А, Премиум); Алиса (11А, Профи) | 4 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A4:Z4 |
| Быков | 3 | Максим (5А, Стандарт); Анастасия (8Б, Премиум); Елизавета (11А, Профи) | 5 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A5:Z5 |
| Грачёв | 3 | Иван (7В, Стандарт); Екатерина (10Б, Премиум); София (4А, Мини) | 6 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A6:Z6 |
| Кремнёв | 3 | Лев (4Б, Мини); Арина (7А, Стандарт); Платон (10А, Профи) | 7 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A7:Z7 |
| Миронцев | 3 | Артём (5Б, Стандарт); Матвей (8В, Премиум); Милана (10А, Профи) | 8 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A8:Z8 |
| Саврасов | 3 | Ева (4А, Мини); Ульяна (7Б, Стандарт); Роман (9А, Премиум) | 9 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A9:Z9 |

**Основание:** Фильтр по кол. D («Кол-во детей» ≥ 3); все найденные строки дополнительно содержат статус «многодетная (3+) — кандидат на скидку 15%» в кол. I.

**Ограничения:**
- Таблица 5 ведётся куратором Беловым — семьи из зон других кураторов могут быть не внесены.
- Колонка «Статус» в Таблице 5 не содержит признака активности семьи (все записи считаются актуальными).

---

## Вопрос 3: Кто ведёт семью Петровых?

**Короткий ответ:**
Семья Петровых — двое детей с разными кураторами:
- **Фёдор Петров** (6Б) — куратор **Ольга Тишина**
- **Мария Петрова** (9А) — куратор **Ирина Комарова**

Единого куратора семьи нет. Сверка источников не требуется — данные согласованы.

**Источник (основной):** Таблица 1 — Сводный мастер (Шумилова)
`1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ`

| ФИО | Класс | Куратор | Строка | Ссылка |
|---|---|---|---|---|
| Петров Фёдор Сергеевич | 6Б | Ольга Тишина | 19 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A19:Z19 |
| Петрова Мария Сергеевна | 9А | Ирина Комарова | 49 | https://docs.google.com/spreadsheets/d/1jURj2nIQlxIUQIIqakQoin1eePK1hls0y3gKaE8OgIQ/edit?gid=0&range=A49:Z49 |

**Источник (подтверждающий):** Таблица 5 — Семьи (Белов)
`1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8`

| Семья | Дети | Строка | Ссылка |
|---|---|---|---|
| Петров | Фёдор (6Б, Годовой); Мария (9А, Премиум) | 10 | https://docs.google.com/spreadsheets/d/1oxM7Wigz5S3VIY3_m0aLxbYXtdHT3WWwcnkKH4XABj8/edit?gid=0&range=A10:Z10 |

**Основание:** Таблица 1 — фильтр по кол. E («Семья (фамилия)» = «Петров»), куратор взят из кол. D. Таблица 5 — строка с `Семья` = «Петров» подтверждает состав: двое детей совпадают с найденными в Таблице 1.

**Ограничения:**
- У семьи двое детей с разными кураторами — при эскалации вопросов по семье в целом необходимо уточнить, кто из кураторов является основным контактом.
