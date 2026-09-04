# Requirements: Quiz for Client

**Defined:** 2026-09-04
**Core Value:** Кандидат за 2–3 минуты заполняет анкету прямо с телефона, а клиент мгновенно получает заявку в Telegram с полными ответами.

## v1 Requirements

### Лендинг

- [ ] **LAND-01**: Страница с фоновым изображением/цветом и коротким текстом о вакансии
- [ ] **LAND-02**: CTA-кнопка ведущая на квиз-анкету
- [ ] **LAND-03**: Адаптивный дизайн (mobile-first)

### Квиз

- [ ] **QUIZ-01**: Пошаговый формат — один вопрос на экране
- [ ] **QUIZ-02**: Тип вопроса: один вариант ответа (radio)
- [ ] **QUIZ-03**: Тип вопроса: несколько вариантов (checkbox)
- [ ] **QUIZ-04**: Тип вопроса: открытый текст (textarea)
- [ ] **QUIZ-05**: Индикатор прогресса (шаг N из M)
- [ ] **QUIZ-06**: Кнопка "Далее" / "Назад" для навигации

### Интеграции

- [ ] **INTG-01**: Отправка ответов в Telegram-бот при завершении квиза
- [ ] **INTG-02**: Facebook Pixel — базовый код PageView на всех страницах
- [ ] **INTG-03**: Facebook Pixel — событие Lead на странице "Спасибо"

### Финал

- [ ] **FINL-01**: Страница "Спасибо" с текстом благодарности (отдельный URL)

### Деплой

- [ ] **DEPL-01**: Хостинг на GitHub Pages
- [ ] **DEPL-02**: Подключение к GitHub-репозиторию

## v2 Requirements

### Расширения

- **EXT-01**: Валидация ответов (обязательные поля, формат телефона/email)
- **EXT-02**: Сохранение прогресса квиза (если пользователь закрыл и вернулся)
- **EXT-03**: A/B тестирование текстов и CTA-кнопок
- **EXT-04**: Google Analytics интеграция

## Out of Scope

| Feature | Reason |
|---------|--------|
| Backend/серверная часть | Всё статическое, Telegram API из браузера |
| База данных | Ответы хранятся только в Telegram |
| CRM-интеграция | Не нужна клиенту |
| Мультиязычность | Только русский |
| Email-рассылки | Не требуются |
| Мобильное приложение | Web-only |

## Traceability

| Requirement | Phase | Status |
|-------------|-------|--------|
| LAND-01 | — | Pending |
| LAND-02 | — | Pending |
| LAND-03 | — | Pending |
| QUIZ-01 | — | Pending |
| QUIZ-02 | — | Pending |
| QUIZ-03 | — | Pending |
| QUIZ-04 | — | Pending |
| QUIZ-05 | — | Pending |
| QUIZ-06 | — | Pending |
| INTG-01 | — | Pending |
| INTG-02 | — | Pending |
| INTG-03 | — | Pending |
| FINL-01 | — | Pending |
| DEPL-01 | — | Pending |
| DEPL-02 | — | Pending |

**Coverage:**
- v1 requirements: 15 total
- Mapped to phases: 0
- Unmapped: 15 ⚠️

---
*Requirements defined: 2026-09-04*
*Last updated: 2026-09-04 after initial definition*
