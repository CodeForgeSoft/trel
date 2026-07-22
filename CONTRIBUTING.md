# Contributing

Спасибо, что хотите помочь проекту! Мы рады любому участию:
баг-репорты, идеи, пул-реквесты, помощь с дизайном.

---

## Начало работы

1. Форкните репозиторий
2. Создайте ветку от `develop`:
   ```
   git checkout develop
   git pull origin develop
   git checkout -b feature/your-feature-name
   ```
3. Внесите изменения
4. Сделайте коммит (см. раздел «Коммиты»)
5. Откройте Pull Request в `develop`

---

## Как обсуждать изменения

1. **Для идей и вопросов** — откройте [Discussion](https://github.com/CodeForgeSoft/trel/discussions)
2. **Для багов** — создайте Issue с описанием шагов воспроизведения
3. **Для конкретных предложений по коду** — можно сразу PR, но лучше сначала обсудить в Issue, чтобы не делать работу впустую

---

## Ветки

```
main        — продакшен, только через PR из develop
develop     — основная ветка разработки
feature/*   — новые фичи (feature/swipe-animations)
fix/*       — исправления (fix/auth-hydration)
```

- `develop` — всегда стабильна, всё прошло ревью
- Ветки называем кратко, на английском, через дефис

---

## Коммиты

Используем [Conventional Commits](https://www.conventionalcommits.org/):

```
feat:     новая функциональность     → feat: add trail detail page
fix:      исправление бага           → fix: fix hydration error in AuthGuard
refactor: переписывание без новой    → refactor: extract api client
          функциональности             into separate module
docs:     документация               → docs: update README
chore:    настройка, конфиги,        → chore: setup turborepo
          дизайн-ассеты
style:    форматирование             → style: format with prettier
test:     тесты                      → test: add tests for auth api
ci:       CI/CD                      → ci: add github actions workflow
```

Простые правила:
- Тело коммита — на английском, в настоящем времени («add», а не «added»)
- Первая буква строчная, в конце без точки
- Не больше 72 символов в заголовке

---

## Pull Request

- Один PR — одна задача
- Ветка от `develop`, PR в `develop`
- Заголовок PR — как хороший commit message
- В описании кратко: что сделано и зачем

### Чек-лист перед PR

- [ ] `npm run typecheck` проходит
- [ ] `npm run lint` без ошибок
- [ ] `npm run build` успешен
- [ ] Нет закомментированного кода
- [ ] Нет `console.log` (кроме временной отладки)

---

## Стиль кода

Пока проект в начале, единый стайлгайд формируется.
Ориентируемся на дефолтные настройки TypeScript, ESLint, Prettier.

---

## Вопросы

Если что-то непонятно — пишите в [Issues](https://github.com/CodeForgeSoft/trel/issues)
или [Discussions](https://github.com/CodeForgeSoft/trel/discussions).
