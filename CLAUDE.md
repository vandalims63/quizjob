# CLAUDE.md

Инструкции для Claude Code в этом проекте.

---

## 🗣️ Язык общения

**Всегда отвечай на русском языке**, если пользователь не попросит иначе.

---

## 🗂️ Контекст проекта

Вся документация и рабочий контекст хранятся в `.planning/`:

| Файл | Назначение |
|------|-----------|
| `.planning/PROJECT.md` | Главный контекст проекта — цели, решения, текущий статус |
| `.planning/config.json` | Настройки GSD-воркфлоу |
| `.planning/codebase/` | Карта кодовой базы |
| `.planning/tasks/` | Активные и выполненные задачи |

**Перед началом любой задачи — прочитай `.planning/PROJECT.md`.**

---

## 🚀 Рабочий процесс

Задачи выполняются через **`/gsd-quick`** — быстрое выполнение с атомарными коммитами.

**Примеры:**
```
/gsd-quick <описание задачи>
```

---

## 📋 Справочник

Детальный контекст: `.planning/PROJECT.md`  
Карта кодовой базы: `.planning/codebase/` (после /gsd-map-codebase)

<!-- GSD:project-start source:PROJECT.md -->
## Project

**Quiz for Client — Рекрутинговый лендинг + квиз**

Сайт-лендинг для рекрутинга мастеров лазерной эпиляции в салон в Кракове. Трафик идёт с Facebook Ads. Кандидат попадает на страницу с вакансией, нажимает кнопку и проходит пошаговый квиз-анкету. Ответы уходят в Telegram-бот клиенту. После отправки — страница "Спасибо" с событием Facebook Pixel Lead.

**Core Value:** Кандидат за 2–3 минуты заполняет анкету прямо с телефона, а клиент мгновенно получает заявку в Telegram с полными ответами.

### Constraints

- **Хостинг**: GitHub Pages — только статические файлы, без серверного кода
- **Telegram API**: Отправка через Bot API прямо из браузера (token в клиентском коде — ок для данного кейса, бот одноцелевой)
- **FB Pixel**: Должен быть на всех страницах (PageView), событие Lead — только на thank you page
- **Mobile-first**: 90%+ трафика будет с мобильных (Facebook Ads)
<!-- GSD:project-end -->

<!-- GSD:stack-start source:STACK.md -->
## Technology Stack

Technology stack not yet documented. Will populate after codebase mapping or first phase.
<!-- GSD:stack-end -->

<!-- GSD:conventions-start source:CONVENTIONS.md -->
## Conventions

Conventions not yet established. Will populate as patterns emerge during development.
<!-- GSD:conventions-end -->

<!-- GSD:architecture-start source:ARCHITECTURE.md -->
## Architecture

Architecture not yet mapped. Follow existing patterns found in the codebase.
<!-- GSD:architecture-end -->

<!-- GSD:skills-start source:skills/ -->
## Project Skills

No project skills found. Add skills to any of: `.claude/skills/`, `.agents/skills/`, `.cursor/skills/`, `.github/skills/`, or `.codex/skills/` with a `SKILL.md` index file.
<!-- GSD:skills-end -->

<!-- GSD:workflow-start source:GSD defaults -->
## GSD Workflow Enforcement

Before using Edit, Write, or other file-changing tools, start work through a GSD command so planning artifacts and execution context stay in sync.

Use these entry points:
- `/gsd-quick` for small fixes, doc updates, and ad-hoc tasks
- `/gsd-debug` for investigation and bug fixing
- `/gsd-execute-phase` for planned phase work

Do not make direct repo edits outside a GSD workflow unless the user explicitly asks to bypass it.
<!-- GSD:workflow-end -->

<!-- GSD:profile-start -->
## Developer Profile

> Profile not yet configured. Run `/gsd-profile-user` to generate your developer profile.
> This section is managed by `generate-claude-profile` -- do not edit manually.
<!-- GSD:profile-end -->
