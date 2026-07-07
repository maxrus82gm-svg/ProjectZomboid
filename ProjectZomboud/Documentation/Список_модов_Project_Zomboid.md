# Список модов Project Zomboid

Документ сформирован по локальной папке Workshop-модов и результату копирования в серверную Workshop-папку.

## Дата проверки

```text
2026-07-06 23:31:16 +05:00
```

## Пути

Локальный источник модов:

```text
G:\SteamLibrary\steamapps\workshop\content\108600
```

Сетевой путь сервера:

```text
\\192.168.0.77\Server\Project Zomboid Dedicated Server
```

Целевая Workshop-папка сервера:

```text
\\192.168.0.77\Server\Project Zomboid Dedicated Server\steamapps\workshop\content\108600
```

## Итоги

- Найдено Workshop ID: 59
- Найдено ModID: 72
- Скопировано или обновлено при проверочном проходе: 2
- Уже было актуально на сервере: 57
- Ошибок копирования: 0

## Добавленные русские переводы

- `PZ B42 RU Translation - Русский перевод`
- Workshop ID: `3455290347`
- ModID: `PZB42RUTranslation`
- Статус: скачан локально, скопирован на сервер, включён в `servertest.ini`.

- `[B42] Project zomboid translate to Russian (by rennocki)`
- Workshop ID: `3748865313`
- ModID: `[B42] Project zomboid translate to Russian (by rennocki)`
- Требует: `PZB42RUTranslation`
- Статус: скачан локально, скопирован на сервер, включён в `servertest.ini`.

## Статус подключения к серверу

- Дата проверки подключения: 2026-07-06 23:31:16 +05:00
- `StartServer64.bat` найден: да
- Файл запуска по сети: `\\192.168.0.77\Server\Project Zomboid Dedicated Server\StartServer64.bat`
- Файл запуска локально на серверной машине: `C:\Server\Project Zomboid Dedicated Server\StartServer64.bat`
- SHA256 `StartServer64.bat`: `1C3FEF0A65F56E1A0D75BB376822D3BACABA5CBAB05B10C0E269E4521B0A0953`
- `servertest.ini` найден: да
- Ожидаемый путь на серверной машине: `C:\Users\silver\Zomboid\Server\servertest.ini`
- Использованный сетевой путь к конфигу: `\\192.168.0.77\ZomboidServerConfig\servertest.ini`
- Backup `servertest.ini` создан: да
- Backup: `\\192.168.0.77\ZomboidServerConfig\servertest.ini.backup_RU_TRANSLATIONS_2026-07-06_23-31-16`
- `WorkshopItems=` применён в `servertest.ini`: да
- `Mods=` применён в `servertest.ini`: да
- Workshop ID применено: 59
- ModID применено: 72
- Серверная Workshop-папка проверена: да
- Workshop ID в серверной Workshop-папке: 59
- Сервер запускался: нет
- Сервер останавливался: нет

## Примечание по кодировке `servertest.ini`

Этот Markdown-документ хранится в UTF-8, но при переносе строк `WorkshopItems=` и `Mods=` в реальный `servertest.ini` нужно сохранять исходную кодировку серверного конфига.

Текущий `servertest.ini` с русскими комментариями нельзя бездумно сохранять в UTF-8. Если он читается корректно как Windows-1251, перед изменением нужно сделать backup рядом с файлом и после изменения сохранить `servertest.ini` обратно в Windows-1251.

## Как обновлять список модов

Источник списка - локальная Workshop-папка:

```text
G:\SteamLibrary\steamapps\workshop\content\108600
```

`WorkshopItems=` берётся из цифровых имён папок в источнике. `Mods=` берётся из строк `id=` во всех файлах `mod.info` внутри этих папок.

Workshop-файлы копируются на сервер только в:

```text
\\192.168.0.77\Server\Project Zomboid Dedicated Server\steamapps\workshop\content\108600
```

Готовые строки ниже вставляются только в:

```text
\\192.168.0.77\ZomboidServerConfig\servertest.ini
```

Перед изменением `servertest.ini` обязателен backup рядом с файлом. Если новый мод подписан в Steam, но его цифровой папки ещё нет в локальном источнике, мод не добавляется в строки ниже до фактической загрузки Workshop-файлов.

## WorkshopItems

```text
WorkshopItems=498441420;533833878;926315905;1551818411;1576361194;1962761540;2056238799;2064137012;2081538550;2110771295;2142622992;2618566294;2642070841;2734855468;2753086629;2757712197;2875848298;2948824747;2950902979;2984301200;3038695235;3141640932;3146046428;3149109194;3261334016;3281755175;3378285185;3378304610;3386498516;3388017161;3389605231;3390487814;3392356751;3392745472;3395171770;3396542795;3406392630;3410989950;3423660713;3425287730;3429176285;3436499337;3436537035;3437629766;3455290347;3461263912;3495906499;3508537032;3546314080;3567084868;3575895484;3591960030;3597673472;3610005735;3617732907;3624971238;3663239580;3684808606;3748865313
```

## Mods

```text
Mods=Hydrocraft;ALICE;svgMCerdato;ORGMAmmoCrafting;curevirus41;ArmoredVestsPatch;ArmoredVests;LockpickingOnly;ZIL130PACK2;Waistbags;RepairAnyClothes;RepairAnyMod;MattSimpleAddonsFriuts;PrepperEquipment;GlassRepair;survivingthroughseasons;VehicleSalvageOverhaulB42;VehicleRepairOverhaul;BB_CommonSense;RiskyInspectWeapon;EQUIPMENT_UI;RACNewVersion;Immersive horror overlays;BirgetPMClothingCorrection;BirgetFemaleBodyModel;PlumbHelp;BirgetMaleBodyModel;rope-towing;VanillaVehiclesAnimated;VanillaVehiclesAnimated_SVU;VVA_cullseats;VVA_PikamyDelight;VVA_slowdoors;VVA_snapDoors;VVA_transparentWindows;StarlitLibrary;RepairableWindows;KAMER_WallHealth_b42;BecomeDesensitizedB42;TchernoLib;DEON_CVG;WhatCanICraft_Addon;BoredomTweaks;moodlesinlua;DeonReloadingBench;DeonART_RFGP;SKITTLE_LongTermPreservation;TrueCrawl;ModLoadOrderSorter_b42;B42RainsFirearmsAndGunParts-RU;campintherain_42.13;campintherain;VMZNEW;UsefulBarrels;UsefulBarrelsMP;CleanUI;PZB42RUTranslation;CleanHotBar;SurvivalHUD;NeatUI_Framework;Waterpipes;ModManager;Ivmakk_CleanUIExtension;INSWEARUS;LongTermPreservationExtended;LongTermPreservationExtendedUI;AliceGear;ItemInspectionUI;YAPZLib;cleanblood;RepairWallCracks_B42;[B42] Project zomboid translate to Russian (by rennocki)
```

## Таблица соответствий

| Workshop ID | Путь к папке                                                 | ModID                                                                                                                                  | mod.info | Скопировано на сервер |
| ----------- | ------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- | -------- | --------------------- |
| 498441420   | G:\SteamLibrary\steamapps\workshop\content\108600\498441420  | Hydrocraft                                                                                                                             | да       | уже было              |
| 533833878   | G:\SteamLibrary\steamapps\workshop\content\108600\533833878  | ALICE                                                                                                                                  | да       | уже было              |
| 926315905   | G:\SteamLibrary\steamapps\workshop\content\108600\926315905  | svgMCerdato                                                                                                                            | да       | уже было              |
| 1551818411  | G:\SteamLibrary\steamapps\workshop\content\108600\1551818411 | ORGMAmmoCrafting                                                                                                                       | да       | уже было              |
| 1576361194  | G:\SteamLibrary\steamapps\workshop\content\108600\1576361194 | curevirus41                                                                                                                            | да       | уже было              |
| 1962761540  | G:\SteamLibrary\steamapps\workshop\content\108600\1962761540 | ArmoredVestsPatch;ArmoredVests                                                                                                         | да       | уже было              |
| 2056238799  | G:\SteamLibrary\steamapps\workshop\content\108600\2056238799 | LockpickingOnly                                                                                                                        | да       | уже было              |
| 2064137012  | G:\SteamLibrary\steamapps\workshop\content\108600\2064137012 | ZIL130PACK2                                                                                                                            | да       | уже было              |
| 2081538550  | G:\SteamLibrary\steamapps\workshop\content\108600\2081538550 | Hydrocraft                                                                                                                             | да       | уже было              |
| 2110771295  | G:\SteamLibrary\steamapps\workshop\content\108600\2110771295 | Waistbags                                                                                                                              | да       | уже было              |
| 2142622992  | G:\SteamLibrary\steamapps\workshop\content\108600\2142622992 | RepairAnyClothes;RepairAnyMod                                                                                                          | да       | уже было              |
| 2618566294  | G:\SteamLibrary\steamapps\workshop\content\108600\2618566294 | MattSimpleAddonsFriuts                                                                                                                 | да       | уже было              |
| 2642070841  | G:\SteamLibrary\steamapps\workshop\content\108600\2642070841 | PrepperEquipment                                                                                                                       | да       | уже было              |
| 2734855468  | G:\SteamLibrary\steamapps\workshop\content\108600\2734855468 | GlassRepair                                                                                                                            | да       | уже было              |
| 2753086629  | G:\SteamLibrary\steamapps\workshop\content\108600\2753086629 | survivingthroughseasons                                                                                                                | да       | уже было              |
| 2757712197  | G:\SteamLibrary\steamapps\workshop\content\108600\2757712197 | VehicleSalvageOverhaulB42;VehicleRepairOverhaul                                                                                        | да       | уже было              |
| 2875848298  | G:\SteamLibrary\steamapps\workshop\content\108600\2875848298 | BB_CommonSense                                                                                                                         | да       | уже было              |
| 2948824747  | G:\SteamLibrary\steamapps\workshop\content\108600\2948824747 | RiskyInspectWeapon                                                                                                                     | да       | уже было              |
| 2950902979  | G:\SteamLibrary\steamapps\workshop\content\108600\2950902979 | EQUIPMENT_UI                                                                                                                           | да       | уже было              |
| 2984301200  | G:\SteamLibrary\steamapps\workshop\content\108600\2984301200 | RACNewVersion                                                                                                                          | да       | уже было              |
| 3038695235  | G:\SteamLibrary\steamapps\workshop\content\108600\3038695235 | Immersive horror overlays                                                                                                              | да       | уже было              |
| 3141640932  | G:\SteamLibrary\steamapps\workshop\content\108600\3141640932 | BirgetPMClothingCorrection;BirgetFemaleBodyModel                                                                                       | да       | уже было              |
| 3146046428  | G:\SteamLibrary\steamapps\workshop\content\108600\3146046428 | PlumbHelp                                                                                                                              | да       | уже было              |
| 3149109194  | G:\SteamLibrary\steamapps\workshop\content\108600\3149109194 | BirgetMaleBodyModel;BirgetPMClothingCorrection                                                                                         | да       | уже было              |
| 3261334016  | G:\SteamLibrary\steamapps\workshop\content\108600\3261334016 | rope-towing                                                                                                                            | да       | уже было              |
| 3281755175  | G:\SteamLibrary\steamapps\workshop\content\108600\3281755175 | VanillaVehiclesAnimated;VanillaVehiclesAnimated_SVU;VVA_cullseats;VVA_PikamyDelight;VVA_slowdoors;VVA_snapDoors;VVA_transparentWindows | да       | уже было              |
| 3378285185  | G:\SteamLibrary\steamapps\workshop\content\108600\3378285185 | StarlitLibrary                                                                                                                         | да       | уже было              |
| 3378304610  | G:\SteamLibrary\steamapps\workshop\content\108600\3378304610 | RepairableWindows                                                                                                                      | да       | уже было              |
| 3386498516  | G:\SteamLibrary\steamapps\workshop\content\108600\3386498516 | KAMER_WallHealth_b42                                                                                                                   | да       | уже было              |
| 3388017161  | G:\SteamLibrary\steamapps\workshop\content\108600\3388017161 | BecomeDesensitizedB42                                                                                                                  | да       | уже было              |
| 3389605231  | G:\SteamLibrary\steamapps\workshop\content\108600\3389605231 | TchernoLib                                                                                                                             | да       | уже было              |
| 3390487814  | G:\SteamLibrary\steamapps\workshop\content\108600\3390487814 | DEON_CVG                                                                                                                               | да       | уже было              |
| 3392356751  | G:\SteamLibrary\steamapps\workshop\content\108600\3392356751 | WhatCanICraft_Addon                                                                                                                    | да       | уже было              |
| 3392745472  | G:\SteamLibrary\steamapps\workshop\content\108600\3392745472 | BoredomTweaks                                                                                                                          | да       | уже было              |
| 3395171770  | G:\SteamLibrary\steamapps\workshop\content\108600\3395171770 | moodlesinlua                                                                                                                           | да       | уже было              |
| 3396542795  | G:\SteamLibrary\steamapps\workshop\content\108600\3396542795 | DeonReloadingBench;DeonART_RFGP                                                                                                        | да       | уже было              |
| 3406392630  | G:\SteamLibrary\steamapps\workshop\content\108600\3406392630 | SKITTLE_LongTermPreservation                                                                                                           | да       | уже было              |
| 3410989950  | G:\SteamLibrary\steamapps\workshop\content\108600\3410989950 | TrueCrawl                                                                                                                              | да       | уже было              |
| 3423660713  | G:\SteamLibrary\steamapps\workshop\content\108600\3423660713 | ModLoadOrderSorter_b42                                                                                                                 | да       | уже было              |
| 3425287730  | G:\SteamLibrary\steamapps\workshop\content\108600\3425287730 | B42RainsFirearmsAndGunParts-RU                                                                                                         | да       | уже было              |
| 3429176285  | G:\SteamLibrary\steamapps\workshop\content\108600\3429176285 | campintherain_42.13;campintherain                                                                                                      | да       | уже было              |
| 3436499337  | G:\SteamLibrary\steamapps\workshop\content\108600\3436499337 | VMZNEW                                                                                                                                 | да       | уже было              |
| 3436537035  | G:\SteamLibrary\steamapps\workshop\content\108600\3436537035 | UsefulBarrels;UsefulBarrelsMP                                                                                                          | да       | да                    |
| 3437629766  | G:\SteamLibrary\steamapps\workshop\content\108600\3437629766 | CleanUI                                                                                                                                | да       | уже было              |
| 3455290347  | G:\SteamLibrary\steamapps\workshop\content\108600\3455290347 | PZB42RUTranslation                                                                                                                     | да       | да                    |
| 3461263912  | G:\SteamLibrary\steamapps\workshop\content\108600\3461263912 | CleanHotBar                                                                                                                            | да       | уже было              |
| 3495906499  | G:\SteamLibrary\steamapps\workshop\content\108600\3495906499 | SurvivalHUD                                                                                                                            | да       | уже было              |
| 3508537032  | G:\SteamLibrary\steamapps\workshop\content\108600\3508537032 | NeatUI_Framework                                                                                                                       | да       | уже было              |
| 3546314080  | G:\SteamLibrary\steamapps\workshop\content\108600\3546314080 | Waterpipes                                                                                                                             | да       | уже было              |
| 3567084868  | G:\SteamLibrary\steamapps\workshop\content\108600\3567084868 | ModManager                                                                                                                             | да       | уже было              |
| 3575895484  | G:\SteamLibrary\steamapps\workshop\content\108600\3575895484 | Ivmakk_CleanUIExtension                                                                                                                | да       | уже было              |
| 3591960030  | G:\SteamLibrary\steamapps\workshop\content\108600\3591960030 | INSWEARUS                                                                                                                              | да       | уже было              |
| 3597673472  | G:\SteamLibrary\steamapps\workshop\content\108600\3597673472 | LongTermPreservationExtended;LongTermPreservationExtendedUI                                                                            | да       | уже было              |
| 3610005735  | G:\SteamLibrary\steamapps\workshop\content\108600\3610005735 | AliceGear                                                                                                                              | да       | уже было              |
| 3617732907  | G:\SteamLibrary\steamapps\workshop\content\108600\3617732907 | ItemInspectionUI                                                                                                                       | да       | уже было              |
| 3624971238  | G:\SteamLibrary\steamapps\workshop\content\108600\3624971238 | YAPZLib                                                                                                                                | да       | уже было              |
| 3663239580  | G:\SteamLibrary\steamapps\workshop\content\108600\3663239580 | cleanblood                                                                                                                             | да       | уже было              |
| 3684808606  | G:\SteamLibrary\steamapps\workshop\content\108600\3684808606 | RepairWallCracks_B42                                                                                                                   | да       | уже было              |
| 3748865313  | G:\SteamLibrary\steamapps\workshop\content\108600\3748865313 | [B42] Project zomboid translate to Russian (by rennocki)                                                                               | да       | да                    |
