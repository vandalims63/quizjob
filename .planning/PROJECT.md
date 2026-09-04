# Quiz for Client — Рекрутинговый лендинг + квиз

## What This Is

Сайт-лендинг для рекрутинга мастеров лазерной эпиляции в салон в Кракове. Трафик идёт с Facebook Ads. Кандидат попадает на страницу с вакансией, нажимает кнопку и проходит пошаговый квиз-анкету. Ответы уходят в Telegram-бот клиенту. После отправки — страница "Спасибо" с событием Facebook Pixel Lead.

## Core Value

Кандидат за 2–3 минуты заполняет анкету прямо с телефона, а клиент мгновенно получает заявку в Telegram с полными ответами.

## Requirements

### Validated

(None yet — ship to validate)

### Active

- [ ] Лендинг с вакансией — фоновое изображение/цвет, короткий текст, CTA-кнопка
- [ ] Пошаговый квиз — один вопрос на экране, кнопка "Далее"
- [ ] Типы вопросов: один вариант, несколько вариантов, открытый текст
- [ ] Страница "Спасибо" (отдельный URL для FB Pixel Lead event)
- [ ] Отправка ответов в Telegram-бот
- [ ] Facebook Pixel — базовый код + событие Lead на thank you page
- [ ] Хостинг на GitHub Pages
- [ ] Адаптивный дизайн (mobile-first, трафик с FB = телефоны)
- [ ] Язык сайта — русский

### Out of Scope

- Backend/серверная часть — всё на статическом HTML/CSS/JS + Telegram API
- База данных — ответы хранятся только в Telegram
- Мультиязычность — только русский
- CRM-интеграция — не нужна, ответы в Telegram
- Email-рассылки — не требуются

## Context

**Клиент:** Заказчик Facebook-рекламы, владелец салона лазерной эпиляции в Кракове (Польша).

**Целевая аудитория сайта:** Русскоговорящие девушки-мастера в Польше, ищущие работу.

**Воронка:**
1. Facebook Ad → клик
2. Лендинг с вакансией → CTA-кнопка
3. Пошаговый квиз-анкета → заполнение
4. Страница "Спасибо" → FB Pixel Lead event + текст благодарности
5. Telegram-бот → клиент получает ответы

**Дизайн-референс:** Минималистичный стиль с другими цветами, минимальная анимация. Фоновое изображение будет предоставлено позже.

**Технический стек:**
- Статический HTML/CSS/JS (GitHub Pages)
- Telegram Bot API для отправки ответов
- Facebook Pixel для трекинга

**Данные которые будут предоставлены позже:**
- Название салона и брендинг
- Фоновое изображение / цвета
- Вопросы для квиза с вариантами ответов
- Facebook Pixel ID
- Telegram Bot Token и Chat ID

## Constraints

- **Хостинг**: GitHub Pages — только статические файлы, без серверного кода
- **Telegram API**: Отправка через Bot API прямо из браузера (token в клиентском коде — ок для данного кейса, бот одноцелевой)
- **FB Pixel**: Должен быть на всех страницах (PageView), событие Lead — только на thank you page
- **Mobile-first**: 90%+ трафика будет с мобильных (Facebook Ads)

## Key Decisions

| Decision | Rationale | Outcome |
|----------|-----------|---------|
| Пошаговый квиз (не длинная форма) | Выше конверсия, лучше UX на мобильных | — Pending |
| Отдельная thank you page (не попап) | Нужен уникальный URL для FB Pixel Lead event | — Pending |
| Telegram-бот для ответов | Мгновенная доставка, удобно клиенту | — Pending |
| GitHub Pages хостинг | Бесплатно, быстро, надёжно, первый опыт пользователя | — Pending |
| Статический сайт без бэкенда | Простота, скорость, GitHub Pages совместимость | — Pending |

## Evolution

This document evolves at phase transitions and milestone boundaries.

**After each phase transition** (via `/gsd-transition`):
1. Requirements invalidated? → Move to Out of Scope with reason
2. Requirements validated? → Move to Validated with phase reference
3. New requirements emerged? → Add to Active
4. Decisions to log? → Add to Key Decisions
5. "What This Is" still accurate? → Update if drifted

**After each milestone** (via `/gsd-complete-milestone`):
1. Full review of all sections
2. Core Value check — still the right priority?
3. Audit Out of Scope — reasons still valid?
4. Update Context with current state

---
*Last updated: 2026-09-04 after initialization*
