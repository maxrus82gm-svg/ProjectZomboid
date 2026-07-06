# Правила Git и Review

## Назначение

Документ описывает безопасную работу с Git, GitHub, diff, status, review и историей изменений в проекте `Project Zomboid Dedicated Server`.

Репозиторий:

```text
https://github.com/maxrus82gm-svg/ProjectZomboid.git
```

Базовый хеш:

```text
a3d392d9547a50af709876cd39f56e49cabc8a2e
```

Политика Git:

```text
Git контролирует пользователь. Агент не делает commit, push, pull, merge, rebase, reset, clean, checkout, switch, создание веток, изменение remote, изменение Git-конфига или переписывание истории без прямой команды пользователя.
```

## Главное правило Git

Git контролирует пользователь.

Агент не делает commit, push, pull, merge, rebase, reset, clean, checkout, switch, создание веток, изменение remote, изменение Git-конфига или переписывание истории без прямой команды пользователя.

Read-only Git-команды разрешены только если текущая задача прямо разрешила Git-проверку.

Если текущая задача запрещает Git, не выполнять даже команды чтения.

Разрешённые read-only команды для TASK 001:

```bat
cd /d M:\GitHub\ProjectZomboid
git status
git remote -v
git branch
git log --oneline -5
```

## Review после отчёта агента

Любой review после отчёта агента начинается с:

```text
СТАТУС КОММИТА: "<commit message>"
Repository: maxrus82gm-svg/ProjectZomboid
Branch: main
Commit: <short sha>
Проверка: изменения найдены / push не обнаружен / требуется уточнение
```

Затем идут:

```text
GIT / REPOSITORY CHECK
REVIEW STATUS
FINDINGS
PROBLEMS
NEXT
```

Если commit message не подтверждён, писать `message не подтверждён`.

Если push не обнаружен, писать `push не обнаружен`.

GitHub не равен локальному Git: GitHub показывает только то, что уже попало в удалённый репозиторий.

## Служебные файлы как UNEXPECTED CHANGES

Если при GitHub / Git / diff / review-проверке обнаружены изменения в служебных файлах, которые не входили в scope задачи, они указываются в `UNEXPECTED CHANGES`.

Служебные папки проекта:

```text
.git; .obsidian; Шаблон_агентской_системы
```

Служебные файлы IDE:

```text
НЕ УКАЗАНО
```

Запрещено писать служебные файлы как `UNCHANGED`, если проверенный diff показывает, что они изменялись.

Если Git / GitHub / diff не проверялись, агент не утверждает, что служебные файлы не менялись. В этом случае писать: `не проверялось`.

## Запреты для этой базы

- Не менять `.git`.
- Не менять `.obsidian`.
- Не менять `M:\GitHub\ProjectZomboid\Шаблон_агентской_системы`.
- Не менять серверную папку `\\192.168.0.77\Server\Project Zomboid Dedicated Server`.
- Не менять серверную папку `C:\Server\Project Zomboid Dedicated Server`.

## Формат проверки

```text
GIT / REPOSITORY CHECK

Repository:
-

Branch:
-

Status:
-

Changed files:
-

Diff summary:
-

UNEXPECTED CHANGES:
-

Commit:
-

Push:
-

Pull:
-

GitHub check:
-
```
