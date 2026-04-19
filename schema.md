# Схема базы данных — Онлайн-школа «Ромашка»

> Получена: апрель 2026 · Источник: Metabase

---

## Таблицы

### students — Ученики
| Колонка | Тип | Описание |
|---|---|---|
| id | int | PK |
| last_name | str | Фамилия |
| first_name | str | Имя |
| patronymic | str | Отчество |
| class | str | Класс (например, 5А) |
| grade_level | int | Звено (1–4 нач., 5–9 ср., 10–11 ст.) |
| tariff | str | Тариф |
| start_date | date | Дата начала обучения |
| status | str | Статус ученика |
| homeroom_teacher_id | int | FK → teachers.id |

**Значения status:**
- `active` — 889
- `graduated` — 93
- `left` — 15

**Значения tariff:**
- `Онлайн-школа` — 533
- `Без зачисления` — 260
- `Без учителя` — 102
- `Персональный` — 102

---

### payments — Платежи
| Колонка | Тип | Описание |
|---|---|---|
| id | int | PK |
| student_id | int | FK → students.id |
| month | date | Расчётный месяц |
| amount | numeric | Сумма |
| due_date | date | Дата списания по плану |
| paid_date | date | Фактическая дата оплаты |
| status | str | Статус платежа |
| tariff | str | Тариф на момент платежа |

**Значения status:**
- `paid` — 6 980
- `annual_prepaid` — 707
- `overdue` — 420
- `partial` — 382

**Значения tariff:**
- `Онлайн-школа` — 4 532
- `Без зачисления` — 2 217
- `Без учителя` — 871
- `Персональный` — 869

---

### renewals — Продления
| Колонка | Тип | Описание |
|---|---|---|
| id | int | PK |
| student_id | int | FK → students.id |
| current_year | int | Учебный год (например, 2025) |
| renewal_status | str | Статус продления |
| renewal_date | date | Дата фиксации решения |
| next_year_tariff | str | Тариф на следующий год |
| comment | str | Комментарий |

**Значения renewal_status:**
- `renewed` — 447
- `declined` — 228
- `no_response` — 214
- `pending` — 108

**Значения next_year_tariff:**
- `Онлайн-школа` — 227
- `Без зачисления` — 105
- `Без учителя` — 84
- `Персональный` — 31
- *(пусто)* — 550

---

### courses — Курсы
| Колонка | Тип | Описание |
|---|---|---|
| id | int | PK |
| name | str | Название курса |
| teacher_id | int | FK → teachers.id |
| grade_level | int | Уровень / класс |
| price_monthly | numeric | Стоимость в месяц |

---

### teachers — Педагоги
| Колонка | Тип | Описание |
|---|---|---|
| id | int | PK |
| name | str | ФИО педагога |
| subject | str | Предмет |

---

### satisfaction — Удовлетворённость
| Колонка | Тип | Описание |
|---|---|---|
| id | int | PK |
| student_id | int | FK → students.id |
| score | int | Оценка |
| comment | str | Комментарий |
| survey_date | date | Дата заполнения |

---

## Связи

```
students ──< payments       (students.id = payments.student_id)
students ──< renewals       (students.id = renewals.student_id)
students ──< satisfaction   (students.id = satisfaction.student_id)
students >── teachers       (students.homeroom_teacher_id = teachers.id)
courses  >── teachers       (courses.teacher_id = teachers.id)
```

---

## Ключевые цифры

| Метрика | Значение |
|---|---|
| Всего учеников | 997 (889 active + 93 graduated + 15 left) |
| Всего платежей | 8 489 |
| Всего записей о продлении | 997 |
| Решение принято | 675 (renewed + declined) |
| Без ответа / в ожидании | 322 (no_response + pending) |
