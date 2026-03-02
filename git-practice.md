# Практика Git: ветвление, слияние и конфликты

## 1) Создание рабочей ветки

```bash
git checkout -b feature/update-domain-analysis
```

Внесите изменения в `docs/domain-analysis.md` и зафиксируйте:

```bash
git add docs/domain-analysis.md
git commit -m "Update domain analysis"
```

## 2) Слияние в основную ветку

```bash
git checkout main
git merge feature/update-domain-analysis
```

## 3) Моделирование конфликта

1. Создайте две ветки от `main`:

```bash
git checkout -b feature/a
git checkout main
git checkout -b feature/b
```

2. В обеих ветках измените одну и ту же строку в одном файле (например, `src/main.txt`) и сделайте коммиты.

3. Слейте первую ветку в `main`, затем попытайтесь слить вторую:

```bash
git checkout main
git merge feature/a
git merge feature/b
```

4. Разрешите конфликт вручную, затем:

```bash
git add src/main.txt
git commit -m "Resolve merge conflict in src/main.txt"
```

## 4) Отправка в удалённый репозиторий

```bash
git push -u origin main
git push origin feature/a
git push origin feature/b
```
