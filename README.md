# ТРПО — Лекция 9: Изучение работы в системе контроля версий

Этот репозиторий подготовлен как шаблон для практической работы по теме систем контроля версий (VCS) и Git.

## Структура репозитория

- `src/` — исходные файлы проекта.
- `docs/domain-analysis.md` — отчёт по анализу предметной области (ПР №1).
- `docs/technical-specification.md` — техническое задание (ПР №2).
- `docs/software-architecture.md` — документация по архитектуре ПО (ПР №3).
- `git-practice.md` — пошаговая практика по ветвлению, слиянию и конфликтам.

## Быстрый старт

```bash
git init
git add .
git commit -m "Initial commit: lecture 9 practice template"
```

## Подключение удалённого репозитория

```bash
git remote add origin https://github.com/<username>/<repo>.git
git remote -v
git push -u origin main
```

## Рекомендуемое имя репозитория

`ФамилияИмяСтудента_номерВарианта`

Пример: `ИвановИван_7`.
