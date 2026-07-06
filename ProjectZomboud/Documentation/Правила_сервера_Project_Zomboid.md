# Правила сервера Project Zomboid

Документ фиксирует правила безопасной работы с dedicated server Project Zomboid, Workshop-модами и путями сервера.

## Пути сервера и локального источника модов

Локальный источник Workshop-модов на рабочей машине:

```text
G:\SteamLibrary\steamapps\workshop\content\108600
```

Эта папка не является сервером. Это локальный источник уже скачанных Workshop-модов.

Сетевая папка dedicated server:

```text
\\192.168.0.77\Server\Project Zomboid Dedicated Server
```

Этот путь используется агентом с рабочей машины для доступа к серверу по сети.

Локальный путь сервера на серверной машине:

```text
C:\Server\Project Zomboid Dedicated Server
```

Этот путь актуален только при работе непосредственно на серверной машине.

Целевая папка Workshop-модов сервера по сети:

```text
\\192.168.0.77\Server\Project Zomboid Dedicated Server\steamapps\workshop\content\108600
```

Та же папка локально на серверной машине:

```text
C:\Server\Project Zomboid Dedicated Server\steamapps\workshop\content\108600
```

## Правила Workshop-модов

- Workshop-моды копируются только в `steamapps\workshop\content\108600`.
- Не класть Workshop-моды просто рядом с сервером.
- Не переименовывать папки Workshop ID.
- Не удалять локальные Workshop-моды.
- Не удалять Workshop-моды на сервере без отдельной явной задачи пользователя.
- При копировании сохранять структуру папок Workshop ID.
- `WorkshopItems=` собирается из цифровых имён папок.
- `Mods=` собирается из строк `id=` внутри `mod.info`.
- Если в одном Workshop ID несколько файлов `mod.info`, нужно учитывать все найденные ModID.

## Запуск и основной конфиг сервера

Основной файл запуска dedicated server по сети:

```text
\\192.168.0.77\Server\Project Zomboid Dedicated Server\StartServer64.bat
```

Локально на серверной машине:

```text
C:\Server\Project Zomboid Dedicated Server\StartServer64.bat
```

Файл запуска `StartServer64.bat` не менять без отдельной явной задачи пользователя.

Основной файл настройки сервера обычно находится в профиле пользователя Windows на серверной машине:

```text
C:\Users\<имя_пользователя>\Zomboid\Server\servertest.ini
```

При работе с рабочей машины нужен доступный сетевой путь к этому профилю. Если профиль сервера недоступен по сети, не выдумывать путь и не менять случайные файлы.

В `servertest.ini` подключаются Workshop-моды через строки:

```text
WorkshopItems=...
Mods=...
```

Перед изменением `servertest.ini` всегда делать backup рядом с исходным файлом.

Сервер не запускать и не останавливать без отдельной явной задачи пользователя.

## Запреты для серверных конфигов

Без отдельной явной задачи пользователя не менять:

- `servertest.ini`;
- `servertest_SandboxVars.lua`;
- `servertest_spawnpoints.lua`;
- `servertest_spawnregions.lua`;
- сохранения;
- базу игроков;
- моды;
- Workshop-файлы;
- логи сервера.

## Запуск и остановка

- Не запускать сервер без отдельной явной задачи пользователя.
- Не останавливать сервер без отдельной явной задачи пользователя.
- Не обновлять dedicated server без отдельной явной задачи пользователя.

## Текущий список модов

Актуальный список Workshop ID и ModID хранится в документе:

```text
M:\GitHub\ProjectZomboid\ProjectZomboud\Documentation\Список_модов_Project_Zomboid.md
```
