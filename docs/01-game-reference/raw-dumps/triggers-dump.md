---
description: A comprehensive list of all triggers.
sidebar_label: Trigger - Dump
---

# Trigger Dump

These are all of the triggers from the game's `.dat` files.

## Global Trigger Summary

:::info

Keys in `TRIGGER` are case-insensitive, but best practice is to always use **UPPERCASE** (e.g. `TRIGGER._GARAGE_SCHOOLGROUNDS`).

:::

|    # | Trigger Key                     | Lua Access                                 | Files                                                                                        |
| ---: | ------------------------------- | ------------------------------------------ | -------------------------------------------------------------------------------------------- |
|    1 | 1_01_BullyTrig                  | `TRIGGER._1_01_BULLYTRIG`                  | 1_01.dat                                                                                     |
|    2 | 1_01_CHECKOBJS1                 | `TRIGGER._1_01_CHECKOBJS1`                 | 1_01.dat                                                                                     |
|    3 | 1_01_FightTrigger               | `TRIGGER._1_01_FIGHTTRIGGER`               | 1_01.dat                                                                                     |
|    4 | 1_01_ParkDoor                   | `TRIGGER._1_01_PARKDOOR`                   | 1_01.dat                                                                                     |
|    5 | 1_01_PrincOffice                | `TRIGGER._1_01_PRINCOFFICE`                | 1_01.dat                                                                                     |
|    6 | 1_01_SchoolTrig                 | `TRIGGER._1_01_SCHOOLTRIG`                 | 1_01.dat                                                                                     |
|    7 | 1_02B_bathroom                  | `TRIGGER._1_02B_BATHROOM`                  | 1_02B.dat                                                                                    |
|    8 | 1_02B_cafeMessage               | `TRIGGER._1_02B_CAFEMESSAGE`               | 1_02B.dat                                                                                    |
|    9 | 1_02B_constTether               | `TRIGGER._1_02B_CONSTTETHER`               | 1_02B.dat                                                                                    |
|   10 | 1_02B_disablePOI                | `TRIGGER._1_02B_DISABLEPOI`                | 1_02B.dat                                                                                    |
|   11 | 1_02B_euniceKiss                | `TRIGGER._1_02B_EUNICEKISS`                | 1_02B.dat                                                                                    |
|   12 | 1_02B_excluderLocker            | `TRIGGER._1_02B_EXCLUDERLOCKER`            | 1_02B.dat                                                                                    |
|   13 | 1_02B_lockerMessage             | `TRIGGER._1_02B_LOCKERMESSAGE`             | 1_02B.dat                                                                                    |
|   14 | 1_02B_lockerMessage02           | `TRIGGER._1_02B_LOCKERMESSAGE02`           | 1_02B.dat                                                                                    |
|   15 | 1_02B_objCafe                   | `TRIGGER._1_02B_OBJCAFE`                   | 1_02B.dat                                                                                    |
|   16 | 1_02B_objLocker                 | `TRIGGER._1_02B_OBJLOCKER`                 | 1_02B.dat                                                                                    |
|   17 | 1_02B_objSocial                 | `TRIGGER._1_02B_OBJSOCIAL`                 | 1_02B.dat                                                                                    |
|   18 | 1_02B_recruitGary               | `TRIGGER._1_02B_RECRUITGARY`               | 1_02B.dat                                                                                    |
|   19 | 1_02B_socialMessage             | `TRIGGER._1_02B_SOCIALMESSAGE`             | 1_02B.dat                                                                                    |
|   20 | 1_02B_warn01                    | `TRIGGER._1_02B_WARN01`                    | 1_02B.dat                                                                                    |
|   21 | 1_02B_warn02                    | `TRIGGER._1_02B_WARN02`                    | 1_02B.dat                                                                                    |
|   22 | 1_02B_warn03                    | `TRIGGER._1_02B_WARN03`                    | 1_02B.dat                                                                                    |
|   23 | 1_02B_warn04                    | `TRIGGER._1_02B_WARN04`                    | 1_02B.dat                                                                                    |
|   24 | 1_02_FightArea                  | `TRIGGER._1_02_FIGHTAREA`                  | 1_02.dat                                                                                     |
|   25 | 1_02_PopulationTrig             | `TRIGGER._1_02_POPULATIONTRIG`             | 1_02.dat                                                                                     |
|   26 | 1_02_RusselTease                | `TRIGGER._1_02_RUSSELTEASE`                | 1_02.dat                                                                                     |
|   27 | 1_02_SchoolTrig                 | `TRIGGER._1_02_SCHOOLTRIG`                 | 1_02.dat                                                                                     |
|   28 | 1_02_TrainArea                  | `TRIGGER._1_02_TRAINAREA`                  | 1_02.dat                                                                                     |
|   29 | 1_03_AutoShopArea               | `TRIGGER._1_03_AUTOSHOPAREA`               | 1_03.dat                                                                                     |
|   30 | 1_03_DavisRegisterHit           | `TRIGGER._1_03_DAVISREGISTERHIT`           | 1_03.dat                                                                                     |
|   31 | 1_03_DavisRun                   | `TRIGGER._1_03_DAVISRUN`                   | 1_03.dat                                                                                     |
|   32 | 1_03_FailTrigger01              | `TRIGGER._1_03_FAILTRIGGER01`              | 1_03.dat                                                                                     |
|   33 | 1_03_FailTrigger02              | `TRIGGER._1_03_FAILTRIGGER02`              | 1_03.dat                                                                                     |
|   34 | 1_03_FalTrigger04               | `TRIGGER._1_03_FALTRIGGER04`               | 1_03.dat                                                                                     |
|   35 | 1_03_Fight1                     | `TRIGGER._1_03_FIGHT1`                     | 1_03.dat                                                                                     |
|   36 | 1_03_Fight3                     | `TRIGGER._1_03_FIGHT3`                     | 1_03.dat                                                                                     |
|   37 | 1_03_Fight4                     | `TRIGGER._1_03_FIGHT4`                     | 1_03.dat                                                                                     |
|   38 | 1_03_Fight5                     | `TRIGGER._1_03_FIGHT5`                     | 1_03.dat                                                                                     |
|   39 | 1_03_FrontGate                  | `TRIGGER._1_03_FRONTGATE`                  | 1_03.dat                                                                                     |
|   40 | 1_03_GameArea                   | `TRIGGER._1_03_GAMEAREA`                   | 1_03.dat                                                                                     |
|   41 | 1_03_Garage02                   | `TRIGGER._1_03_GARAGE02`                   | 1_03.dat                                                                                     |
|   42 | 1_03_Garage03                   | `TRIGGER._1_03_GARAGE03`                   | 1_03.dat                                                                                     |
|   43 | 1_03_GarbageCan02               | `TRIGGER._1_03_GARBAGECAN02`               | 1_03.dat                                                                                     |
|   44 | 1_03_GarbageCan05               | `TRIGGER._1_03_GARBAGECAN05`               | 1_03.dat                                                                                     |
|   45 | 1_03_GarbageCan06               | `TRIGGER._1_03_GARBAGECAN06`               | 1_03.dat                                                                                     |
|   46 | 1_03_GarbageCan07               | `TRIGGER._1_03_GARBAGECAN07`               | 1_03.dat                                                                                     |
|   47 | 1_03_JumpTut01                  | `TRIGGER._1_03_JUMPTUT01`                  | 1_03.dat                                                                                     |
|   48 | 1_03_KeepPedTrigger             | `TRIGGER._1_03_KEEPPEDTRIGGER`             | 1_03.dat                                                                                     |
|   49 | 1_03_Ladder_Drop                | `TRIGGER._1_03_LADDER_DROP`                | 1_03.dat                                                                                     |
|   50 | 1_03_PeterTrigger               | `TRIGGER._1_03_PETERTRIGGER`               | 1_03.dat                                                                                     |
|   51 | 1_03_SchoolYard                 | `TRIGGER._1_03_SCHOOLYARD`                 | 1_03.dat                                                                                     |
|   52 | 1_03_barelLad                   | `TRIGGER._1_03_BARELLAD`                   | 1_03.dat                                                                                     |
|   53 | 1_04_BottleNIS                  | `TRIGGER._1_04_BOTTLENIS`                  | 1_04.dat                                                                                     |
|   54 | 1_04_BottleShootArea            | `TRIGGER._1_04_BOTTLESHOOTAREA`            | 1_04.dat                                                                                     |
|   55 | 1_04_BottleZone                 | `TRIGGER._1_04_BOTTLEZONE`                 | 1_04.dat                                                                                     |
|   56 | 1_04_FieldTrig                  | `TRIGGER._1_04_FIELDTRIG`                  | 1_04.dat                                                                                     |
|   57 | 1_04_NemSitDown                 | `TRIGGER._1_04_NEMSITDOWN`                 | 1_04.dat                                                                                     |
|   58 | 1_04_Parking                    | `TRIGGER._1_04_PARKING`                    | 1_04.dat                                                                                     |
|   59 | 1_04_Soda_Nerd                  | `TRIGGER._1_04_SODA_NERD`                  | SodaNerd.dat                                                                                 |
|   60 | 1_04_SuppressFieldPop           | `TRIGGER._1_04_SUPPRESSFIELDPOP`           | 1_04.dat                                                                                     |
|   61 | 1_04_SuppressParkingPop         | `TRIGGER._1_04_SUPPRESSPARKINGPOP`         | 1_04.dat                                                                                     |
|   62 | 1_04_tree1_trig                 | `TRIGGER._1_04_TREE1_TRIG`                 | 1_04.dat                                                                                     |
|   63 | 1_04_tree2_trig                 | `TRIGGER._1_04_TREE2_TRIG`                 | 1_04.dat                                                                                     |
|   64 | 1_04_tree_sit                   | `TRIGGER._1_04_TREE_SIT`                   | 1_04.dat                                                                                     |
|   65 | 1_05B_algieLocker               | `TRIGGER._1_05B_ALGIELOCKER`               | 1_05b.dat                                                                                    |
|   66 | 1_05B_algieStall                | `TRIGGER._1_05B_ALGIESTALL`                | 1_05b.dat                                                                                    |
|   67 | 1_05B_areaSecondFloorBR         | `TRIGGER._1_05B_AREASECONDFLOORBR`         | 1_05b.dat                                                                                    |
|   68 | 1_05B_bathroomFirstFloor        | `TRIGGER._1_05B_BATHROOMFIRSTFLOOR`        | 1_05b.dat                                                                                    |
|   69 | 1_05B_bathroomSecondFloor       | `TRIGGER._1_05B_BATHROOMSECONDFLOOR`       | 1_05b.dat                                                                                    |
|   70 | 1_05B_firstFloorAmbientOff      | `TRIGGER._1_05B_FIRSTFLOORAMBIENTOFF`      | 1_05b.dat                                                                                    |
|   71 | 1_05B_firstFloorAmbientOn       | `TRIGGER._1_05B_FIRSTFLOORAMBIENTON`       | 1_05b.dat                                                                                    |
|   72 | 1_05B_firstFloorGirlsBR         | `TRIGGER._1_05B_FIRSTFLOORGIRLSBR`         | 1_05b.dat                                                                                    |
|   73 | 1_05B_loadSmoke                 | `TRIGGER._1_05B_LOADSMOKE`                 | 1_05b.dat                                                                                    |
|   74 | 1_05B_secondFloorGirlsBR        | `TRIGGER._1_05B_SECONDFLOORGIRLSBR`        | 1_05b.dat                                                                                    |
|   75 | 1_05_backDoorOff                | `TRIGGER._1_05_BACKDOOROFF`                | 1_05.dat                                                                                     |
|   76 | 1_05_frontDoorOff               | `TRIGGER._1_05_FRONTDOOROFF`               | 1_05.dat                                                                                     |
|   77 | 1_05_triggerJockPack            | `TRIGGER._1_05_TRIGGERJOCKPACK`            | 1_05.dat                                                                                     |
|   78 | 1_05_triggerJockPackWarning     | `TRIGGER._1_05_TRIGGERJOCKPACKWARNING`     | 1_05.dat                                                                                     |
|   79 | 1_05_triggerJocksNearFront      | `TRIGGER._1_05_TRIGGERJOCKSNEARFRONT`      | 1_05.dat                                                                                     |
|   80 | 1_05_triggerJocksNearLibrary    | `TRIGGER._1_05_TRIGGERJOCKSNEARLIBRARY`    | 1_05.dat                                                                                     |
|   81 | 1_07_BUCKY_BOUND                | `TRIGGER._1_07_BUCKY_BOUND`                | 1_07.dat                                                                                     |
|   82 | 1_07_FightTrigger               | `TRIGGER._1_07_FIGHTTRIGGER`               | 1_07.dat                                                                                     |
|   83 | 1_07_GateTrig                   | `TRIGGER._1_07_GATETRIG`                   | 1_07.dat                                                                                     |
|   84 | 1_07_Gate_T                     | `TRIGGER._1_07_GATE_T`                     | 1_07.dat                                                                                     |
|   85 | 1_07_Library_Door               | `TRIGGER._1_07_LIBRARY_DOOR`               | 1_07.dat                                                                                     |
|   86 | 1_07_NEAR_PARKING_LOT           | `TRIGGER._1_07_NEAR_PARKING_LOT`           | 1_07.dat                                                                                     |
|   87 | 1_07_NoAmbientPeds              | `TRIGGER._1_07_NOAMBIENTPEDS`              | 1_07.dat                                                                                     |
|   88 | 1_07_SpawnZone                  | `TRIGGER._1_07_SPAWNZONE`                  | 1_07.dat                                                                                     |
|   89 | 1_07_Spawner01                  | `TRIGGER._1_07_SPAWNER01`                  | 1_07.dat                                                                                     |
|   90 | 1_07_Spawner02                  | `TRIGGER._1_07_SPAWNER02`                  | 1_07.dat                                                                                     |
|   91 | 1_07_Spawner03                  | `TRIGGER._1_07_SPAWNER03`                  | 1_07.dat                                                                                     |
|   92 | 1_07_Spawner04                  | `TRIGGER._1_07_SPAWNER04`                  | 1_07.dat                                                                                     |
|   93 | 1_07_Spawner05                  | `TRIGGER._1_07_SPAWNER05`                  | 1_07.dat                                                                                     |
|   94 | 1_07_Spawner06                  | `TRIGGER._1_07_SPAWNER06`                  | 1_07.dat                                                                                     |
|   95 | 1_07_ToolBox01                  | `TRIGGER._1_07_TOOLBOX01`                  | 1_07.dat                                                                                     |
|   96 | 1_08_BathroomLocker             | `TRIGGER._1_08_BATHROOMLOCKER`             | 1_08.dat                                                                                     |
|   97 | 1_08_CafTrig                    | `TRIGGER._1_08_CAFTRIG`                    | 1_08.dat                                                                                     |
|   98 | 1_08_GYMGIRLWASH                | `TRIGGER._1_08_GYMGIRLWASH`                | 1_08.dat                                                                                     |
|   99 | 1_08_JimmyLeft                  | `TRIGGER._1_08_JIMMYLEFT`                  | 1_08.dat                                                                                     |
|  100 | 1_09_AisleLeft                  | `TRIGGER._1_09_AISLELEFT`                  | 1_09.dat                                                                                     |
|  101 | 1_09_AisleRight                 | `TRIGGER._1_09_AISLERIGHT`                 | 1_09.dat                                                                                     |
|  102 | 1_09_BoxLeft1                   | `TRIGGER._1_09_BOXLEFT1`                   | 1_09.dat                                                                                     |
|  103 | 1_09_BoxLeft2                   | `TRIGGER._1_09_BOXLEFT2`                   | 1_09.dat                                                                                     |
|  104 | 1_09_BoxRight1                  | `TRIGGER._1_09_BOXRIGHT1`                  | 1_09.dat                                                                                     |
|  105 | 1_09_BoxRight2                  | `TRIGGER._1_09_BOXRIGHT2`                  | 1_09.dat                                                                                     |
|  106 | 1_09_Catwalk1                   | `TRIGGER._1_09_CATWALK1`                   | 1_09.dat                                                                                     |
|  107 | 1_09_StageLeft                  | `TRIGGER._1_09_STAGELEFT`                  | 1_09.dat                                                                                     |
|  108 | 1_09_StageRight                 | `TRIGGER._1_09_STAGERIGHT`                 | 1_09.dat                                                                                     |
|  109 | 1_10_BasementDoor               | `TRIGGER._1_10_BASEMENTDOOR`               | 1_10.dat                                                                                     |
|  110 | 1_10_BullyTrigger               | `TRIGGER._1_10_BULLYTRIGGER`               | 1_10.dat                                                                                     |
|  111 | 1_10_CrouchHint                 | `TRIGGER._1_10_CROUCHHINT`                 | 1_10.dat                                                                                     |
|  112 | 1_10_GARY_TURN_OFF_ELEC         | `TRIGGER._1_10_GARY_TURN_OFF_ELEC`         | 1_10.dat                                                                                     |
|  113 | 1_10_InCage                     | `TRIGGER._1_10_INCAGE`                     | 1_10.dat                                                                                     |
|  114 | 1_10_NearHole                   | `TRIGGER._1_10_NEARHOLE`                   | 1_10.dat                                                                                     |
|  115 | 1_10_Near_BasementDoor          | `TRIGGER._1_10_NEAR_BASEMENTDOOR`          | 1_10.dat                                                                                     |
|  116 | 1_10_TheHole                    | `TRIGGER._1_10_THEHOLE`                    | 1_10.dat                                                                                     |
|  117 | 1_10_almost_complete            | `TRIGGER._1_10_ALMOST_COMPLETE`            | 1_10.dat                                                                                     |
|  118 | 1_10_atFurnace                  | `TRIGGER._1_10_ATFURNACE`                  | 1_10.dat                                                                                     |
|  119 | 1_10_aud_2                      | `TRIGGER._1_10_AUD_2`                      | 1_10.dat                                                                                     |
|  120 | 1_10_crawl_elec                 | `TRIGGER._1_10_CRAWL_ELEC`                 | 1_10.dat                                                                                     |
|  121 | 1_10_exit_cage                  | `TRIGGER._1_10_EXIT_CAGE`                  | 1_10.dat                                                                                     |
|  122 | 1_10_ring_peds                  | `TRIGGER._1_10_RING_PEDS`                  | 1_10.dat                                                                                     |
|  123 | 1_10_room0                      | `TRIGGER._1_10_ROOM0`                      | 1_10.dat                                                                                     |
|  124 | 1_10_room1                      | `TRIGGER._1_10_ROOM1`                      | 1_10.dat                                                                                     |
|  125 | 1_10_room2                      | `TRIGGER._1_10_ROOM2`                      | 1_10.dat                                                                                     |
|  126 | 1_10_room3                      | `TRIGGER._1_10_ROOM3`                      | 1_10.dat                                                                                     |
|  127 | 1_10_room4                      | `TRIGGER._1_10_ROOM4`                      | 1_10.dat                                                                                     |
|  128 | 1_11X1_bullies                  | `TRIGGER._1_11X1_BULLIES`                  | 1_11x1.dat                                                                                   |
|  129 | 1_11X1_outside                  | `TRIGGER._1_11X1_OUTSIDE`                  | 1_11x1.dat                                                                                   |
|  130 | 1_11X1_pete                     | `TRIGGER._1_11X1_PETE`                     | 1_11x1.dat                                                                                   |
|  131 | 1_11x2_chadAttack               | `TRIGGER._1_11X2_CHADATTACK`               | 1_11x2.dat                                                                                   |
|  132 | 1_11x2_garden                   | `TRIGGER._1_11X2_GARDEN`                   | 1_11x2.dat                                                                                   |
|  133 | 1_11x2_shitTarget               | `TRIGGER._1_11X2_SHITTARGET`               | 1_11x2.dat                                                                                   |
|  134 | 1_11xp_DeadRat                  | `TRIGGER._1_11XP_DEADRAT`                  | 1_11xp.dat                                                                                   |
|  135 | 1_11xp_F4000                    | `TRIGGER._1_11XP_F4000`                    | 1_11xp.dat                                                                                   |
|  136 | 1_11xp_Firecracker              | `TRIGGER._1_11XP_FIRECRACKER`              | 1_11xp.dat                                                                                   |
|  137 | 1_11xp_ItchPowder               | `TRIGGER._1_11XP_ITCHPOWDER`               | 1_11xp.dat                                                                                   |
|  138 | 1_11xp_JokeCandy                | `TRIGGER._1_11XP_JOKECANDY`                | 1_11xp.dat                                                                                   |
|  139 | 1_11xp_KickMe                   | `TRIGGER._1_11XP_KICKME`                   | 1_11xp.dat                                                                                   |
|  140 | 1_11xp_Marbles                  | `TRIGGER._1_11XP_MARBLES`                  | 1_11xp.dat                                                                                   |
|  141 | 1_11xp_StinkBomb                | `TRIGGER._1_11XP_STINKBOMB`                | 1_11xp.dat                                                                                   |
|  142 | 1_G1_BeatriceWarning            | `TRIGGER._1_G1_BEATRICEWARNING`            | 1_G1_new.dat                                                                                 |
|  143 | 1_G1_MathProxy                  | `TRIGGER._1_G1_MATHPROXY`                  | 1_G1_new.dat                                                                                 |
|  144 | 1_G1_StaffProxy                 | `TRIGGER._1_G1_STAFFPROXY`                 | 1_G1_new.dat                                                                                 |
|  145 | 1_S01_Bathroom                  | `TRIGGER._1_S01_BATHROOM`                  | 1_S01.dat                                                                                    |
|  146 | 1_S01_BathroomSetup             | `TRIGGER._1_S01_BATHROOMSETUP`             | 1_S01.dat                                                                                    |
|  147 | 1_S01_Bottle_Trig_Bath          | `TRIGGER._1_S01_BOTTLE_TRIG_BATH`          | 1_S01.dat                                                                                    |
|  148 | 1_S01_Bottle_Trig_Cafe          | `TRIGGER._1_S01_BOTTLE_TRIG_CAFE`          | 1_S01.dat                                                                                    |
|  149 | 1_S01_Bottle_Trig_Case          | `TRIGGER._1_S01_BOTTLE_TRIG_CASE`          | 1_S01.dat                                                                                    |
|  150 | 1_S01_Cafe                      | `TRIGGER._1_S01_CAFE`                      | 1_S01.dat                                                                                    |
|  151 | 1_S01_Create_Edna               | `TRIGGER._1_S01_CREATE_EDNA`               | 1_S01.dat                                                                                    |
|  152 | 1_S01_Glass                     | `TRIGGER._1_S01_GLASS`                     | 1_S01.dat                                                                                    |
|  153 | 1_S01_HattrickDelete            | `TRIGGER._1_S01_HATTRICKDELETE`            | 1_S01.dat                                                                                    |
|  154 | 1_S01_Kitchen                   | `TRIGGER._1_S01_KITCHEN`                   | 1_S01.dat                                                                                    |
|  155 | 1_S01_Phillips_Return           | `TRIGGER._1_S01_PHILLIPS_RETURN`           | 1_S01.dat                                                                                    |
|  156 | 1_S01_PlayerBlocking            | `TRIGGER._1_S01_PLAYERBLOCKING`            | 1_S01.dat                                                                                    |
|  157 | 1_S01_Prefect1                  | `TRIGGER._1_S01_PREFECT1`                  | 1_S01.dat                                                                                    |
|  158 | 1_S01_Prefect_8_1_Spawn         | `TRIGGER._1_S01_PREFECT_8_1_SPAWN`         | 1_S01.dat                                                                                    |
|  159 | 1_S01_Prefect_Running1          | `TRIGGER._1_S01_PREFECT_RUNNING1`          | 1_S01.dat                                                                                    |
|  160 | 1_S01_Prefect_Running1_Delete   | `TRIGGER._1_S01_PREFECT_RUNNING1_DELETE`   | 1_S01.dat                                                                                    |
|  161 | 1_S01_TrophySetup               | `TRIGGER._1_S01_TROPHYSETUP`               | 1_S01.dat                                                                                    |
|  162 | 1_g1_Locker                     | `TRIGGER._1_G1_LOCKER`                     | 1_G1_new.dat                                                                                 |
|  163 | 2_01_EdnaFacePlayer             | `TRIGGER._2_01_EDNAFACEPLAYER`             | 2_01.dat                                                                                     |
|  164 | 2_01_GreaserTrig                | `TRIGGER._2_01_GREASERTRIG`                | 2_01.dat                                                                                     |
|  165 | 2_01_GreaserTrig2               | `TRIGGER._2_01_GREASERTRIG2`               | 2_01.dat                                                                                     |
|  166 | 2_01_MOUNTBIKE                  | `TRIGGER._2_01_MOUNTBIKE`                  | 2_01.dat                                                                                     |
|  167 | 2_01_PreppyTrig                 | `TRIGGER._2_01_PREPPYTRIG`                 | 2_01.dat                                                                                     |
|  168 | 2_01_PreppyTrig2                | `TRIGGER._2_01_PREPPYTRIG2`                | 2_01.dat                                                                                     |
|  169 | 2_01_StartCopfight              | `TRIGGER._2_01_STARTCOPFIGHT`              | 2_01.dat                                                                                     |
|  170 | 2_01_TutPlay1                   | `TRIGGER._2_01_TUTPLAY1`                   | 2_01.dat                                                                                     |
|  171 | 2_01_tutOff                     | `TRIGGER._2_01_TUTOFF`                     | 2_01.dat                                                                                     |
|  172 | 2_01_tutOff2                    | `TRIGGER._2_01_TUTOFF2`                    | 2_01.dat                                                                                     |
|  173 | 2_02_returnComic                | `TRIGGER._2_02_RETURNCOMIC`                | 2_02.dat                                                                                     |
|  174 | 2_02_schoolParking              | `TRIGGER._2_02_SCHOOLPARKING`              | 2_02.dat                                                                                     |
|  175 | 2_03_BRTadTrigger               | `TRIGGER._2_03_BRTADTRIGGER`               | 2_03.dat                                                                                     |
|  176 | 2_03_Back_Gate                  | `TRIGGER._2_03_BACK_GATE`                  | 2_03.dat                                                                                     |
|  177 | 2_03_Back_Unlock                | `TRIGGER._2_03_BACK_UNLOCK`                | 2_03.dat                                                                                     |
|  178 | 2_03_Backyard                   | `TRIGGER._2_03_BACKYARD`                   | 2_03.dat                                                                                     |
|  179 | 2_03_FrontDoorTrigger           | `TRIGGER._2_03_FRONTDOORTRIGGER`           | 2_03.dat                                                                                     |
|  180 | 2_03_FrontGateArea              | `TRIGGER._2_03_FRONTGATEAREA`              | 2_03.dat                                                                                     |
|  181 | 2_03_FrontYard                  | `TRIGGER._2_03_FRONTYARD`                  | 2_03.dat                                                                                     |
|  182 | 2_03_Front_Unlock               | `TRIGGER._2_03_FRONT_UNLOCK`               | 2_03.dat                                                                                     |
|  183 | 2_03_RearDoorTrigger            | `TRIGGER._2_03_REARDOORTRIGGER`            | 2_03.dat                                                                                     |
|  184 | 2_03_RearGateArea               | `TRIGGER._2_03_REARGATEAREA`               | 2_03.dat                                                                                     |
|  185 | 2_03_TadHouse                   | `TRIGGER._2_03_TADHOUSE`                   | 2_03.dat                                                                                     |
|  186 | 2_03_TadNIS                     | `TRIGGER._2_03_TADNIS`                     | 2_03.dat                                                                                     |
|  187 | 2_03_TadsBlock                  | `TRIGGER._2_03_TADSBLOCK`                  | 2_03.dat                                                                                     |
|  188 | 2_04_BarrelFire01               | `TRIGGER._2_04_BARRELFIRE01`               | 2_04.dat                                                                                     |
|  189 | 2_04_BarrelFire02               | `TRIGGER._2_04_BARRELFIRE02`               | 2_04.dat                                                                                     |
|  190 | 2_04_BarrelFire03               | `TRIGGER._2_04_BARRELFIRE03`               | 2_04.dat                                                                                     |
|  191 | 2_04_BarrelFire04               | `TRIGGER._2_04_BARRELFIRE04`               | 2_04.dat                                                                                     |
|  192 | 2_04_BarrelFire05               | `TRIGGER._2_04_BARRELFIRE05`               | 2_04.dat                                                                                     |
|  193 | 2_04_BarrelFire06               | `TRIGGER._2_04_BARRELFIRE06`               | 2_04.dat                                                                                     |
|  194 | 2_04_CHEATER_1_ZONE             | `TRIGGER._2_04_CHEATER_1_ZONE`             | 2_04_Bus.dat                                                                                 |
|  195 | 2_04_CHEATER_2_ZONE             | `TRIGGER._2_04_CHEATER_2_ZONE`             | 2_04_Bus.dat                                                                                 |
|  196 | 2_04_CHEATER_3_ZONE             | `TRIGGER._2_04_CHEATER_3_ZONE`             | 2_04_Bus.dat                                                                                 |
|  197 | 2_04_CHEATER_4_ZONE             | `TRIGGER._2_04_CHEATER_4_ZONE`             | 2_04_Bus.dat                                                                                 |
|  198 | 2_04_ChangeBeach                | `TRIGGER._2_04_CHANGEBEACH`                | 2_04.dat                                                                                     |
|  199 | 2_04_DormDoor                   | `TRIGGER._2_04_DORMDOOR`                   | 2_04.dat                                                                                     |
|  200 | 2_04_TireFire01b                | `TRIGGER._2_04_TIREFIRE01B`                | 2_04.dat                                                                                     |
|  201 | 2_04_TireFire02b                | `TRIGGER._2_04_TIREFIRE02B`                | 2_04.dat                                                                                     |
|  202 | 2_04_TireFire03b                | `TRIGGER._2_04_TIREFIRE03B`                | 2_04.dat                                                                                     |
|  203 | 2_05_BACKGATE                   | `TRIGGER._2_05_BACKGATE`                   | 2_05_new.dat                                                                                 |
|  204 | 2_05_EggStashArea               | `TRIGGER._2_05_EGGSTASHAREA`               | 2_05_new.dat                                                                                 |
|  205 | 2_05_FRONTGATE                  | `TRIGGER._2_05_FRONTGATE`                  | 2_05_new.dat                                                                                 |
|  206 | 2_05_FrontExit                  | `TRIGGER._2_05_FRONTEXIT`                  | 2_05_new.dat                                                                                 |
|  207 | 2_05_RecruitRussell             | `TRIGGER._2_05_RECRUITRUSSELL`             | 2_05_new.dat                                                                                 |
|  208 | 2_05_RichArea                   | `TRIGGER._2_05_RICHAREA`                   | 2_05_new.dat                                                                                 |
|  209 | 2_05_Room1                      | `TRIGGER._2_05_ROOM1`                      | 2_05_new.dat                                                                                 |
|  210 | 2_05_Room2                      | `TRIGGER._2_05_ROOM2`                      | 2_05_new.dat                                                                                 |
|  211 | 2_05_Room3                      | `TRIGGER._2_05_ROOM3`                      | 2_05_new.dat                                                                                 |
|  212 | 2_05_Room4                      | `TRIGGER._2_05_ROOM4`                      | 2_05_new.dat                                                                                 |
|  213 | 2_05_Room5                      | `TRIGGER._2_05_ROOM5`                      | 2_05_new.dat                                                                                 |
|  214 | 2_05_Room6                      | `TRIGGER._2_05_ROOM6`                      | 2_05_new.dat                                                                                 |
|  215 | 2_05_RussellOffBike             | `TRIGGER._2_05_RUSSELLOFFBIKE`             | 2_05_new.dat                                                                                 |
|  216 | 2_05_TadsBlock                  | `TRIGGER._2_05_TADSBLOCK`                  | 2_05_new.dat                                                                                 |
|  217 | 2_05_TadsYard                   | `TRIGGER._2_05_TADSYARD`                   | 2_05_new.dat                                                                                 |
|  218 | 2_05_Tree01                     | `TRIGGER._2_05_TREE01`                     | 2_05_new.dat                                                                                 |
|  219 | 2_05_Tree02                     | `TRIGGER._2_05_TREE02`                     | 2_05_new.dat                                                                                 |
|  220 | 2_05_WallBreak01                | `TRIGGER._2_05_WALLBREAK01`                | 2_05_new.dat                                                                                 |
|  221 | 2_05_WallBreak02                | `TRIGGER._2_05_WALLBREAK02`                | 2_05_new.dat                                                                                 |
|  222 | 2_06_BikeZone                   | `TRIGGER._2_06_BIKEZONE`                   | 2_06.dat                                                                                     |
|  223 | 2_06_Theater                    | `TRIGGER._2_06_THEATER`                    | 2_06.dat                                                                                     |
|  224 | 2_07_GORD_ON_DOCK               | `TRIGGER._2_07_GORD_ON_DOCK`               | 2_07_BeachA.dat                                                                              |
|  225 | 2_07_OUTSIDEDOOR                | `TRIGGER._2_07_OUTSIDEDOOR`                | 2_07_BeachA.dat                                                                              |
|  226 | 2_07_OUT_OF_AREA                | `TRIGGER._2_07_OUT_OF_AREA`                | 2_07_BeachA.dat                                                                              |
|  227 | 2_07_OUT_OF_AREA_WARN           | `TRIGGER._2_07_OUT_OF_AREA_WARN`           | 2_07_BeachA.dat                                                                              |
|  228 | 2_07_PREPPY_NINJA_TRIG          | `TRIGGER._2_07_PREPPY_NINJA_TRIG`          | 2_07_BeachA.dat                                                                              |
|  229 | 2_07_REAR_PIER                  | `TRIGGER._2_07_REAR_PIER`                  | 2_07_BeachA.dat                                                                              |
|  230 | 2_07_behindDoor                 | `TRIGGER._2_07_BEHINDDOOR`                 | 2_07_BeachA.dat                                                                              |
|  231 | 2_08_BifAttackTrig              | `TRIGGER._2_08_BIFATTACKTRIG`              | 2_08.dat                                                                                     |
|  232 | 2_08_DoorStairs                 | `TRIGGER._2_08_DOORSTAIRS`                 | 2_08.dat                                                                                     |
|  233 | 2_08_FirstFloorTrig             | `TRIGGER._2_08_FIRSTFLOORTRIG`             | 2_08.dat                                                                                     |
|  234 | 2_08_FoyeurDoor                 | `TRIGGER._2_08_FOYEURDOOR`                 | 2_08.dat                                                                                     |
|  235 | 2_08_PlantTarget                | `TRIGGER._2_08_PLANTTARGET`                | 2_08.dat                                                                                     |
|  236 | 2_08_SecndFloorTrig             | `TRIGGER._2_08_SECNDFLOORTRIG`             | 2_08.dat                                                                                     |
|  237 | 2_08_SolariumEntrance           | `TRIGGER._2_08_SOLARIUMENTRANCE`           | 2_08.dat                                                                                     |
|  238 | 2_08_StairPreppy                | `TRIGGER._2_08_STAIRPREPPY`                | 2_08.dat                                                                                     |
|  239 | 2_08_ThrdFloorTrig              | `TRIGGER._2_08_THRDFLOORTRIG`              | 2_08.dat                                                                                     |
|  240 | 2_08_ToSolarium                 | `TRIGGER._2_08_TOSOLARIUM`                 | 2_08.dat                                                                                     |
|  241 | 2_08_TriggerStairs              | `TRIGGER._2_08_TRIGGERSTAIRS`              | 2_08.dat                                                                                     |
|  242 | 2_B_BOSS_FIGHT                  | `TRIGGER._2_B_BOSS_FIGHT`                  | 2_B.dat                                                                                      |
|  243 | 2_B_BOSS_FIGHT_INTRO            | `TRIGGER._2_B_BOSS_FIGHT_INTRO`            | 2_B.dat                                                                                      |
|  244 | 2_B_DRBRACE_DOOR                | `TRIGGER._2_B_DRBRACE_DOOR`                | 2_B.dat                                                                                      |
|  245 | 2_B_DRBRACE_DOOR01              | `TRIGGER._2_B_DRBRACE_DOOR01`              | 2_B.dat                                                                                      |
|  246 | 2_B_PLAYER_NEAR_BAR             | `TRIGGER._2_B_PLAYER_NEAR_BAR`             | 2_B.dat                                                                                      |
|  247 | 2_B_SECOND_ATTACK               | `TRIGGER._2_B_SECOND_ATTACK`               | 2_B.dat                                                                                      |
|  248 | 2_B_Tether                      | `TRIGGER._2_B_TETHER`                      | 2_B.dat                                                                                      |
|  249 | 2_G2_ballToss                   | `TRIGGER._2_G2_BALLTOSS`                   | 2_G2.dat                                                                                     |
|  250 | 2_G2_ballTossExcluderInside     | `TRIGGER._2_G2_BALLTOSSEXCLUDERINSIDE`     | Global.dat                                                                                   |
|  251 | 2_G2_ballTossExcluderOutside    | `TRIGGER._2_G2_BALLTOSSEXCLUDEROUTSIDE`    | Global.dat                                                                                   |
|  252 | 2_G2_dunkExcluderOutside        | `TRIGGER._2_G2_DUNKEXCLUDEROUTSIDE`        | Global.dat                                                                                   |
|  253 | 2_G2_dunkTank                   | `TRIGGER._2_G2_DUNKTANK`                   | 2_G2.dat                                                                                     |
|  254 | 2_G2_excluderCoaster            | `TRIGGER._2_G2_EXCLUDERCOASTER`            | 2_G2.dat                                                                                     |
|  255 | 2_G2_excluderFerris             | `TRIGGER._2_G2_EXCLUDERFERRIS`             | 2_G2.dat                                                                                     |
|  256 | 2_G2_excluderSquid              | `TRIGGER._2_G2_EXCLUDERSQUID`              | 2_G2.dat                                                                                     |
|  257 | 2_G2_freakShow                  | `TRIGGER._2_G2_FREAKSHOW`                  | 2_G2.dat                                                                                     |
|  258 | 2_G2_highStriker                | `TRIGGER._2_G2_HIGHSTRIKER`                | 2_G2.dat                                                                                     |
|  259 | 2_G2_pinkyAngryFail             | `TRIGGER._2_G2_PINKYANGRYFAIL`             | 2_G2.dat                                                                                     |
|  260 | 2_G2_pinkyArrived               | `TRIGGER._2_G2_PINKYARRIVED`               | 2_G2.dat                                                                                     |
|  261 | 2_G2_shootingExcluderInside     | `TRIGGER._2_G2_SHOOTINGEXCLUDERINSIDE`     | Global.dat                                                                                   |
|  262 | 2_G2_shootingExcluderOutside    | `TRIGGER._2_G2_SHOOTINGEXCLUDEROUTSIDE`    | Global.dat                                                                                   |
|  263 | 2_G2_shootingGallery            | `TRIGGER._2_G2_SHOOTINGGALLERY`            | 2_G2.dat                                                                                     |
|  264 | 2_G2_ticketShop                 | `TRIGGER._2_G2_TICKETSHOP`                 | 2_G2.dat                                                                                     |
|  265 | 2_S02CarSpeedup                 | `TRIGGER._2_S02CARSPEEDUP`                 | 2_S02.dat                                                                                    |
|  266 | 2_S02_CarFailTrigger            | `TRIGGER._2_S02_CARFAILTRIGGER`            | 2_S02.dat                                                                                    |
|  267 | 2_S02_CarInDriveway             | `TRIGGER._2_S02_CARINDRIVEWAY`             | 2_S02.dat                                                                                    |
|  268 | 2_S02_CarInit                   | `TRIGGER._2_S02_CARINIT`                   | 2_S02.dat                                                                                    |
|  269 | 2_S02_CarTrigger                | `TRIGGER._2_S02_CARTRIGGER`                | 2_S02.dat                                                                                    |
|  270 | 2_S02_Cop1                      | `TRIGGER._2_S02_COP1`                      | 2_S02.dat                                                                                    |
|  271 | 2_S02_Cop_Car1_Stop             | `TRIGGER._2_S02_COP_CAR1_STOP`             | 2_S02.dat                                                                                    |
|  272 | 2_S02_Cop_Car2_Stop             | `TRIGGER._2_S02_COP_CAR2_STOP`             | 2_S02.dat                                                                                    |
|  273 | 2_S02_End_Trigger1              | `TRIGGER._2_S02_END_TRIGGER1`              | 2_S02.dat                                                                                    |
|  274 | 2_S02_HATTRICKYARD              | `TRIGGER._2_S02_HATTRICKYARD`              | 2_S02.dat                                                                                    |
|  275 | 2_S02_HattrickNIS               | `TRIGGER._2_S02_HATTRICKNIS`               | 2_S02.dat                                                                                    |
|  276 | 2_S02_Intro_Failure             | `TRIGGER._2_S02_INTRO_FAILURE`             | 2_S02.dat                                                                                    |
|  277 | 2_S02_PathVolume                | `TRIGGER._2_S02_PATHVOLUME`                | 2_S02.dat                                                                                    |
|  278 | 2_S04Sheet3NIS                  | `TRIGGER._2_S04SHEET3NIS`                  | 2_S04.dat                                                                                    |
|  279 | 2_S04_AutoShopArea              | `TRIGGER._2_S04_AUTOSHOPAREA`              | 2_S04.dat                                                                                    |
|  280 | 2_S04_LibraryJump               | `TRIGGER._2_S04_LIBRARYJUMP`               | 2_S04.dat                                                                                    |
|  281 | 2_S04_Nerd_Escape               | `TRIGGER._2_S04_NERD_ESCAPE`               | 2_S04.dat                                                                                    |
|  282 | 2_S04_SchoolPop                 | `TRIGGER._2_S04_SCHOOLPOP`                 | 2_S04.dat                                                                                    |
|  283 | 2_S04_Sheet1                    | `TRIGGER._2_S04_SHEET1`                    | 2_S04.dat                                                                                    |
|  284 | 2_S04_Sheet2                    | `TRIGGER._2_S04_SHEET2`                    | 2_S04.dat                                                                                    |
|  285 | 2_S04_Sheet3                    | `TRIGGER._2_S04_SHEET3`                    | 2_S04.dat                                                                                    |
|  286 | 2_S04_Sheet3Create              | `TRIGGER._2_S04_SHEET3CREATE`              | 2_S04.dat                                                                                    |
|  287 | 2_S04_Sheet3Outer               | `TRIGGER._2_S04_SHEET3OUTER`               | 2_S04.dat                                                                                    |
|  288 | 2_S04_Sheet4                    | `TRIGGER._2_S04_SHEET4`                    | 2_S04.dat                                                                                    |
|  289 | 2_S04_Sheet4Inner               | `TRIGGER._2_S04_SHEET4INNER`               | 2_S04.dat                                                                                    |
|  290 | 2_S04_Sheet5E1                  | `TRIGGER._2_S04_SHEET5E1`                  | 2_S04.dat                                                                                    |
|  291 | 2_S04_Sheet5E2                  | `TRIGGER._2_S04_SHEET5E2`                  | 2_S04.dat                                                                                    |
|  292 | 2_S04_Sheet5Start               | `TRIGGER._2_S04_SHEET5START`               | 2_S04.dat                                                                                    |
|  293 | 2_S04_StartSheet2               | `TRIGGER._2_S04_STARTSHEET2`               | 2_S04.dat                                                                                    |
|  294 | 2_S04_TetherBully               | `TRIGGER._2_S04_TETHERBULLY`               | 2_S04.dat                                                                                    |
|  295 | 2_S04_TrashCan                  | `TRIGGER._2_S04_TRASHCAN`                  | 2_S04.dat                                                                                    |
|  296 | 2_S05_AwfulHack                 | `TRIGGER._2_S05_AWFULHACK`                 | 2_S05.dat                                                                                    |
|  297 | 2_S05_DisturbRadius             | `TRIGGER._2_S05_DISTURBRADIUS`             | 2_S05.dat                                                                                    |
|  298 | 2_S05_DrugAlley                 | `TRIGGER._2_S05_DRUGALLEY`                 | 2_S05.dat                                                                                    |
|  299 | 2_S05_Excluder                  | `TRIGGER._2_S05_EXCLUDER`                  | 2_S05.dat                                                                                    |
|  300 | 2_S05_Target                    | `TRIGGER._2_S05_TARGET`                    | 2_S05.dat                                                                                    |
|  301 | 2_S05_TeacherArea               | `TRIGGER._2_S05_TEACHERAREA`               | 2_S05.dat                                                                                    |
|  302 | 2_S05_TeacherRadius             | `TRIGGER._2_S05_TEACHERRADIUS`             | 2_S05.dat                                                                                    |
|  303 | 2_S05_TrashCan1                 | `TRIGGER._2_S05_TRASHCAN1`                 | 2_S05.dat                                                                                    |
|  304 | 2_S05_TrashCan2                 | `TRIGGER._2_S05_TRASHCAN2`                 | 2_S05.dat                                                                                    |
|  305 | 2_S05_TrashCan3                 | `TRIGGER._2_S05_TRASHCAN3`                 | 2_S05.dat                                                                                    |
|  306 | 2_S05_Tree                      | `TRIGGER._2_S05_TREE`                      | 2_S05.dat                                                                                    |
|  307 | 2_S05_Tree2                     | `TRIGGER._2_S05_TREE2`                     | 2_S05.dat                                                                                    |
|  308 | 2_S06B_AngieChristyRoom         | `TRIGGER._2_S06B_ANGIECHRISTYROOM`         | 2_S06b.dat                                                                                   |
|  309 | 2_S06B_EuniceFrontDoor          | `TRIGGER._2_S06B_EUNICEFRONTDOOR`          | 2_S06b.dat                                                                                   |
|  310 | 2_S06B_MandyRoom                | `TRIGGER._2_S06B_MANDYROOM`                | 2_S06b.dat                                                                                   |
|  311 | 2_S06B_atticEntry               | `TRIGGER._2_S06B_ATTICENTRY`               | 2_S06b.dat                                                                                   |
|  312 | 2_S06B_launchAsian              | `TRIGGER._2_S06B_LAUNCHASIAN`              | 2_S06b.dat                                                                                   |
|  313 | 2_S06B_makeGirlsStudy           | `TRIGGER._2_S06B_MAKEGIRLSSTUDY`           | 2_S06b.dat                                                                                   |
|  314 | 2_S06B_pinkyRoom                | `TRIGGER._2_S06B_PINKYROOM`                | 2_S06b.dat                                                                                   |
|  315 | 2_S06B_showerWarn               | `TRIGGER._2_S06B_SHOWERWARN`               | 2_S06b.dat                                                                                   |
|  316 | 2_S06B_trigger01                | `TRIGGER._2_S06B_TRIGGER01`                | 2_S06b.dat                                                                                   |
|  317 | 2_S06B_trigger02                | `TRIGGER._2_S06B_TRIGGER02`                | 2_S06b.dat                                                                                   |
|  318 | 2_S06B_trigger03                | `TRIGGER._2_S06B_TRIGGER03`                | 2_S06b.dat                                                                                   |
|  319 | 2_S06B_triggerShowerDialogue    | `TRIGGER._2_S06B_TRIGGERSHOWERDIALOGUE`    | 2_S06b.dat                                                                                   |
|  320 | 2_S06B_upstairsHallway          | `TRIGGER._2_S06B_UPSTAIRSHALLWAY`          | 2_S06b.dat                                                                                   |
|  321 | 2_S06_PrefectWander             | `TRIGGER._2_S06_PREFECTWANDER`             | 2_S06.dat                                                                                    |
|  322 | 2_S06_latticeCam                | `TRIGGER._2_S06_LATTICECAM`                | 2_S06.dat                                                                                    |
|  323 | 2_S06_mandySpeak                | `TRIGGER._2_S06_MANDYSPEAK`                | 2_S06.dat                                                                                    |
|  324 | 2_S06_stg1Burton                | `TRIGGER._2_S06_STG1BURTON`                | 2_S06.dat                                                                                    |
|  325 | 2_S06_stg1_Busted               | `TRIGGER._2_S06_STG1_BUSTED`               | 2_S06.dat                                                                                    |
|  326 | 2_S06_stg3Burton                | `TRIGGER._2_S06_STG3BURTON`                | 2_S06.dat                                                                                    |
|  327 | 2_S06_stg3LeftDorm              | `TRIGGER._2_S06_STG3LEFTDORM`              | 2_S06.dat                                                                                    |
|  328 | 2_S06_triggerLoadSchool         | `TRIGGER._2_S06_TRIGGERLOADSCHOOL`         | 2_S06.dat                                                                                    |
|  329 | 2_S06_tutLattice                | `TRIGGER._2_S06_TUTLATTICE`                | 2_S06.dat                                                                                    |
|  330 | 306PoorArea                     | `TRIGGER._306POORAREA`                     | 3_06New.dat                                                                                  |
|  331 | 3B_CopsSpeedUp                  | `TRIGGER._3B_COPSSPEEDUP`                  | 3_B.dat                                                                                      |
|  332 | 3_01D_RUDY                      | `TRIGGER._3_01D_RUDY`                      | 3_01D.dat                                                                                    |
|  333 | 3_01_KissFinal                  | `TRIGGER._3_01_KISSFINAL`                  | 3_01.dat                                                                                     |
|  334 | 3_01_MeetClimb                  | `TRIGGER._3_01_MEETCLIMB`                  | 3_01.dat                                                                                     |
|  335 | 3_01_MissionArea                | `TRIGGER._3_01_MISSIONAREA`                | 3_01.dat                                                                                     |
|  336 | 3_01_MissionBlock               | `TRIGGER._3_01_MISSIONBLOCK`               | 3_01.dat                                                                                     |
|  337 | 3_01_OnRoof                     | `TRIGGER._3_01_ONROOF`                     | 3_01.dat                                                                                     |
|  338 | 3_02_BUSINESSAREA               | `TRIGGER._3_02_BUSINESSAREA`               | 3_02.dat, 3_02_new.dat                                                                       |
|  339 | 3_02_PARKENTRANCE               | `TRIGGER._3_02_PARKENTRANCE`               | 3_02.dat, 3_02_new.dat                                                                       |
|  340 | 3_02_SPAWNER01                  | `TRIGGER._3_02_SPAWNER01`                  | 3_02.dat, 3_02_new.dat                                                                       |
|  341 | 3_02_SPAWNER02                  | `TRIGGER._3_02_SPAWNER02`                  | 3_02.dat, 3_02_new.dat                                                                       |
|  342 | 3_02_SPAWNER03                  | `TRIGGER._3_02_SPAWNER03`                  | 3_02.dat, 3_02_new.dat                                                                       |
|  343 | 3_02_SPAWNER04                  | `TRIGGER._3_02_SPAWNER04`                  | 3_02.dat, 3_02_new.dat                                                                       |
|  344 | 3_02_SPAWNER05                  | `TRIGGER._3_02_SPAWNER05`                  | 3_02.dat, 3_02_new.dat                                                                       |
|  345 | 3_04_algieFlee                  | `TRIGGER._3_04_ALGIEFLEE`                  | 3_04.dat                                                                                     |
|  346 | 3_04_cornScream2                | `TRIGGER._3_04_CORNSCREAM2`                | 3_04.dat                                                                                     |
|  347 | 3_04_corneliusCut               | `TRIGGER._3_04_CORNELIUSCUT`               | 3_04.dat                                                                                     |
|  348 | 3_04_loadBikes                  | `TRIGGER._3_04_LOADBIKES`                  | 3_04.dat                                                                                     |
|  349 | 3_04_stg4_Return                | `TRIGGER._3_04_STG4_RETURN`                | 3_04.dat                                                                                     |
|  350 | 3_05_1StartUpstairs             | `TRIGGER._3_05_1STARTUPSTAIRS`             | 3_05.dat                                                                                     |
|  351 | 3_05_2CatwalkStart              | `TRIGGER._3_05_2CATWALKSTART`              | 3_05.dat                                                                                     |
|  352 | 3_05_3NortonsDoor               | `TRIGGER._3_05_3NORTONSDOOR`               | 3_05.dat                                                                                     |
|  353 | 3_05_Ambush                     | `TRIGGER._3_05_AMBUSH`                     | 3_05.dat                                                                                     |
|  354 | 3_05_BossFightTrigger           | `TRIGGER._3_05_BOSSFIGHTTRIGGER`           | 3_05.dat                                                                                     |
|  355 | 3_05_Catwalk2                   | `TRIGGER._3_05_CATWALK2`                   | 3_05.dat                                                                                     |
|  356 | 3_05_ExitGreasers1              | `TRIGGER._3_05_EXITGREASERS1`              | 3_05.dat                                                                                     |
|  357 | 3_05_Hammerwall01               | `TRIGGER._3_05_HAMMERWALL01`               | 3_05.dat                                                                                     |
|  358 | 3_05_Hammerwall02               | `TRIGGER._3_05_HAMMERWALL02`               | 3_05.dat                                                                                     |
|  359 | 3_05_Hammerwall03               | `TRIGGER._3_05_HAMMERWALL03`               | 3_05.dat                                                                                     |
|  360 | 3_05_Hammerwall04               | `TRIGGER._3_05_HAMMERWALL04`               | 3_05.dat                                                                                     |
|  361 | 3_05_Hammerwall05               | `TRIGGER._3_05_HAMMERWALL05`               | 3_05.dat                                                                                     |
|  362 | 3_05_SecondFloor                | `TRIGGER._3_05_SECONDFLOOR`                | 3_05.dat                                                                                     |
|  363 | 3_05_StartCatwalk               | `TRIGGER._3_05_STARTCATWALK`               | 3_05.dat                                                                                     |
|  364 | 3_05_StartShooting              | `TRIGGER._3_05_STARTSHOOTING`              | 3_05.dat                                                                                     |
|  365 | 3_05_StartShooting2             | `TRIGGER._3_05_STARTSHOOTING2`             | 3_05.dat                                                                                     |
|  366 | 3_06_FailTrig                   | `TRIGGER._3_06_FAILTRIG`                   | 3_06New.dat                                                                                  |
|  367 | 3_06_FightTrig                  | `TRIGGER._3_06_FIGHTTRIG`                  | 3_06New.dat                                                                                  |
|  368 | 3_06_InnerArea                  | `TRIGGER._3_06_INNERAREA`                  | 3_06New.dat                                                                                  |
|  369 | 3_06_OuterArea                  | `TRIGGER._3_06_OUTERAREA`                  | 3_06New.dat                                                                                  |
|  370 | 3_07_StartConv                  | `TRIGGER._3_07_STARTCONV`                  | 3_07.dat                                                                                     |
|  371 | 3_08_BackToRoomTrig             | `TRIGGER._3_08_BACKTOROOMTRIG`             | 3_08.dat                                                                                     |
|  372 | 3_08_Intercom_Trigger           | `TRIGGER._3_08_INTERCOM_TRIGGER`           | 3_08.dat                                                                                     |
|  373 | 3_08_RunStart                   | `TRIGGER._3_08_RUNSTART`                   | 3_08.dat                                                                                     |
|  374 | 3_08_SchoolPop                  | `TRIGGER._3_08_SCHOOLPOP`                  | 3_08.dat                                                                                     |
|  375 | 3_B_BIKE_REGION_NE              | `TRIGGER._3_B_BIKE_REGION_NE`              | 3_B_BIKE_STUFF.dat                                                                           |
|  376 | 3_B_BIKE_REGION_NW              | `TRIGGER._3_B_BIKE_REGION_NW`              | 3_B_BIKE_STUFF.dat                                                                           |
|  377 | 3_B_BIKE_REGION_SE              | `TRIGGER._3_B_BIKE_REGION_SE`              | 3_B_BIKE_STUFF.dat                                                                           |
|  378 | 3_B_BIKE_REGION_SW              | `TRIGGER._3_B_BIKE_REGION_SW`              | 3_B_BIKE_STUFF.dat                                                                           |
|  379 | 3_B_MAGNET                      | `TRIGGER._3_B_MAGNET`                      | 3_B.dat                                                                                      |
|  380 | 3_B_REGION_S                    | `TRIGGER._3_B_REGION_S`                    | 3_B_BIKE_STUFF.dat                                                                           |
|  381 | 3_B_STAGE_2_TRIGGER             | `TRIGGER._3_B_STAGE_2_TRIGGER`             | 3_B.dat                                                                                      |
|  382 | 3_G3_CheeringCrowd              | `TRIGGER._3_G3_CHEERINGCROWD`              | 3_G3.dat                                                                                     |
|  383 | 3_G3_MoveLola                   | `TRIGGER._3_G3_MOVELOLA`                   | 3_G3.dat                                                                                     |
|  384 | 3_G3_Tree1                      | `TRIGGER._3_G3_TREE1`                      | 3_G3.dat                                                                                     |
|  385 | 3_G3_Tree2                      | `TRIGGER._3_G3_TREE2`                      | 3_G3.dat                                                                                     |
|  386 | 3_G3_Tree3                      | `TRIGGER._3_G3_TREE3`                      | 3_G3.dat                                                                                     |
|  387 | 3_G3_Tree4                      | `TRIGGER._3_G3_TREE4`                      | 3_G3.dat                                                                                     |
|  388 | 3_R09_AreaT01                   | `TRIGGER._3_R09_AREAT01`                   | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Preppies.dat                  |
|  389 | 3_R09_AreaT02                   | `TRIGGER._3_R09_AREAT02`                   | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Preppies.dat                  |
|  390 | 3_R09_BasementTrigger           | `TRIGGER._3_R09_BASEMENTTRIGGER`           | 3_R09_Nerds.dat                                                                              |
|  391 | 3_R09_MainArea                  | `TRIGGER._3_R09_MAINAREA`                  | 3_R09_Dropouts.dat, 3_R09_Greasers.dat                                                       |
|  392 | 3_R09_SpawnT01                  | `TRIGGER._3_R09_SPAWNT01`                  | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Nerds.dat, 3_R09_Preppies.dat |
|  393 | 3_R09_SpawnT02                  | `TRIGGER._3_R09_SPAWNT02`                  | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Nerds.dat, 3_R09_Preppies.dat |
|  394 | 3_R09_Upstairs                  | `TRIGGER._3_R09_UPSTAIRS`                  | 3_R09_Nerds.dat                                                                              |
|  395 | 3_S03T_H_Car_Drop7_Stop         | `TRIGGER._3_S03T_H_CAR_DROP7_STOP`         | 3_S03T.dat                                                                                   |
|  396 | 3_S03T_OPEN_GATE_T              | `TRIGGER._3_S03T_OPEN_GATE_T`              | 3_S03T.dat                                                                                   |
|  397 | 3_S03T_Test_1                   | `TRIGGER._3_S03T_TEST_1`                   | 3_S03T.dat                                                                                   |
|  398 | 3_S03T_Test_1_Activate          | `TRIGGER._3_S03T_TEST_1_ACTIVATE`          | 3_S03T.dat                                                                                   |
|  399 | 3_S03T_Test_2                   | `TRIGGER._3_S03T_TEST_2`                   | 3_S03T.dat                                                                                   |
|  400 | 3_S03T_Test_2_Activate          | `TRIGGER._3_S03T_TEST_2_ACTIVATE`          | 3_S03T.dat                                                                                   |
|  401 | 3_S03T_Test_3                   | `TRIGGER._3_S03T_TEST_3`                   | 3_S03T.dat                                                                                   |
|  402 | 3_S03T_Test_3_Activate          | `TRIGGER._3_S03T_TEST_3_ACTIVATE`          | 3_S03T.dat                                                                                   |
|  403 | 3_S03T_Test_4                   | `TRIGGER._3_S03T_TEST_4`                   | 3_S03T.dat                                                                                   |
|  404 | 3_S03T_Test_4_Activate          | `TRIGGER._3_S03T_TEST_4_ACTIVATE`          | 3_S03T.dat                                                                                   |
|  405 | 3_S03T_Test_5                   | `TRIGGER._3_S03T_TEST_5`                   | 3_S03T.dat                                                                                   |
|  406 | 3_S03T_Test_5_Activate          | `TRIGGER._3_S03T_TEST_5_ACTIVATE`          | 3_S03T.dat                                                                                   |
|  407 | 3_S03T_Test_6                   | `TRIGGER._3_S03T_TEST_6`                   | 3_S03T.dat                                                                                   |
|  408 | 3_S03T_Test_6_Activate          | `TRIGGER._3_S03T_TEST_6_ACTIVATE`          | 3_S03T.dat                                                                                   |
|  409 | 3_S03_TEMP_DOORTELEPORT         | `TRIGGER._3_S03_TEMP_DOORTELEPORT`         | 3_S03T.dat                                                                                   |
|  410 | 3_S03_failAlley                 | `TRIGGER._3_S03_FAILALLEY`                 | 3_S03.dat                                                                                    |
|  411 | 3_S03_failGreaser               | `TRIGGER._3_S03_FAILGREASER`               | 3_S03.dat                                                                                    |
|  412 | 3_S03_failPool                  | `TRIGGER._3_S03_FAILPOOL`                  | 3_S03.dat                                                                                    |
|  413 | 3_S03_objectiveAlley            | `TRIGGER._3_S03_OBJECTIVEALLEY`            | 3_S03.dat                                                                                    |
|  414 | 3_S03_objectiveGreaser          | `TRIGGER._3_S03_OBJECTIVEGREASER`          | 3_S03.dat                                                                                    |
|  415 | 3_S03_objectivePool             | `TRIGGER._3_S03_OBJECTIVEPOOL`             | 3_S03.dat                                                                                    |
|  416 | 3_S03_parkingLot                | `TRIGGER._3_S03_PARKINGLOT`                | 3_S03.dat                                                                                    |
|  417 | 3_S03_poolArea                  | `TRIGGER._3_S03_POOLAREA`                  | 3_S03.dat                                                                                    |
|  418 | 3_S09_AmbushTrigger01           | `TRIGGER._3_S09_AMBUSHTRIGGER01`           | 3_S09.dat                                                                                    |
|  419 | 3_S09_AmbushTrigger02           | `TRIGGER._3_S09_AMBUSHTRIGGER02`           | 3_S09.dat                                                                                    |
|  420 | 3_S09_AmbushTrigger03           | `TRIGGER._3_S09_AMBUSHTRIGGER03`           | 3_S09.dat                                                                                    |
|  421 | 3_S09_Breakable01               | `TRIGGER._3_S09_BREAKABLE01`               | 3_S09.dat                                                                                    |
|  422 | 3_S09_Breakable02               | `TRIGGER._3_S09_BREAKABLE02`               | 3_S09.dat                                                                                    |
|  423 | 3_S09_Breakable03               | `TRIGGER._3_S09_BREAKABLE03`               | 3_S09.dat                                                                                    |
|  424 | 3_S09_Breakable04               | `TRIGGER._3_S09_BREAKABLE04`               | 3_S09.dat                                                                                    |
|  425 | 3_S09_Breakable05               | `TRIGGER._3_S09_BREAKABLE05`               | 3_S09.dat                                                                                    |
|  426 | 3_S09_Breakable06               | `TRIGGER._3_S09_BREAKABLE06`               | 3_S09.dat                                                                                    |
|  427 | 3_S09_Breakable07               | `TRIGGER._3_S09_BREAKABLE07`               | 3_S09.dat                                                                                    |
|  428 | 3_S09_Breakable08               | `TRIGGER._3_S09_BREAKABLE08`               | 3_S09.dat                                                                                    |
|  429 | 3_S09_Breakable09               | `TRIGGER._3_S09_BREAKABLE09`               | 3_S09.dat                                                                                    |
|  430 | 3_S09_Breakable10               | `TRIGGER._3_S09_BREAKABLE10`               | 3_S09.dat                                                                                    |
|  431 | 3_S09_Cover01                   | `TRIGGER._3_S09_COVER01`                   | 3_S09.dat, RaulTest.dat                                                                      |
|  432 | 3_S09_Cover02                   | `TRIGGER._3_S09_COVER02`                   | 3_S09.dat, RaulTest.dat                                                                      |
|  433 | 3_S09_Cover03                   | `TRIGGER._3_S09_COVER03`                   | 3_S09.dat, RaulTest.dat                                                                      |
|  434 | 3_S09_Cover04                   | `TRIGGER._3_S09_COVER04`                   | 3_S09.dat, RaulTest.dat                                                                      |
|  435 | 3_S09_Cover05                   | `TRIGGER._3_S09_COVER05`                   | 3_S09.dat                                                                                    |
|  436 | 3_S09_CoverArea                 | `TRIGGER._3_S09_COVERAREA`                 | 3_S09.dat, RaulTest.dat                                                                      |
|  437 | 3_S09_CoverCrate01              | `TRIGGER._3_S09_COVERCRATE01`              | 3_S09.dat                                                                                    |
|  438 | 3_S09_CoverCrate02              | `TRIGGER._3_S09_COVERCRATE02`              | 3_S09.dat                                                                                    |
|  439 | 3_S09_Dumpster01                | `TRIGGER._3_S09_DUMPSTER01`                | 3_S09.dat, RaulTest.dat                                                                      |
|  440 | 3_S09_LeavingTrigger            | `TRIGGER._3_S09_LEAVINGTRIGGER`            | 3_S09.dat, RaulTest.dat                                                                      |
|  441 | 3_S10_ATagsLoad                 | `TRIGGER._3_S10_ATAGSLOAD`                 | 3_S10.dat                                                                                    |
|  442 | 3_S10_BTagsLoad                 | `TRIGGER._3_S10_BTAGSLOAD`                 | 3_S10.dat                                                                                    |
|  443 | 3_S10_CTagsLoad                 | `TRIGGER._3_S10_CTAGSLOAD`                 | 3_S10.dat                                                                                    |
|  444 | 3_S10_DTagsLoad                 | `TRIGGER._3_S10_DTAGSLOAD`                 | 3_S10.dat                                                                                    |
|  445 | 3_S10_PoorArea                  | `TRIGGER._3_S10_POORAREA`                  | 3_S10.dat                                                                                    |
|  446 | 3_S10_TUT_TAG                   | `TRIGGER._3_S10_TUT_TAG`                   | 3_S10.dat                                                                                    |
|  447 | 3_S10_TutTrigger                | `TRIGGER._3_S10_TUTTRIGGER`                | 3_S10.dat                                                                                    |
|  448 | 3_S10_Tut_Tag02                 | `TRIGGER._3_S10_TUT_TAG02`                 | 3_S10.dat                                                                                    |
|  449 | 3_S10_Tut_Tag03                 | `TRIGGER._3_S10_TUT_TAG03`                 | 3_S10.dat                                                                                    |
|  450 | 3_S10_TutorialStart             | `TRIGGER._3_S10_TUTORIALSTART`             | 3_S10.dat                                                                                    |
|  451 | 3_S10_underBridge               | `TRIGGER._3_S10_UNDERBRIDGE`               | 3_S10.dat                                                                                    |
|  452 | 3_S11_Asylum_Gate_Warning       | `TRIGGER._3_S11_ASYLUM_GATE_WARNING`       | 3_S11.dat                                                                                    |
|  453 | 3_S11_Asylum_Gate_Warning2      | `TRIGGER._3_S11_ASYLUM_GATE_WARNING2`      | 3_S11.dat                                                                                    |
|  454 | 3_S11_Break_Out                 | `TRIGGER._3_S11_BREAK_OUT`                 | 3_S11.dat                                                                                    |
|  455 | 3_S11_Fire01                    | `TRIGGER._3_S11_FIRE01`                    | 3_S11.dat                                                                                    |
|  456 | 3_S11_Fire02                    | `TRIGGER._3_S11_FIRE02`                    | 3_S11.dat                                                                                    |
|  457 | 3_S11_Fire03                    | `TRIGGER._3_S11_FIRE03`                    | 3_S11.dat                                                                                    |
|  458 | 3_S11_Fire04                    | `TRIGGER._3_S11_FIRE04`                    | 3_S11.dat                                                                                    |
|  459 | 3_S11_Fire05                    | `TRIGGER._3_S11_FIRE05`                    | 3_S11.dat                                                                                    |
|  460 | 3_S11_Fire06                    | `TRIGGER._3_S11_FIRE06`                    | 3_S11.dat                                                                                    |
|  461 | 3_S11_Fire07                    | `TRIGGER._3_S11_FIRE07`                    | 3_S11.dat                                                                                    |
|  462 | 3_S11_Galloway_Trigger          | `TRIGGER._3_S11_GALLOWAY_TRIGGER`          | 3_S11.dat                                                                                    |
|  463 | 3_S11_Inside_Asylum             | `TRIGGER._3_S11_INSIDE_ASYLUM`             | 3_S11.dat                                                                                    |
|  464 | 3_S11_PHILLIPS_REUNION          | `TRIGGER._3_S11_PHILLIPS_REUNION`          | 3_S11.dat                                                                                    |
|  465 | 3_S11_Phillips_Car_Stop         | `TRIGGER._3_S11_PHILLIPS_CAR_STOP`         | 3_S11.dat                                                                                    |
|  466 | 3_S11_Player_On_A_Grounds       | `TRIGGER._3_S11_PLAYER_ON_A_GROUNDS`       | 3_S11.dat                                                                                    |
|  467 | 3_S_10_FailTrigger              | `TRIGGER._3_S_10_FAILTRIGGER`              | 3_S10.dat                                                                                    |
|  468 | 3_XM_SpawnTrigger               | `TRIGGER._3_XM_SPAWNTRIGGER`               | 3_XM.dat                                                                                     |
|  469 | 4_01_artNorth                   | `TRIGGER._4_01_ARTNORTH`                   | 4_01.dat                                                                                     |
|  470 | 4_01_artSouth                   | `TRIGGER._4_01_ARTSOUTH`                   | 4_01.dat                                                                                     |
|  471 | 4_01_christySpeech              | `TRIGGER._4_01_CHRISTYSPEECH`              | 4_01.dat                                                                                     |
|  472 | 4_01_girlsDormBathroom          | `TRIGGER._4_01_GIRLSDORMBATHROOM`          | 4_01.dat                                                                                     |
|  473 | 4_01_gymInsideDoor              | `TRIGGER._4_01_GYMINSIDEDOOR`              | 4_01.dat                                                                                     |
|  474 | 4_01_gymTunnel                  | `TRIGGER._4_01_GYMTUNNEL`                  | 4_01.dat                                                                                     |
|  475 | 4_01_launchEunice               | `TRIGGER._4_01_LAUNCHEUNICE`               | 4_01.dat                                                                                     |
|  476 | 4_01_mandyRoom                  | `TRIGGER._4_01_MANDYROOM`                  | 4_01.dat                                                                                     |
|  477 | 4_01_mandyRoomBusted            | `TRIGGER._4_01_MANDYROOMBUSTED`            | 4_01.dat                                                                                     |
|  478 | 4_01_mandyRoomWarn              | `TRIGGER._4_01_MANDYROOMWARN`              | 4_01.dat                                                                                     |
|  479 | 4_01_showerRoom                 | `TRIGGER._4_01_SHOWERROOM`                 | 4_01.dat                                                                                     |
|  480 | 4_01_showerWarn                 | `TRIGGER._4_01_SHOWERWARN`                 | 4_01.dat                                                                                     |
|  481 | 4_01_tutLattice                 | `TRIGGER._4_01_TUTLATTICE`                 | 4_01.dat                                                                                     |
|  482 | 4_02_Algie_Final_Stand          | `TRIGGER._4_02_ALGIE_FINAL_STAND`          | Test_4_02.dat                                                                                |
|  483 | 4_02_Algie_Left_Lib             | `TRIGGER._4_02_ALGIE_LEFT_LIB`             | Test_4_02.dat                                                                                |
|  484 | 4_02_Bar_01                     | `TRIGGER._4_02_BAR_01`                     | 4_02.dat, Test_4_02.dat                                                                      |
|  485 | 4_02_Bar_02                     | `TRIGGER._4_02_BAR_02`                     | 4_02.dat, Test_4_02.dat                                                                      |
|  486 | 4_02_Bar_03                     | `TRIGGER._4_02_BAR_03`                     | 4_02.dat, Test_4_02.dat                                                                      |
|  487 | 4_02_Breaker_Box                | `TRIGGER._4_02_BREAKER_BOX`                | 4_02.dat, Test_4_02.dat                                                                      |
|  488 | 4_02_Delete_Wave1               | `TRIGGER._4_02_DELETE_WAVE1`               | 4_02.dat, Test_4_02.dat                                                                      |
|  489 | 4_02_Delete_Wave3               | `TRIGGER._4_02_DELETE_WAVE3`               | 4_02.dat, Test_4_02.dat                                                                      |
|  490 | 4_02_Eavesdrop                  | `TRIGGER._4_02_EAVESDROP`                  | 4_02.dat, Test_4_02.dat                                                                      |
|  491 | 4_02_Finale                     | `TRIGGER._4_02_FINALE`                     | 4_02.dat, Test_4_02.dat                                                                      |
|  492 | 4_02_GateKeeper                 | `TRIGGER._4_02_GATEKEEPER`                 | 4_02.dat                                                                                     |
|  493 | 4_02_KeyPad                     | `TRIGGER._4_02_KEYPAD`                     | 4_02.dat                                                                                     |
|  494 | 4_02_NERDS                      | `TRIGGER._4_02_NERDS`                      | 4_02.dat, Test_4_02.dat                                                                      |
|  495 | 4_02_Nerd_Ambush1               | `TRIGGER._4_02_NERD_AMBUSH1`               | Test_4_02.dat                                                                                |
|  496 | 4_02_Nerd_Ambush2               | `TRIGGER._4_02_NERD_AMBUSH2`               | Test_4_02.dat                                                                                |
|  497 | 4_02_Nerd_Deleter               | `TRIGGER._4_02_NERD_DELETER`               | Test_4_02.dat                                                                                |
|  498 | 4_02_O_R1_1T                    | `TRIGGER._4_02_O_R1_1T`                    | 4_02.dat, Test_4_02.dat                                                                      |
|  499 | 4_02_O_R2_1T                    | `TRIGGER._4_02_O_R2_1T`                    | 4_02.dat, Test_4_02.dat                                                                      |
|  500 | 4_02_O_WN1_1T                   | `TRIGGER._4_02_O_WN1_1T`                   | 4_02.dat, Test_4_02.dat                                                                      |
|  501 | 4_02_O_WN2_1T                   | `TRIGGER._4_02_O_WN2_1T`                   | 4_02.dat, Test_4_02.dat                                                                      |
|  502 | 4_02_O_WN3_1T                   | `TRIGGER._4_02_O_WN3_1T`                   | 4_02.dat, Test_4_02.dat                                                                      |
|  503 | 4_02_O_WN4_1T                   | `TRIGGER._4_02_O_WN4_1T`                   | 4_02.dat, Test_4_02.dat                                                                      |
|  504 | 4_02_O_W_F_1T                   | `TRIGGER._4_02_O_W_F_1T`                   | Test_4_02.dat                                                                                |
|  505 | 4_02_ObsDoor                    | `TRIGGER._4_02_OBSDOOR`                    | 4_02.dat                                                                                     |
|  506 | 4_02_ObsDoorCheck               | `TRIGGER._4_02_OBSDOORCHECK`               | 4_02.dat                                                                                     |
|  507 | 4_02_PREFECT1                   | `TRIGGER._4_02_PREFECT1`                   | 4_02.dat, Test_4_02.dat                                                                      |
|  508 | 4_02_PREFECT2                   | `TRIGGER._4_02_PREFECT2`                   | 4_02.dat, Test_4_02.dat                                                                      |
|  509 | 4_02_P_Wave2                    | `TRIGGER._4_02_P_WAVE2`                    | 4_02.dat, Test_4_02.dat                                                                      |
|  510 | 4_02_P_Wave3                    | `TRIGGER._4_02_P_WAVE3`                    | 4_02.dat, Test_4_02.dat                                                                      |
|  511 | 4_02_P_Wave4                    | `TRIGGER._4_02_P_WAVE4`                    | 4_02.dat, Test_4_02.dat                                                                      |
|  512 | 4_02_Player_On_CannonT          | `TRIGGER._4_02_PLAYER_ON_CANNONT`          | 4_02.dat, Test_4_02.dat                                                                      |
|  513 | 4_02_Player_Out_Of_Lib          | `TRIGGER._4_02_PLAYER_OUT_OF_LIB`          | 4_02.dat, Test_4_02.dat                                                                      |
|  514 | 4_02_Spotted_Scout              | `TRIGGER._4_02_SPOTTED_SCOUT`              | 4_02.dat, Test_4_02.dat                                                                      |
|  515 | 4_02_Spud_Cannon                | `TRIGGER._4_02_SPUD_CANNON`                | 4_02.dat, Test_4_02.dat                                                                      |
|  516 | 4_02_Spud_Tripod                | `TRIGGER._4_02_SPUD_TRIPOD`                | 4_02.dat, Test_4_02.dat                                                                      |
|  517 | 4_02_TEMP_Cannon_Line2          | `TRIGGER._4_02_TEMP_CANNON_LINE2`          | 4_02.dat, Test_4_02.dat                                                                      |
|  518 | 4_02_WATER                      | `TRIGGER._4_02_WATER`                      | Test_4_02.dat                                                                                |
|  519 | 4_03_Bar_05_01                  | `TRIGGER._4_03_BAR_05_01`                  | 4_03.dat                                                                                     |
|  520 | 4_03_Bar_05_02                  | `TRIGGER._4_03_BAR_05_02`                  | 4_03.dat                                                                                     |
|  521 | 4_03_Bar_Blip_Trigger           | `TRIGGER._4_03_BAR_BLIP_TRIGGER`           | 4_03.dat                                                                                     |
|  522 | 4_03_Cannon                     | `TRIGGER._4_03_CANNON`                     | 4_03.dat                                                                                     |
|  523 | 4_03_Cannon_Tripod              | `TRIGGER._4_03_CANNON_TRIPOD`              | 4_03.dat                                                                                     |
|  524 | 4_03_Jock_Past_Water            | `TRIGGER._4_03_JOCK_PAST_WATER`            | 4_03.dat                                                                                     |
|  525 | 4_03_Leave1                     | `TRIGGER._4_03_LEAVE1`                     | 4_03.dat                                                                                     |
|  526 | 4_03_Leave2                     | `TRIGGER._4_03_LEAVE2`                     | 4_03.dat                                                                                     |
|  527 | 4_03_Ob_Bar1                    | `TRIGGER._4_03_OB_BAR1`                    | 4_03.dat                                                                                     |
|  528 | 4_03_Ob_Bar2                    | `TRIGGER._4_03_OB_BAR2`                    | 4_03.dat                                                                                     |
|  529 | 4_03_Ob_Bar3                    | `TRIGGER._4_03_OB_BAR3`                    | 4_03.dat                                                                                     |
|  530 | 4_03_Ob_Bar4                    | `TRIGGER._4_03_OB_BAR4`                    | 4_03.dat                                                                                     |
|  531 | 4_03_Ob_Grounds                 | `TRIGGER._4_03_OB_GROUNDS`                 | 4_03.dat                                                                                     |
|  532 | 4_03_ObsDoor                    | `TRIGGER._4_03_OBSDOOR`                    | 4_03.dat                                                                                     |
|  533 | 4_03_Open_Door                  | `TRIGGER._4_03_OPEN_DOOR`                  | 4_03.dat                                                                                     |
|  534 | 4_03_Open_Door2                 | `TRIGGER._4_03_OPEN_DOOR2`                 | 4_03.dat                                                                                     |
|  535 | 4_03_Player_To_Far              | `TRIGGER._4_03_PLAYER_TO_FAR`              | 4_03.dat                                                                                     |
|  536 | 4_03_SetUp_Nerds                | `TRIGGER._4_03_SETUP_NERDS`                | 4_03.dat                                                                                     |
|  537 | 4_03_TETHER_BAR_04              | `TRIGGER._4_03_TETHER_BAR_04`              | 4_03.dat                                                                                     |
|  538 | 4_03_Trigger_Wave1              | `TRIGGER._4_03_TRIGGER_WAVE1`              | 4_03.dat                                                                                     |
|  539 | 4_04_CTRLROOM                   | `TRIGGER._4_04_CTRLROOM`                   | 4_04.dat                                                                                     |
|  540 | 4_04_ENDMINE                    | `TRIGGER._4_04_ENDMINE`                    | 4_04.dat                                                                                     |
|  541 | 4_04_EXIT                       | `TRIGGER._4_04_EXIT`                       | 4_04.dat                                                                                     |
|  542 | 4_04_JOCKNIS                    | `TRIGGER._4_04_JOCKNIS`                    | 4_04.dat                                                                                     |
|  543 | 4_04_MAZE_HALL_05               | `TRIGGER._4_04_MAZE_HALL_05`               | 4_04.dat                                                                                     |
|  544 | 4_04_MAZE_HALL_07               | `TRIGGER._4_04_MAZE_HALL_07`               | 4_04.dat                                                                                     |
|  545 | 4_04_MAZE_HALL_08               | `TRIGGER._4_04_MAZE_HALL_08`               | 4_04.dat                                                                                     |
|  546 | 4_04_MINE_ESCAPE                | `TRIGGER._4_04_MINE_ESCAPE`                | 4_04.dat                                                                                     |
|  547 | 4_04_MONITOR01                  | `TRIGGER._4_04_MONITOR01`                  | 4_04.dat                                                                                     |
|  548 | 4_04_MONITOR02                  | `TRIGGER._4_04_MONITOR02`                  | 4_04.dat                                                                                     |
|  549 | 4_04_MONITOR03                  | `TRIGGER._4_04_MONITOR03`                  | 4_04.dat                                                                                     |
|  550 | 4_04_MineNerds1                 | `TRIGGER._4_04_MINENERDS1`                 | 4_04.dat                                                                                     |
|  551 | 4_04_MineNerds2                 | `TRIGGER._4_04_MINENERDS2`                 | 4_04.dat                                                                                     |
|  552 | 4_04_MineNerds3                 | `TRIGGER._4_04_MINENERDS3`                 | 4_04.dat                                                                                     |
|  553 | 4_04_NerdTrig                   | `TRIGGER._4_04_NERDTRIG`                   | 4_04.dat                                                                                     |
|  554 | 4_04_REACHED_FUNHOUSE           | `TRIGGER._4_04_REACHED_FUNHOUSE`           | 4_04.dat                                                                                     |
|  555 | 4_04_Reaper01                   | `TRIGGER._4_04_REAPER01`                   | 4_04.dat                                                                                     |
|  556 | 4_04_Reaper02                   | `TRIGGER._4_04_REAPER02`                   | 4_04.dat                                                                                     |
|  557 | 4_04_Reaper03                   | `TRIGGER._4_04_REAPER03`                   | 4_04.dat                                                                                     |
|  558 | 4_04_Reaper04                   | `TRIGGER._4_04_REAPER04`                   | 4_04.dat                                                                                     |
|  559 | 4_04_Reaper05                   | `TRIGGER._4_04_REAPER05`                   | 4_04.dat                                                                                     |
|  560 | 4_04_Reaper06                   | `TRIGGER._4_04_REAPER06`                   | 4_04.dat                                                                                     |
|  561 | 4_04_ReaperRoom                 | `TRIGGER._4_04_REAPERROOM`                 | 4_04.dat                                                                                     |
|  562 | 4_05_FIELD                      | `TRIGGER._4_05_FIELD`                      | 4_05.dat                                                                                     |
|  563 | 4_05_failAlley                  | `TRIGGER._4_05_FAILALLEY`                  | 4_05.dat                                                                                     |
|  564 | 4_05_failMain                   | `TRIGGER._4_05_FAILMAIN`                   | 4_05.dat                                                                                     |
|  565 | 4_05_failPath                   | `TRIGGER._4_05_FAILPATH`                   | 4_05.dat                                                                                     |
|  566 | 4_05_mascotPOI1                 | `TRIGGER._4_05_MASCOTPOI1`                 | 4_05.dat                                                                                     |
|  567 | 4_05_mascotPOI2                 | `TRIGGER._4_05_MASCOTPOI2`                 | 4_05.dat                                                                                     |
|  568 | 4_05_mascotPOI3                 | `TRIGGER._4_05_MASCOTPOI3`                 | 4_05.dat                                                                                     |
|  569 | 4_05_mascotPOI4                 | `TRIGGER._4_05_MASCOTPOI4`                 | 4_05.dat                                                                                     |
|  570 | 4_05_mascotPOI5                 | `TRIGGER._4_05_MASCOTPOI5`                 | 4_05.dat                                                                                     |
|  571 | 4_05_nerdAmbush                 | `TRIGGER._4_05_NERDAMBUSH`                 | 4_05.dat                                                                                     |
|  572 | 4_05_warnAlley                  | `TRIGGER._4_05_WARNALLEY`                  | 4_05.dat                                                                                     |
|  573 | 4_05_warnMain                   | `TRIGGER._4_05_WARNMAIN`                   | 4_05.dat                                                                                     |
|  574 | 4_05_warnPath                   | `TRIGGER._4_05_WARNPATH`                   | 4_05.dat                                                                                     |
|  575 | 4_05cut_fakeDoor                | `TRIGGER._4_05CUT_FAKEDOOR`                | 4_05cut.dat                                                                                  |
|  576 | 4_06_BIB01                      | `TRIGGER._4_06_BIB01`                      | 4_06.dat                                                                                     |
|  577 | 4_06_BIB02                      | `TRIGGER._4_06_BIB02`                      | 4_06.dat                                                                                     |
|  578 | 4_06_BIB03                      | `TRIGGER._4_06_BIB03`                      | 4_06.dat                                                                                     |
|  579 | 4_06_Bench_01                   | `TRIGGER._4_06_BENCH_01`                   | 4_06.dat                                                                                     |
|  580 | 4_06_Bench_01A                  | `TRIGGER._4_06_BENCH_01A`                  | 4_06.dat                                                                                     |
|  581 | 4_06_Bench_02                   | `TRIGGER._4_06_BENCH_02`                   | 4_06.dat                                                                                     |
|  582 | 4_06_Bench_02A                  | `TRIGGER._4_06_BENCH_02A`                  | 4_06.dat                                                                                     |
|  583 | 4_06_Bench_03                   | `TRIGGER._4_06_BENCH_03`                   | 4_06.dat                                                                                     |
|  584 | 4_06_Bench_03A                  | `TRIGGER._4_06_BENCH_03A`                  | 4_06.dat                                                                                     |
|  585 | 4_06_Bench_04                   | `TRIGGER._4_06_BENCH_04`                   | 4_06.dat                                                                                     |
|  586 | 4_06_Bench_04A                  | `TRIGGER._4_06_BENCH_04A`                  | 4_06.dat                                                                                     |
|  587 | 4_06_Cooler                     | `TRIGGER._4_06_COOLER`                     | 4_06.dat                                                                                     |
|  588 | 4_06_Cooler_Location            | `TRIGGER._4_06_COOLER_LOCATION`            | 4_06.dat                                                                                     |
|  589 | 4_06_DockingTrigger             | `TRIGGER._4_06_DOCKINGTRIGGER`             | 4_06.dat                                                                                     |
|  590 | 4_06_Duffle_Bag                 | `TRIGGER._4_06_DUFFLE_BAG`                 | 4_06.dat                                                                                     |
|  591 | 4_06_Field01                    | `TRIGGER._4_06_FIELD01`                    | 4_06.dat                                                                                     |
|  592 | 4_06_Field02                    | `TRIGGER._4_06_FIELD02`                    | 4_06.dat                                                                                     |
|  593 | 4_06_Field03                    | `TRIGGER._4_06_FIELD03`                    | 4_06.dat                                                                                     |
|  594 | 4_06_Field_Zone                 | `TRIGGER._4_06_FIELD_ZONE`                 | 4_06.dat                                                                                     |
|  595 | 4_06_GatObjective               | `TRIGGER._4_06_GATOBJECTIVE`               | 4_06.dat                                                                                     |
|  596 | 4_06_Hack_Switch                | `TRIGGER._4_06_HACK_SWITCH`                | 4_06.dat                                                                                     |
|  597 | 4_06_InsideDockingTrigger       | `TRIGGER._4_06_INSIDEDOCKINGTRIGGER`       | 4_06.dat                                                                                     |
|  598 | 4_06_Load_Field                 | `TRIGGER._4_06_LOAD_FIELD`                 | 4_06.dat                                                                                     |
|  599 | 4_06_OOB01                      | `TRIGGER._4_06_OOB01`                      | 4_06.dat                                                                                     |
|  600 | 4_06_OOB02                      | `TRIGGER._4_06_OOB02`                      | 4_06.dat                                                                                     |
|  601 | 4_06_OOB03                      | `TRIGGER._4_06_OOB03`                      | 4_06.dat                                                                                     |
|  602 | 4_06_OPAENDTRIGG                | `TRIGGER._4_06_OPAENDTRIGG`                | 4_06.dat                                                                                     |
|  603 | 4_06_OPCENDTRIGG                | `TRIGGER._4_06_OPCENDTRIGG`                | 4_06.dat                                                                                     |
|  604 | 4_06_OutsideGate                | `TRIGGER._4_06_OUTSIDEGATE`                | 4_06.dat                                                                                     |
|  605 | 4_B1_EARNEST_PATTERN02          | `TRIGGER._4_B1_EARNEST_PATTERN02`          | 4_B1.dat                                                                                     |
|  606 | 4_B1_EARNEST_PATTERN03          | `TRIGGER._4_B1_EARNEST_PATTERN03`          | 4_B1.dat                                                                                     |
|  607 | 4_G4_BleacherPervert            | `TRIGGER._4_G4_BLEACHERPERVERT`            | 4_G4.dat                                                                                     |
|  608 | 4_G4_BusPoster02                | `TRIGGER._4_G4_BUSPOSTER02`                | 4_G4.dat                                                                                     |
|  609 | 4_G4_BusPoster08                | `TRIGGER._4_G4_BUSPOSTER08`                | 4_G4.dat                                                                                     |
|  610 | 4_G4_BusTag2                    | `TRIGGER._4_G4_BUSTAG2`                    | 4_G4.dat                                                                                     |
|  611 | 4_G4_BusTag8                    | `TRIGGER._4_G4_BUSTAG8`                    | 4_G4.dat                                                                                     |
|  612 | 4_G4_LIBNERDS                   | `TRIGGER._4_G4_LIBNERDS`                   | 4_G4.dat                                                                                     |
|  613 | 4_G4_LeftTown                   | `TRIGGER._4_G4_LEFTTOWN`                   | 4_G4.dat                                                                                     |
|  614 | 4_G4_NerdComics                 | `TRIGGER._4_G4_NERDCOMICS`                 | 4_G4.dat                                                                                     |
|  615 | 4_G4_OutOfGrounds               | `TRIGGER._4_G4_OUTOFGROUNDS`               | 4_G4.dat                                                                                     |
|  616 | 4_G4_SchoolPoster02             | `TRIGGER._4_G4_SCHOOLPOSTER02`             | 4_G4.dat                                                                                     |
|  617 | 4_G4_SchoolPoster03             | `TRIGGER._4_G4_SCHOOLPOSTER03`             | 4_G4.dat                                                                                     |
|  618 | 4_G4_SchoolPoster04             | `TRIGGER._4_G4_SCHOOLPOSTER04`             | 4_G4.dat                                                                                     |
|  619 | 4_G4_SchoolTag2                 | `TRIGGER._4_G4_SCHOOLTAG2`                 | 4_G4.dat                                                                                     |
|  620 | 4_G4_SchoolTag3                 | `TRIGGER._4_G4_SCHOOLTAG3`                 | 4_G4.dat                                                                                     |
|  621 | 4_G4_SchoolTag4                 | `TRIGGER._4_G4_SCHOOLTAG4`                 | 4_G4.dat                                                                                     |
|  622 | 4_G4_TaggingTrig                | `TRIGGER._4_G4_TAGGINGTRIG`                | 4_G4.dat                                                                                     |
|  623 | 4_G4_TaggingTrig3               | `TRIGGER._4_G4_TAGGINGTRIG3`               | 4_G4.dat                                                                                     |
|  624 | 4_G4_TiltPost1                  | `TRIGGER._4_G4_TILTPOST1`                  | 4_G4.dat                                                                                     |
|  625 | 4_G4_TiltTag1                   | `TRIGGER._4_G4_TILTTAG1`                   | 4_G4.dat                                                                                     |
|  626 | 4_S11_AtticPlank01              | `TRIGGER._4_S11_ATTICPLANK01`              | 4_S11T.dat                                                                                   |
|  627 | 4_S11_AtticPlank02              | `TRIGGER._4_S11_ATTICPLANK02`              | 4_S11T.dat                                                                                   |
|  628 | 4_S11_AtticPlank03              | `TRIGGER._4_S11_ATTICPLANK03`              | 4_S11T.dat                                                                                   |
|  629 | 4_S11_DockerDoor                | `TRIGGER._4_S11_DOCKERDOOR`                | 4_S11T.dat                                                                                   |
|  630 | 4_S11_EndTrigger                | `TRIGGER._4_S11_ENDTRIGGER`                | 4_S11T.dat                                                                                   |
|  631 | 4_S11_FieldTrigger              | `TRIGGER._4_S11_FIELDTRIGGER`              | 4_S11T.dat                                                                                   |
|  632 | 4_S11_GymBag                    | `TRIGGER._4_S11_GYMBAG`                    | 4_S11T.dat                                                                                   |
|  633 | 4_S11_GymBagTrigger             | `TRIGGER._4_S11_GYMBAGTRIGGER`             | 4_S11T.dat                                                                                   |
|  634 | 4_S11_JPhoto                    | `TRIGGER._4_S11_JPHOTO`                    | 4_S11T.dat                                                                                   |
|  635 | 4_S11_JockDiscoveryTrigger      | `TRIGGER._4_S11_JOCKDISCOVERYTRIGGER`      | 4_S11T.dat                                                                                   |
|  636 | 4_S11_LockedDoor                | `TRIGGER._4_S11_LOCKEDDOOR`                | 4_S11T.dat                                                                                   |
|  637 | 4_S11_NerdTrigger               | `TRIGGER._4_S11_NERDTRIGGER`               | 4_S11T.dat                                                                                   |
|  638 | 4_S11_PaddleTrigger             | `TRIGGER._4_S11_PADDLETRIGGER`             | 4_S11T.dat                                                                                   |
|  639 | 4_S11_RandomTeacherTrigger      | `TRIGGER._4_S11_RANDOMTEACHERTRIGGER`      | 4_S11T.dat                                                                                   |
|  640 | 4_S11_SafeZone                  | `TRIGGER._4_S11_SAFEZONE`                  | 4_S11T.dat                                                                                   |
|  641 | 4_S11_SafeZoneA                 | `TRIGGER._4_S11_SAFEZONEA`                 | 4_S11T.dat                                                                                   |
|  642 | 4_S11_SafeZoneB                 | `TRIGGER._4_S11_SAFEZONEB`                 | 4_S11T.dat                                                                                   |
|  643 | 4_S12_MSPHILLIPS                | `TRIGGER._4_S12_MSPHILLIPS`                | 4_S12.dat                                                                                    |
|  644 | 4_S12_PEANUTBIKE                | `TRIGGER._4_S12_PEANUTBIKE`                | 4_S12.dat                                                                                    |
|  645 | 4_S12_PEANUTBIKE2               | `TRIGGER._4_S12_PEANUTBIKE2`               | 4_S12.dat                                                                                    |
|  646 | 5_01_Meet_Librarian             | `TRIGGER._5_01_MEET_LIBRARIAN`             | 5_01.dat                                                                                     |
|  647 | 5_01_RatSpawnT01                | `TRIGGER._5_01_RATSPAWNT01`                | 5_01.dat                                                                                     |
|  648 | 5_01_RatSpawnT02                | `TRIGGER._5_01_RATSPAWNT02`                | 5_01.dat                                                                                     |
|  649 | 5_01_RatSpawnT03                | `TRIGGER._5_01_RATSPAWNT03`                | 5_01.dat                                                                                     |
|  650 | 5_01_RatSpawnT04                | `TRIGGER._5_01_RATSPAWNT04`                | 5_01.dat                                                                                     |
|  651 | 5_01_RatSpawnT05                | `TRIGGER._5_01_RATSPAWNT05`                | 5_01.dat                                                                                     |
|  652 | 5_01_RatSpawnT06                | `TRIGGER._5_01_RATSPAWNT06`                | 5_01.dat                                                                                     |
|  653 | 5_01_RatSpawnT07                | `TRIGGER._5_01_RATSPAWNT07`                | 5_01.dat                                                                                     |
|  654 | 5_01_RatSpawnT08                | `TRIGGER._5_01_RATSPAWNT08`                | 5_01.dat                                                                                     |
|  655 | 5_01_RatSpawnT09                | `TRIGGER._5_01_RATSPAWNT09`                | 5_01.dat                                                                                     |
|  656 | 5_01_RatSpawnT10                | `TRIGGER._5_01_RATSPAWNT10`                | 5_01.dat                                                                                     |
|  657 | 5_01_RatSpawnT11                | `TRIGGER._5_01_RATSPAWNT11`                | 5_01.dat                                                                                     |
|  658 | 5_01_RatSpawnT12                | `TRIGGER._5_01_RATSPAWNT12`                | 5_01.dat                                                                                     |
|  659 | 5_01_RatSpawnT13                | `TRIGGER._5_01_RATSPAWNT13`                | 5_01.dat                                                                                     |
|  660 | 5_01_RatSpawnT14                | `TRIGGER._5_01_RATSPAWNT14`                | 5_01.dat                                                                                     |
|  661 | 5_01_RatSpawnT15                | `TRIGGER._5_01_RATSPAWNT15`                | 5_01.dat                                                                                     |
|  662 | 5_01_RatSpawnT16                | `TRIGGER._5_01_RATSPAWNT16`                | 5_01.dat                                                                                     |
|  663 | 5_01_RatSpawnT17                | `TRIGGER._5_01_RATSPAWNT17`                | 5_01.dat                                                                                     |
|  664 | 5_01_RatSpawnT18                | `TRIGGER._5_01_RATSPAWNT18`                | 5_01.dat                                                                                     |
|  665 | 5_01_RatSpawnT19                | `TRIGGER._5_01_RATSPAWNT19`                | 5_01.dat                                                                                     |
|  666 | 5_01_RatSpawnT20                | `TRIGGER._5_01_RATSPAWNT20`                | 5_01.dat                                                                                     |
|  667 | 5_01_main_room_tr               | `TRIGGER._5_01_MAIN_ROOM_TR`               | 5_01.dat                                                                                     |
|  668 | 5_02_BigSmoke                   | `TRIGGER._5_02_BIGSMOKE`                   | 5_02.dat                                                                                     |
|  669 | 5_02_BonfireTrigger01           | `TRIGGER._5_02_BONFIRETRIGGER01`           | 5_02.dat                                                                                     |
|  670 | 5_02_BonfireTrigger02           | `TRIGGER._5_02_BONFIRETRIGGER02`           | 5_02.dat                                                                                     |
|  671 | 5_02_DepopRichArea              | `TRIGGER._5_02_DEPOPRICHAREA`              | 5_02.dat                                                                                     |
|  672 | 5_02_DepopulateDocks            | `TRIGGER._5_02_DEPOPULATEDOCKS`            | 5_02.dat                                                                                     |
|  673 | 5_02_DockPartyCreate            | `TRIGGER._5_02_DOCKPARTYCREATE`            | 5_02.dat                                                                                     |
|  674 | 5_02_FailTrigger                | `TRIGGER._5_02_FAILTRIGGER`                | 5_02.dat                                                                                     |
|  675 | 5_02_FinalNIS                   | `TRIGGER._5_02_FINALNIS`                   | 5_02.dat                                                                                     |
|  676 | 5_02_Flame01                    | `TRIGGER._5_02_FLAME01`                    | 5_02.dat                                                                                     |
|  677 | 5_02_Flame02                    | `TRIGGER._5_02_FLAME02`                    | 5_02.dat                                                                                     |
|  678 | 5_02_Flame03                    | `TRIGGER._5_02_FLAME03`                    | 5_02.dat                                                                                     |
|  679 | 5_02_GameArea                   | `TRIGGER._5_02_GAMEAREA`                   | 5_02.dat                                                                                     |
|  680 | 5_02_GreaserHangout             | `TRIGGER._5_02_GREASERHANGOUT`             | 5_02.dat                                                                                     |
|  681 | 5_02_InWarehouse                | `TRIGGER._5_02_INWAREHOUSE`                | 5_02.dat                                                                                     |
|  682 | 5_02_NearNIS                    | `TRIGGER._5_02_NEARNIS`                    | 5_02.dat                                                                                     |
|  683 | 5_02_OnBarge                    | `TRIGGER._5_02_ONBARGE`                    | 5_02.dat                                                                                     |
|  684 | 5_02_PortExit                   | `TRIGGER._5_02_PORTEXIT`                   | 5_02.dat                                                                                     |
|  685 | 5_02_RatCrate                   | `TRIGGER._5_02_RATCRATE`                   | 5_02.dat                                                                                     |
|  686 | 5_02_StartRatPhoto              | `TRIGGER._5_02_STARTRATPHOTO`              | 5_02.dat                                                                                     |
|  687 | 5_02_TrophyPile                 | `TRIGGER._5_02_TROPHYPILE`                 | 5_02.dat                                                                                     |
|  688 | 5_02_WarehouseUpstairs          | `TRIGGER._5_02_WAREHOUSEUPSTAIRS`          | 5_02.dat                                                                                     |
|  689 | 5_02_WarehouseUpstairs02        | `TRIGGER._5_02_WAREHOUSEUPSTAIRS02`        | 5_02.dat                                                                                     |
|  690 | 5_03_1st_Floor_1st_Hall         | `TRIGGER._5_03_1ST_FLOOR_1ST_HALL`         | 5_03.dat                                                                                     |
|  691 | 5_03_Asylum_Grounds_SetUp       | `TRIGGER._5_03_ASYLUM_GROUNDS_SETUP`       | 5_03.dat                                                                                     |
|  692 | 5_03_BlockB                     | `TRIGGER._5_03_BLOCKB`                     | 5_03.dat                                                                                     |
|  693 | 5_03_Control_Room_Door          | `TRIGGER._5_03_CONTROL_ROOM_DOOR`          | 5_03.dat                                                                                     |
|  694 | 5_03_DOW_1                      | `TRIGGER._5_03_DOW_1`                      | 5_03.dat                                                                                     |
|  695 | 5_03_DOW_2                      | `TRIGGER._5_03_DOW_2`                      | 5_03.dat                                                                                     |
|  696 | 5_03_DOW_3                      | `TRIGGER._5_03_DOW_3`                      | 5_03.dat                                                                                     |
|  697 | 5_03_Exit                       | `TRIGGER._5_03_EXIT`                       | 5_03.dat                                                                                     |
|  698 | 5_03_FIRE01                     | `TRIGGER._5_03_FIRE01`                     | 5_03.dat                                                                                     |
|  699 | 5_03_FIRE02                     | `TRIGGER._5_03_FIRE02`                     | 5_03.dat                                                                                     |
|  700 | 5_03_FIRE03                     | `TRIGGER._5_03_FIRE03`                     | 5_03.dat                                                                                     |
|  701 | 5_03_FIRE04                     | `TRIGGER._5_03_FIRE04`                     | 5_03.dat                                                                                     |
|  702 | 5_03_FIRE05                     | `TRIGGER._5_03_FIRE05`                     | 5_03.dat                                                                                     |
|  703 | 5_03_FRONT_GATE_LINE            | `TRIGGER._5_03_FRONT_GATE_LINE`            | 5_03.dat                                                                                     |
|  704 | 5_03_GameOver                   | `TRIGGER._5_03_GAMEOVER`                   | 5_03.dat                                                                                     |
|  705 | 5_03_Gen_Johnny                 | `TRIGGER._5_03_GEN_JOHNNY`                 | 5_03.dat                                                                                     |
|  706 | 5_03_Inside_Asylum              | `TRIGGER._5_03_INSIDE_ASYLUM`              | 5_03.dat                                                                                     |
|  707 | 5_03_JOHNNY_END_TRIGGER         | `TRIGGER._5_03_JOHNNY_END_TRIGGER`         | 5_03.dat                                                                                     |
|  708 | 5_03_Johnny_Goto1               | `TRIGGER._5_03_JOHNNY_GOTO1`               | 5_03.dat                                                                                     |
|  709 | 5_03_Johnny_Trig1               | `TRIGGER._5_03_JOHNNY_TRIG1`               | 5_03.dat                                                                                     |
|  710 | 5_03_Johnny_Yelling             | `TRIGGER._5_03_JOHNNY_YELLING`             | 5_03.dat                                                                                     |
|  711 | 5_03_LEFT                       | `TRIGGER._5_03_LEFT`                       | 5_03.dat                                                                                     |
|  712 | 5_03_Leaving                    | `TRIGGER._5_03_LEAVING`                    | 5_03.dat                                                                                     |
|  713 | 5_03_OnGrounds                  | `TRIGGER._5_03_ONGROUNDS`                  | 5_03.dat                                                                                     |
|  714 | 5_03_Orderly_CS1_1              | `TRIGGER._5_03_ORDERLY_CS1_1`              | 5_03.dat                                                                                     |
|  715 | 5_03_Player_In_CR               | `TRIGGER._5_03_PLAYER_IN_CR`               | 5_03.dat                                                                                     |
|  716 | 5_03_Rec_Room                   | `TRIGGER._5_03_REC_ROOM`                   | 5_03.dat                                                                                     |
|  717 | 5_04_AMBUSH_01                  | `TRIGGER._5_04_AMBUSH_01`                  | 5_04.dat                                                                                     |
|  718 | 5_04_AMBUSH_02                  | `TRIGGER._5_04_AMBUSH_02`                  | 5_04.dat                                                                                     |
|  719 | 5_04_AMBUSH_03                  | `TRIGGER._5_04_AMBUSH_03`                  | 5_04.dat                                                                                     |
|  720 | 5_04_AMBUSH_04                  | `TRIGGER._5_04_AMBUSH_04`                  | 5_04.dat                                                                                     |
|  721 | 5_04_AMBUSH_05                  | `TRIGGER._5_04_AMBUSH_05`                  | 5_04.dat                                                                                     |
|  722 | 5_04_BANNERS_01                 | `TRIGGER._5_04_BANNERS_01`                 | 5_04.dat                                                                                     |
|  723 | 5_04_BANNERS_02                 | `TRIGGER._5_04_BANNERS_02`                 | 5_04.dat                                                                                     |
|  724 | 5_04_BANNERS_03                 | `TRIGGER._5_04_BANNERS_03`                 | 5_04.dat                                                                                     |
|  725 | 5_04_BANNERS_04                 | `TRIGGER._5_04_BANNERS_04`                 | 5_04.dat                                                                                     |
|  726 | 5_04_BANNERS_05                 | `TRIGGER._5_04_BANNERS_05`                 | 5_04.dat                                                                                     |
|  727 | 5_04_BANNERS_06                 | `TRIGGER._5_04_BANNERS_06`                 | 5_04.dat                                                                                     |
|  728 | 5_04_BANNERS_07                 | `TRIGGER._5_04_BANNERS_07`                 | 5_04.dat                                                                                     |
|  729 | 5_04_BANNERS_08                 | `TRIGGER._5_04_BANNERS_08`                 | 5_04.dat                                                                                     |
|  730 | 5_04_BANNERS_09                 | `TRIGGER._5_04_BANNERS_09`                 | 5_04.dat                                                                                     |
|  731 | 5_04_BANNERS_10                 | `TRIGGER._5_04_BANNERS_10`                 | 5_04.dat                                                                                     |
|  732 | 5_04_BANNERS_11                 | `TRIGGER._5_04_BANNERS_11`                 | 5_04.dat                                                                                     |
|  733 | 5_04_BANNERS_12                 | `TRIGGER._5_04_BANNERS_12`                 | 5_04.dat                                                                                     |
|  734 | 5_04_BANNERS_13                 | `TRIGGER._5_04_BANNERS_13`                 | 5_04.dat                                                                                     |
|  735 | 5_04_BIKE_STOP_01               | `TRIGGER._5_04_BIKE_STOP_01`               | 5_04.dat                                                                                     |
|  736 | 5_04_BIKE_STOP_02               | `TRIGGER._5_04_BIKE_STOP_02`               | 5_04.dat                                                                                     |
|  737 | 5_04_CHANGEROOM                 | `TRIGGER._5_04_CHANGEROOM`                 | 5_04.dat                                                                                     |
|  738 | 5_04_COP_START_01               | `TRIGGER._5_04_COP_START_01`               | 5_04.dat                                                                                     |
|  739 | 5_04_COP_START_02               | `TRIGGER._5_04_COP_START_02`               | 5_04.dat                                                                                     |
|  740 | 5_04_CREATE_FOURTH_PEDS         | `TRIGGER._5_04_CREATE_FOURTH_PEDS`         | 5_04.dat                                                                                     |
|  741 | 5_04_DOOR_HACK                  | `TRIGGER._5_04_DOOR_HACK`                  | 5_04.dat                                                                                     |
|  742 | 5_04_DO_CHAT                    | `TRIGGER._5_04_DO_CHAT`                    | 5_04.dat                                                                                     |
|  743 | 5_04_DO_ESCAPE                  | `TRIGGER._5_04_DO_ESCAPE`                  | 5_04.dat                                                                                     |
|  744 | 5_04_DO_GOAL                    | `TRIGGER._5_04_DO_GOAL`                    | 5_04.dat                                                                                     |
|  745 | 5_04_DO_NEAR_BIKE               | `TRIGGER._5_04_DO_NEAR_BIKE`               | 5_04.dat                                                                                     |
|  746 | 5_04_DO_STOP_01                 | `TRIGGER._5_04_DO_STOP_01`                 | 5_04.dat                                                                                     |
|  747 | 5_04_GYMHOOP                    | `TRIGGER._5_04_GYMHOOP`                    | 5_04.dat                                                                                     |
|  748 | 5_04_GYMWALL                    | `TRIGGER._5_04_GYMWALL`                    | 5_04.dat                                                                                     |
|  749 | 5_04_LASTAMBUSH                 | `TRIGGER._5_04_LASTAMBUSH`                 | 5_04.dat                                                                                     |
|  750 | 5_04_LIGHT_01                   | `TRIGGER._5_04_LIGHT_01`                   | 5_04.dat                                                                                     |
|  751 | 5_04_LIGHT_02                   | `TRIGGER._5_04_LIGHT_02`                   | 5_04.dat                                                                                     |
|  752 | 5_04_LIGHT_03                   | `TRIGGER._5_04_LIGHT_03`                   | 5_04.dat                                                                                     |
|  753 | 5_04_LIGHT_04                   | `TRIGGER._5_04_LIGHT_04`                   | 5_04.dat                                                                                     |
|  754 | 5_04_OTHERROUTE                 | `TRIGGER._5_04_OTHERROUTE`                 | 5_04.dat                                                                                     |
|  755 | 5_04_PREVENT01                  | `TRIGGER._5_04_PREVENT01`                  | 5_04.dat                                                                                     |
|  756 | 5_04_PREVENT02                  | `TRIGGER._5_04_PREVENT02`                  | 5_04.dat                                                                                     |
|  757 | 5_05_Alley                      | `TRIGGER._5_05_ALLEY`                      | 5_05.dat                                                                                     |
|  758 | 5_05_BoltCutters                | `TRIGGER._5_05_BOLTCUTTERS`                | 5_05.dat                                                                                     |
|  759 | 5_05_BurtonTether               | `TRIGGER._5_05_BURTONTETHER`               | 5_05.dat                                                                                     |
|  760 | 5_05_ClearMower                 | `TRIGGER._5_05_CLEARMOWER`                 | 5_05.dat                                                                                     |
|  761 | 5_05_DogFood                    | `TRIGGER._5_05_DOGFOOD`                    | 5_05.dat                                                                                     |
|  762 | 5_05_ExcludedMeatFactory        | `TRIGGER._5_05_EXCLUDEDMEATFACTORY`        | 5_05.dat                                                                                     |
|  763 | 5_05_FactoryArea                | `TRIGGER._5_05_FACTORYAREA`                | 5_05.dat                                                                                     |
|  764 | 5_05_LastPotty                  | `TRIGGER._5_05_LASTPOTTY`                  | 5_05.dat                                                                                     |
|  765 | 5_05_POTTY                      | `TRIGGER._5_05_POTTY`                      | 5_05.dat                                                                                     |
|  766 | 5_05_Park                       | `TRIGGER._5_05_PARK`                       | 5_05.dat                                                                                     |
|  767 | 5_05_ParkOut                    | `TRIGGER._5_05_PARKOUT`                    | 5_05.dat                                                                                     |
|  768 | 5_05_RunAwayZoe                 | `TRIGGER._5_05_RUNAWAYZOE`                 | 5_05.dat                                                                                     |
|  769 | 5_05_TBoneTarget                | `TRIGGER._5_05_TBONETARGET`                | 5_05.dat                                                                                     |
|  770 | 5_06_BarricadeCrash             | `TRIGGER._5_06_BARRICADECRASH`             | 5_06.dat                                                                                     |
|  771 | 5_06_BarricadeDoor              | `TRIGGER._5_06_BARRICADEDOOR`              | 5_06.dat                                                                                     |
|  772 | 5_06_BikeTrigger                | `TRIGGER._5_06_BIKETRIGGER`                | 5_06.dat                                                                                     |
|  773 | 5_06_Bridge                     | `TRIGGER._5_06_BRIDGE`                     | 5_06.dat                                                                                     |
|  774 | 5_06_EndTrigger                 | `TRIGGER._5_06_ENDTRIGGER`                 | 5_06.dat                                                                                     |
|  775 | 5_06_RussellDoor                | `TRIGGER._5_06_RUSSELLDOOR`                | 5_06.dat                                                                                     |
|  776 | 5_06_RussellGarage              | `TRIGGER._5_06_RUSSELLGARAGE`              | 5_06.dat                                                                                     |
|  777 | 5_06_RussellGate                | `TRIGGER._5_06_RUSSELLGATE`                | 5_06.dat                                                                                     |
|  778 | 5_06_RussellTrigger             | `TRIGGER._5_06_RUSSELLTRIGGER`             | 5_06.dat                                                                                     |
|  779 | 5_07_BarricadeNIS               | `TRIGGER._5_07_BARRICADENIS`               | 5_07.dat                                                                                     |
|  780 | 5_07_ChemEntrance               | `TRIGGER._5_07_CHEMENTRANCE`               | 5_07.dat                                                                                     |
|  781 | 5_07_DoorLocked01               | `TRIGGER._5_07_DOORLOCKED01`               | 5_07.dat                                                                                     |
|  782 | 5_07_DoorLocked02               | `TRIGGER._5_07_DOORLOCKED02`               | 5_07.dat                                                                                     |
|  783 | 5_07_ElectricDoor               | `TRIGGER._5_07_ELECTRICDOOR`               | 5_07.dat                                                                                     |
|  784 | 5_07_Fire01                     | `TRIGGER._5_07_FIRE01`                     | 5_07.dat                                                                                     |
|  785 | 5_07_FirstZoe                   | `TRIGGER._5_07_FIRSTZOE`                   | 5_07.dat                                                                                     |
|  786 | 5_07_MissionInit                | `TRIGGER._5_07_MISSIONINIT`                | 5_07.dat                                                                                     |
|  787 | 5_07_OmarFight                  | `TRIGGER._5_07_OMARFIGHT`                  | 5_07.dat                                                                                     |
|  788 | 5_07_OutsideTheOffice           | `TRIGGER._5_07_OUTSIDETHEOFFICE`           | 5_07.dat                                                                                     |
|  789 | 5_07_PartThree                  | `TRIGGER._5_07_PARTTHREE`                  | 5_07.dat                                                                                     |
|  790 | 5_07_PedAttack01                | `TRIGGER._5_07_PEDATTACK01`                | 5_07.dat                                                                                     |
|  791 | 5_07_PedAttack02                | `TRIGGER._5_07_PEDATTACK02`                | 5_07.dat                                                                                     |
|  792 | 5_07_PedAttack03                | `TRIGGER._5_07_PEDATTACK03`                | 5_07.dat                                                                                     |
|  793 | 5_07_Ranged01                   | `TRIGGER._5_07_RANGED01`                   | 5_07.dat                                                                                     |
|  794 | 5_07_Ranged02                   | `TRIGGER._5_07_RANGED02`                   | 5_07.dat                                                                                     |
|  795 | 5_07_SecondZoe                  | `TRIGGER._5_07_SECONDZOE`                  | 5_07.dat                                                                                     |
|  796 | 5_07_SecuritySwitch             | `TRIGGER._5_07_SECURITYSWITCH`             | 5_07.dat                                                                                     |
|  797 | 5_07_SiloAttack01               | `TRIGGER._5_07_SILOATTACK01`               | 5_07.dat                                                                                     |
|  798 | 5_07_Slaughterhouse             | `TRIGGER._5_07_SLAUGHTERHOUSE`             | 5_07.dat                                                                                     |
|  799 | 5_07_Spawner01                  | `TRIGGER._5_07_SPAWNER01`                  | 5_07.dat                                                                                     |
|  800 | 5_07_Spawner02                  | `TRIGGER._5_07_SPAWNER02`                  | 5_07.dat                                                                                     |
|  801 | 5_07_TrainSwitch                | `TRIGGER._5_07_TRAINSWITCH`                | 5_07.dat                                                                                     |
|  802 | 5_07_TrainSwitch02              | `TRIGGER._5_07_TRAINSWITCH02`              | 5_07.dat                                                                                     |
|  803 | 5_09_Ambush                     | `TRIGGER._5_09_AMBUSH`                     | 5_09.dat                                                                                     |
|  804 | 5_09_CityHallArea               | `TRIGGER._5_09_CITYHALLAREA`               | 5_09.dat                                                                                     |
|  805 | 5_09_CityHallTag2               | `TRIGGER._5_09_CITYHALLTAG2`               | 5_09.dat                                                                                     |
|  806 | 5_09_CityHallTag3               | `TRIGGER._5_09_CITYHALLTAG3`               | 5_09.dat                                                                                     |
|  807 | 5_09_CityHall_Building          | `TRIGGER._5_09_CITYHALL_BUILDING`          | 5_09.dat                                                                                     |
|  808 | 5_09_CityHall_Grounds           | `TRIGGER._5_09_CITYHALL_GROUNDS`           | 5_09.dat                                                                                     |
|  809 | 5_09_CityHall_Tag               | `TRIGGER._5_09_CITYHALL_TAG`               | 5_09.dat                                                                                     |
|  810 | 5_09_CityHall_Tower             | `TRIGGER._5_09_CITYHALL_TOWER`             | 5_09.dat                                                                                     |
|  811 | 5_09_CityHall_Wall_Climbed      | `TRIGGER._5_09_CITYHALL_WALL_CLIMBED`      | 5_09.dat                                                                                     |
|  812 | 5_09_DogYard                    | `TRIGGER._5_09_DOGYARD`                    | 5_09.dat                                                                                     |
|  813 | 5_09_Earnest_Outdoors           | `TRIGGER._5_09_EARNEST_OUTDOORS`           | 5_09.dat                                                                                     |
|  814 | 5_09_GreaserLoad                | `TRIGGER._5_09_GREASERLOAD`                | 5_09.dat                                                                                     |
|  815 | 5_09_Greaser_Safezone           | `TRIGGER._5_09_GREASER_SAFEZONE`           | 5_09.dat                                                                                     |
|  816 | 5_09_Paint_Yard                 | `TRIGGER._5_09_PAINT_YARD`                 | 5_09.dat                                                                                     |
|  817 | 5_09_PhotoOp                    | `TRIGGER._5_09_PHOTOOP`                    | 5_09.dat                                                                                     |
|  818 | 5_09_Players_Room               | `TRIGGER._5_09_PLAYERS_ROOM`               | 5_09.dat                                                                                     |
|  819 | 5_09_TowerTop                   | `TRIGGER._5_09_TOWERTOP`                   | 5_09.dat                                                                                     |
|  820 | 5_B_CHEM_DOOR                   | `TRIGGER._5_B_CHEM_DOOR`                   | iChemPlant.dat                                                                               |
|  821 | 5_B_CHEM_DOOR_2                 | `TRIGGER._5_B_CHEM_DOOR_2`                 | iChemPlant.dat                                                                               |
|  822 | 5_B_CRAWL                       | `TRIGGER._5_B_CRAWL`                       | 5_Ba.dat                                                                                     |
|  823 | 5_B_ChemCamShot                 | `TRIGGER._5_B_CHEMCAMSHOT`                 | 5_Ba.dat                                                                                     |
|  824 | 5_B_ChemCamShot02               | `TRIGGER._5_B_CHEMCAMSHOT02`               | 5_Ba.dat                                                                                     |
|  825 | 5_B_DEBUG_EDGAR                 | `TRIGGER._5_B_DEBUG_EDGAR`                 | 5_Ba.dat                                                                                     |
|  826 | 5_B_ENTRANCE                    | `TRIGGER._5_B_ENTRANCE`                    | 5_Ba.dat                                                                                     |
|  827 | 5_B_FALL_INTO_SLUDGE            | `TRIGGER._5_B_FALL_INTO_SLUDGE`            | 5_Ba.dat                                                                                     |
|  828 | 5_B_FINALSTAGE                  | `TRIGGER._5_B_FINALSTAGE`                  | 5_Ba.dat                                                                                     |
|  829 | 5_B_GRAB_GOOD                   | `TRIGGER._5_B_GRAB_GOOD`                   | 5_Ba.dat                                                                                     |
|  830 | 5_B_LIFTDOWN                    | `TRIGGER._5_B_LIFTDOWN`                    | 5_Ba.dat                                                                                     |
|  831 | 5_B_LIFTUP                      | `TRIGGER._5_B_LIFTUP`                      | 5_Ba.dat                                                                                     |
|  832 | 5_B_LadderCamShot               | `TRIGGER._5_B_LADDERCAMSHOT`               | 5_Ba.dat                                                                                     |
|  833 | 5_B_LadderCamShot02             | `TRIGGER._5_B_LADDERCAMSHOT02`             | 5_Ba.dat                                                                                     |
|  834 | 5_B_LadderCamShot03             | `TRIGGER._5_B_LADDERCAMSHOT03`             | 5_Ba.dat                                                                                     |
|  835 | 5_B_LowStaircase                | `TRIGGER._5_B_LOWSTAIRCASE`                | 5_Ba.dat                                                                                     |
|  836 | 5_B_STAGE2_START                | `TRIGGER._5_B_STAGE2_START`                | 5_Ba.dat                                                                                     |
|  837 | 5_B_STEAMAREA                   | `TRIGGER._5_B_STEAMAREA`                   | 5_Ba.dat                                                                                     |
|  838 | 5_B_SecDoor1                    | `TRIGGER._5_B_SECDOOR1`                    | 5_Ba.dat                                                                                     |
|  839 | 5_B_SecDoor2                    | `TRIGGER._5_B_SECDOOR2`                    | 5_Ba.dat                                                                                     |
|  840 | 5_G5_GroundDoorExit             | `TRIGGER._5_G5_GROUNDDOOREXIT`             | 5_G5.dat                                                                                     |
|  841 | 5_G5_Ladder04                   | `TRIGGER._5_G5_LADDER04`                   | 5_G5.dat                                                                                     |
|  842 | 5_G5_WHBackDoor                 | `TRIGGER._5_G5_WHBACKDOOR`                 | 5_G5.dat                                                                                     |
|  843 | 5_G5_WHFrontDoor                | `TRIGGER._5_G5_WHFRONTDOOR`                | 5_G5.dat                                                                                     |
|  844 | 5_G5_WareDoorZoe                | `TRIGGER._5_G5_WAREDOORZOE`                | 5_G5.dat                                                                                     |
|  845 | 5_G5_Zone01                     | `TRIGGER._5_G5_ZONE01`                     | 5_G5.dat                                                                                     |
|  846 | 5_G5_Zone02                     | `TRIGGER._5_G5_ZONE02`                     | 5_G5.dat                                                                                     |
|  847 | 5_G5_Zone03                     | `TRIGGER._5_G5_ZONE03`                     | 5_G5.dat                                                                                     |
|  848 | 5_G5_Zone04                     | `TRIGGER._5_G5_ZONE04`                     | 5_G5.dat                                                                                     |
|  849 | 5_G5_finish                     | `TRIGGER._5_G5_FINISH`                     | 5_G5.dat                                                                                     |
|  850 | 5_G5_meet_zoe                   | `TRIGGER._5_G5_MEET_ZOE`                   | 5_G5.dat                                                                                     |
|  851 | 5_T1_BikeGarage                 | `TRIGGER._5_T1_BIKEGARAGE`                 | 3_R07.dat                                                                                    |
|  852 | 602_LibEntrance                 | `TRIGGER._602_LIBENTRANCE`                 | 6_02.dat                                                                                     |
|  853 | 6_01_PRINCIPALTRIG              | `TRIGGER._6_01_PRINCIPALTRIG`              | 6_01.dat                                                                                     |
|  854 | 6_02A_BACKROUTE_STUDENTS        | `TRIGGER._6_02A_BACKROUTE_STUDENTS`        | 6_02a.dat                                                                                    |
|  855 | 6_02A_IA_COPS                   | `TRIGGER._6_02A_IA_COPS`                   | 6_02a.dat                                                                                    |
|  856 | 6_02A_SCHOOLFRONT_COPS          | `TRIGGER._6_02A_SCHOOLFRONT_COPS`          | 6_02a.dat                                                                                    |
|  857 | 6_02A_SF_GIRLS                  | `TRIGGER._6_02A_SF_GIRLS`                  | 6_02a.dat                                                                                    |
|  858 | 6_02_WonderMeats                | `TRIGGER._6_02_WONDERMEATS`                | 6_02.dat                                                                                     |
|  859 | 6_02g_bottomStairs              | `TRIGGER._6_02G_BOTTOMSTAIRS`              | 6_02gdorm.dat                                                                                |
|  860 | 6_02g_downstairs                | `TRIGGER._6_02G_DOWNSTAIRS`                | 6_02gdorm.dat                                                                                |
|  861 | 6_02g_entrance                  | `TRIGGER._6_02G_ENTRANCE`                  | 6_02gdorm.dat                                                                                |
|  862 | 6_02g_fireVase02                | `TRIGGER._6_02G_FIREVASE02`                | 6_02gdorm.dat                                                                                |
|  863 | 6_02g_johnny                    | `TRIGGER._6_02G_JOHNNY`                    | 6_02gdorm.dat                                                                                |
|  864 | 6_02g_livingroom                | `TRIGGER._6_02G_LIVINGROOM`                | 6_02gdorm.dat                                                                                |
|  865 | 6_02g_loadPeds                  | `TRIGGER._6_02G_LOADPEDS`                  | 6_02gdorm.dat                                                                                |
|  866 | 6_02g_norton                    | `TRIGGER._6_02G_NORTON`                    | 6_02gdorm.dat                                                                                |
|  867 | 6_02g_vase01                    | `TRIGGER._6_02G_VASE01`                    | 6_02gdorm.dat                                                                                |
|  868 | 6_02g_vase02                    | `TRIGGER._6_02G_VASE02`                    | 6_02gdorm.dat                                                                                |
|  869 | 6_02g_vase03                    | `TRIGGER._6_02G_VASE03`                    | 6_02gdorm.dat                                                                                |
|  870 | 6_03_Fail01                     | `TRIGGER._6_03_FAIL01`                     | 6_02.dat                                                                                     |
|  871 | 6_03_Fail02                     | `TRIGGER._6_03_FAIL02`                     | 6_02.dat                                                                                     |
|  872 | 6_03_Fail03                     | `TRIGGER._6_03_FAIL03`                     | 6_02.dat                                                                                     |
|  873 | 6_03_GetAway                    | `TRIGGER._6_03_GETAWAY`                    | 6_02.dat                                                                                     |
|  874 | 6_03_GymPop                     | `TRIGGER._6_03_GYMPOP`                     | 6_02.dat                                                                                     |
|  875 | 6_03_HallPopOverride            | `TRIGGER._6_03_HALLPOPOVERRIDE`            | 6_02.dat                                                                                     |
|  876 | 6_03_NISJOCK01                  | `TRIGGER._6_03_NISJOCK01`                  | 6_02.dat                                                                                     |
|  877 | 6_03_NISJOCK02                  | `TRIGGER._6_03_NISJOCK02`                  | 6_02.dat                                                                                     |
|  878 | 6_03_NISJOCK03                  | `TRIGGER._6_03_NISJOCK03`                  | 6_02.dat                                                                                     |
|  879 | 6_03_NISJOCK04                  | `TRIGGER._6_03_NISJOCK04`                  | 6_02.dat                                                                                     |
|  880 | 6_03_NISNERD01                  | `TRIGGER._6_03_NISNERD01`                  | 6_02.dat                                                                                     |
|  881 | 6_03_NISNERD02                  | `TRIGGER._6_03_NISNERD02`                  | 6_02.dat                                                                                     |
|  882 | 6_03_NISNERD03                  | `TRIGGER._6_03_NISNERD03`                  | 6_02.dat                                                                                     |
|  883 | 6_03_NISNERD04                  | `TRIGGER._6_03_NISNERD04`                  | 6_02.dat                                                                                     |
|  884 | 6_03_NISNERD05                  | `TRIGGER._6_03_NISNERD05`                  | 6_02.dat                                                                                     |
|  885 | 6_03_WarnFail01                 | `TRIGGER._6_03_WARNFAIL01`                 | 6_02.dat                                                                                     |
|  886 | 6_03_WarnFail02                 | `TRIGGER._6_03_WARNFAIL02`                 | 6_02.dat                                                                                     |
|  887 | 6_03_WarnFail03                 | `TRIGGER._6_03_WARNFAIL03`                 | 6_02.dat                                                                                     |
|  888 | 6_B_BELLS_ONE                   | `TRIGGER._6_B_BELLS_ONE`                   | 6_Ba.dat                                                                                     |
|  889 | 6_B_BELLS_THREE                 | `TRIGGER._6_B_BELLS_THREE`                 | 6_Ba.dat                                                                                     |
|  890 | 6_B_BELLS_TWO                   | `TRIGGER._6_B_BELLS_TWO`                   | 6_Ba.dat                                                                                     |
|  891 | 6_B_FIRSTPLANKRUN               | `TRIGGER._6_B_FIRSTPLANKRUN`               | 6_Ba.dat                                                                                     |
|  892 | 6_B_GARY_THROW_1                | `TRIGGER._6_B_GARY_THROW_1`                | 6_Ba.dat                                                                                     |
|  893 | 6_B_GARY_THROW_2                | `TRIGGER._6_B_GARY_THROW_2`                | 6_Ba.dat                                                                                     |
|  894 | 6_B_GARY_TRIGGER_1              | `TRIGGER._6_B_GARY_TRIGGER_1`              | 6_Ba.dat                                                                                     |
|  895 | 6_B_GARY_TRIGGER_2              | `TRIGGER._6_B_GARY_TRIGGER_2`              | 6_Ba.dat                                                                                     |
|  896 | 6_B_GARY_TRIGGER_3              | `TRIGGER._6_B_GARY_TRIGGER_3`              | 6_Ba.dat                                                                                     |
|  897 | 6_B_GARY_TRIGGER_4              | `TRIGGER._6_B_GARY_TRIGGER_4`              | 6_Ba.dat                                                                                     |
|  898 | 6_B_GARY_TRIGGER_5              | `TRIGGER._6_B_GARY_TRIGGER_5`              | 6_Ba.dat                                                                                     |
|  899 | 6_B_GARY_TRIGGER_6              | `TRIGGER._6_B_GARY_TRIGGER_6`              | 6_Ba.dat                                                                                     |
|  900 | 6_B_GLASS_TRIGGER               | `TRIGGER._6_B_GLASS_TRIGGER`               | 6_Ba.dat                                                                                     |
|  901 | 6_B_LADDER1_BEGIN               | `TRIGGER._6_B_LADDER1_BEGIN`               | 6_Ba.dat                                                                                     |
|  902 | 6_B_LADDER2_BEGIN               | `TRIGGER._6_B_LADDER2_BEGIN`               | 6_Ba.dat                                                                                     |
|  903 | 6_B_OFFROOF                     | `TRIGGER._6_B_OFFROOF`                     | 6_Ba.dat                                                                                     |
|  904 | 6_B_START                       | `TRIGGER._6_B_START`                       | 6_Ba.dat                                                                                     |
|  905 | 6_B_SchoolRoofTop               | `TRIGGER._6_B_SCHOOLROOFTOP`               | 6_Ba.dat                                                                                     |
|  906 | AMB_BUSINESS_AREA               | `TRIGGER._AMB_BUSINESS_AREA`               | SoundTriggers.dat                                                                            |
|  907 | AMB_Beach02_ISLAND              | `TRIGGER._AMB_BEACH02_ISLAND`              | SoundTriggers.dat                                                                            |
|  908 | AMB_CARNIVAL_AREA               | `TRIGGER._AMB_CARNIVAL_AREA`               | SoundTriggers.dat                                                                            |
|  909 | AMB_CHEMLAB                     | `TRIGGER._AMB_CHEMLAB`                     | SP_Chem_Lab.dat                                                                              |
|  910 | AMB_ForestBeachTunnel           | `TRIGGER._AMB_FORESTBEACHTUNNEL`           | SoundTriggers.dat                                                                            |
|  911 | AMB_HOBOAREA                    | `TRIGGER._AMB_HOBOAREA`                    | SoundTriggers.dat                                                                            |
|  912 | AMB_INDUSTRIAL_AREA             | `TRIGGER._AMB_INDUSTRIAL_AREA`             | SoundTriggers.dat                                                                            |
|  913 | AMB_JunkYard_AREA               | `TRIGGER._AMB_JUNKYARD_AREA`               | SP_JunkYard.dat                                                                              |
|  914 | AMB_Openwater                   | `TRIGGER._AMB_OPENWATER`                   | SoundTriggers.dat                                                                            |
|  915 | AMB_POOR_AREA                   | `TRIGGER._AMB_POOR_AREA`                   | SoundTriggers.dat                                                                            |
|  916 | AMB_RICH_AREA                   | `TRIGGER._AMB_RICH_AREA`                   | SoundTriggers.dat                                                                            |
|  917 | AMB_RIVER                       | `TRIGGER._AMB_RIVER`                       | SoundTriggers.dat                                                                            |
|  918 | AMB_RIVER03                     | `TRIGGER._AMB_RIVER03`                     | SoundTriggers.dat                                                                            |
|  919 | AMB_RIVER04                     | `TRIGGER._AMB_RIVER04`                     | SoundTriggers.dat                                                                            |
|  920 | AMB_RIVERDAM                    | `TRIGGER._AMB_RIVERDAM`                    | SoundTriggers.dat                                                                            |
|  921 | AMB_RIVER_DOCK                  | `TRIGGER._AMB_RIVER_DOCK`                  | SoundTriggers.dat                                                                            |
|  922 | AMB_SCHOOL_AREA                 | `TRIGGER._AMB_SCHOOL_AREA`                 | SoundTriggers.dat                                                                            |
|  923 | AMB_SmallBeachForest            | `TRIGGER._AMB_SMALLBEACHFOREST`            | SoundTriggers.dat                                                                            |
|  924 | AREA_AROUND_BUTTON              | `TRIGGER._AREA_AROUND_BUTTON`              | 3_B.dat                                                                                      |
|  925 | ASYLUM_FRONT_DOOR_R             | `TRIGGER._ASYLUM_FRONT_DOOR_R`             | PAn_Main.dat                                                                                 |
|  926 | ASYLUM_FRONT_GATE_DOOR          | `TRIGGER._ASYLUM_FRONT_GATE_DOOR`          | PAn_Main.dat                                                                                 |
|  927 | AcrossGymBack                   | `TRIGGER._ACROSSGYMBACK`                   | C5.dat, PhotoZoom.dat                                                                        |
|  928 | AfterSteam                      | `TRIGGER._AFTERSTEAM`                      | Janitors.dat                                                                                 |
|  929 | AlleyPiss1                      | `TRIGGER._ALLEYPISS1`                      | PAn_Main.dat                                                                                 |
|  930 | AlleyPiss2                      | `TRIGGER._ALLEYPISS2`                      | PAn_Main.dat                                                                                 |
|  931 | AlleyPiss3                      | `TRIGGER._ALLEYPISS3`                      | PAn_Main.dat                                                                                 |
|  932 | Amb_Carnival_Tunnel             | `TRIGGER._AMB_CARNIVAL_TUNNEL`             | SoundTriggers.dat                                                                            |
|  933 | Amb_ClassRoom                   | `TRIGGER._AMB_CLASSROOM`                   | SP_ClassRoom.dat                                                                             |
|  934 | Amb_ForestTrainTunnels          | `TRIGGER._AMB_FORESTTRAINTUNNELS`          | SoundTriggers.dat                                                                            |
|  935 | Amb_ForestTunnels               | `TRIGGER._AMB_FORESTTUNNELS`               | SoundTriggers.dat                                                                            |
|  936 | Amb_RichAreaCliff               | `TRIGGER._AMB_RICHAREACLIFF`               | SoundTriggers.dat                                                                            |
|  937 | Amb_SchoolRoofTop               | `TRIGGER._AMB_SCHOOLROOFTOP`               | SoundTriggers.dat                                                                            |
|  938 | Amb_TownHallRoofTop             | `TRIGGER._AMB_TOWNHALLROOFTOP`             | SoundTriggers.dat                                                                            |
|  939 | AmbientEvent1                   | `TRIGGER._AMBIENTEVENT1`                   | 3_06New.dat                                                                                  |
|  940 | AmbientEvent2                   | `TRIGGER._AMBIENTEVENT2`                   | 3_06New.dat                                                                                  |
|  941 | AngelStatue                     | `TRIGGER._ANGELSTATUE`                     | C5.dat, PhotoZoom.dat                                                                        |
|  942 | AniBroom                        | `TRIGGER._ANIBROOM`                        | Janitors.dat                                                                                 |
|  943 | Armor                           | `TRIGGER._ARMOR`                           | ttest.dat                                                                                    |
|  944 | Art_Room                        | `TRIGGER._ART_ROOM`                        | SP_Art_Room.dat                                                                              |
|  945 | AssyInterTone01                 | `TRIGGER._ASSYINTERTONE01`                 | SP_Asylum.dat                                                                                |
|  946 | AssyMain02                      | `TRIGGER._ASSYMAIN02`                      | SP_Asylum.dat                                                                                |
|  947 | AssyMainDamaged                 | `TRIGGER._ASSYMAINDAMAGED`                 | SP_Asylum.dat                                                                                |
|  948 | AssyRecRoom                     | `TRIGGER._ASSYRECROOM`                     | SP_Asylum.dat                                                                                |
|  949 | AssyShowers                     | `TRIGGER._ASSYSHOWERS`                     | SP_Asylum.dat                                                                                |
|  950 | AssylumMain                     | `TRIGGER._ASSYLUMMAIN`                     | SP_Asylum.dat                                                                                |
|  951 | AsyBars                         | `TRIGGER._ASYBARS`                         | 5_03.dat                                                                                     |
|  952 | AsyBars01                       | `TRIGGER._ASYBARS01`                       | 5_03.dat                                                                                     |
|  953 | AsyBars02                       | `TRIGGER._ASYBARS02`                       | 5_03.dat                                                                                     |
|  954 | AsyDoorB                        | `TRIGGER._ASYDOORB`                        | iasylum.dat                                                                                  |
|  955 | AsyDoors                        | `TRIGGER._ASYDOORS`                        | iasylum.dat                                                                                  |
|  956 | AsyDoors10                      | `TRIGGER._ASYDOORS10`                      | iasylum.dat                                                                                  |
|  957 | AsyDoors11                      | `TRIGGER._ASYDOORS11`                      | iasylum.dat                                                                                  |
|  958 | AsyDoors12                      | `TRIGGER._ASYDOORS12`                      | iasylum.dat                                                                                  |
|  959 | AsyDoors13                      | `TRIGGER._ASYDOORS13`                      | iasylum.dat                                                                                  |
|  960 | AsyDoors14                      | `TRIGGER._ASYDOORS14`                      | iasylum.dat                                                                                  |
|  961 | AsyDoors15                      | `TRIGGER._ASYDOORS15`                      | iasylum.dat                                                                                  |
|  962 | Asylum                          | `TRIGGER._ASYLUM`                          | SoundTriggers.dat                                                                            |
|  963 | AsylumPatrols                   | `TRIGGER._ASYLUMPATROLS`                   | eventsAsylum.dat                                                                             |
|  964 | AudioStPinkBankTest             | `TRIGGER._AUDIOSTPINKBANKTEST`             | SP_Test_Area.dat                                                                             |
|  965 | AudioStereoBankTest             | `TRIGGER._AUDIOSTEREOBANKTEST`             | SP_Test_Area.dat                                                                             |
|  966 | AudioStereoStreamTest           | `TRIGGER._AUDIOSTEREOSTREAMTEST`           | SP_Test_Area.dat                                                                             |
|  967 | AudioSteroPinkStreamTest        | `TRIGGER._AUDIOSTEROPINKSTREAMTEST`        | SP_Test_Area.dat                                                                             |
|  968 | AudioSurrBankTest               | `TRIGGER._AUDIOSURRBANKTEST`               | SP_Test_Area.dat                                                                             |
|  969 | AudioSurrPinkBankTest           | `TRIGGER._AUDIOSURRPINKBANKTEST`           | SP_Test_Area.dat                                                                             |
|  970 | AudioSurrPinkStreamTest         | `TRIGGER._AUDIOSURRPINKSTREAMTEST`         | SP_Test_Area.dat                                                                             |
|  971 | AudioSurrndStreamTest           | `TRIGGER._AUDIOSURRNDSTREAMTEST`           | SP_Test_Area.dat                                                                             |
|  972 | Auditorium                      | `TRIGGER._AUDITORIUM`                      | SP_Auditorium.dat                                                                            |
|  973 | AutoGarage                      | `TRIGGER._AUTOGARAGE`                      | C5.dat, PhotoZoom.dat                                                                        |
|  974 | AutoShop                        | `TRIGGER._AUTOSHOP`                        | C5.dat, PhotoZoom.dat                                                                        |
|  975 | AutoShopSide                    | `TRIGGER._AUTOSHOPSIDE`                    | C5.dat, PhotoZoom.dat                                                                        |
|  976 | BA_BMXGarage                    | `TRIGGER._BA_BMXGARAGE`                    | tbusines_doors.dat                                                                           |
|  977 | BA_DoorStr01                    | `TRIGGER._BA_DOORSTR01`                    | tbusines_doors.dat                                                                           |
|  978 | BA_DoorStr02                    | `TRIGGER._BA_DOORSTR02`                    | tbusines_doors.dat                                                                           |
|  979 | BA_DoorStr03                    | `TRIGGER._BA_DOORSTR03`                    | tbusines_doors.dat                                                                           |
|  980 | BA_DoorStr04                    | `TRIGGER._BA_DOORSTR04`                    | tbusines_doors.dat                                                                           |
|  981 | BA_DoorStr05                    | `TRIGGER._BA_DOORSTR05`                    | tbusines_doors.dat                                                                           |
|  982 | BA_DoorStr07                    | `TRIGGER._BA_DOORSTR07`                    | tbusines_doors.dat                                                                           |
|  983 | BA_DoorStr08                    | `TRIGGER._BA_DOORSTR08`                    | tbusines_doors.dat                                                                           |
|  984 | BA_PrepDoor02                   | `TRIGGER._BA_PREPDOOR02`                   | tbusines_doors.dat                                                                           |
|  985 | BA_PrepDoor03                   | `TRIGGER._BA_PREPDOOR03`                   | tbusines_doors.dat                                                                           |
|  986 | BA_PrepDoor04                   | `TRIGGER._BA_PREPDOOR04`                   | tbusines_doors.dat                                                                           |
|  987 | BA_PrepDoor05                   | `TRIGGER._BA_PREPDOOR05`                   | tbusines_doors.dat                                                                           |
|  988 | BA_PrepDoor06                   | `TRIGGER._BA_PREPDOOR06`                   | tbusines_doors.dat                                                                           |
|  989 | BA_PrepDoor09                   | `TRIGGER._BA_PREPDOOR09`                   | tbusines_doors.dat                                                                           |
|  990 | BA_PrepDoor10                   | `TRIGGER._BA_PREPDOOR10`                   | tbusines_doors.dat                                                                           |
|  991 | BA_PrepDoor11                   | `TRIGGER._BA_PREPDOOR11`                   | tbusines_doors.dat                                                                           |
|  992 | BBChair                         | `TRIGGER._BBCHAIR`                         | ttest.dat                                                                                    |
|  993 | BBatter                         | `TRIGGER._BBATTER`                         | iballtos.dat                                                                                 |
|  994 | BCatcher                        | `TRIGGER._BCATCHER`                        | iballtos.dat                                                                                 |
|  995 | BD_Medium1                      | `TRIGGER._BD_MEDIUM1`                      | tags_dorm.dat                                                                                |
|  996 | BD_Medium2                      | `TRIGGER._BD_MEDIUM2`                      | tags_dorm.dat                                                                                |
|  997 | BDormFlag1                      | `TRIGGER._BDORMFLAG1`                      | C5.dat, PhotoZoom.dat                                                                        |
|  998 | BDormTarg                       | `TRIGGER._BDORMTARG`                       | PAn_Main.dat                                                                                 |
|  999 | BEACH_AREA_P                    | `TRIGGER._BEACH_AREA_P`                    | SoundTriggers.dat                                                                            |
| 1000 | BMXGate                         | `TRIGGER._BMXGATE`                         | ttest.dat                                                                                    |
| 1001 | BMXParkJump01                   | `TRIGGER._BMXPARKJUMP01`                   | 3_02_BMX.dat                                                                                 |
| 1002 | BMX_BigRoom                     | `TRIGGER._BMX_BIGROOM`                     | SP_BMXTrack.dat                                                                              |
| 1003 | BMX_GarageDoor                  | `TRIGGER._BMX_GARAGEDOOR`                  | tBMX.dat                                                                                     |
| 1004 | BMX_Room                        | `TRIGGER._BMX_ROOM`                        | SP_BMXTrack.dat                                                                              |
| 1005 | BMX_Warning_Trig                | `TRIGGER._BMX_WARNING_TRIG`                | BMX_Rumble.dat                                                                               |
| 1006 | BNews                           | `TRIGGER._BNEWS`                           | ttest.dat                                                                                    |
| 1007 | BSign                           | `TRIGGER._BSIGN`                           | ttest.dat                                                                                    |
| 1008 | BTable                          | `TRIGGER._BTABLE`                          | ttest.dat                                                                                    |
| 1009 | BUS_SODA_01                     | `TRIGGER._BUS_SODA_01`                     | SndBnkLoad.dat                                                                               |
| 1010 | BUmpire                         | `TRIGGER._BUMPIRE`                         | iballtos.dat                                                                                 |
| 1011 | BXPBag                          | `TRIGGER._BXPBAG`                          | iboxing_punchingbags.dat                                                                     |
| 1012 | BXPBag01                        | `TRIGGER._BXPBAG01`                        | iboxing_punchingbags.dat                                                                     |
| 1013 | BXPBag02                        | `TRIGGER._BXPBAG02`                        | iboxing_punchingbags.dat                                                                     |
| 1014 | BadPlaceTrigger                 | `TRIGGER._BADPLACETRIGGER`                 | Population.dat                                                                               |
| 1015 | BalanceBeam                     | `TRIGGER._BALANCEBEAM`                     | ttest.dat                                                                                    |
| 1016 | BarberShop                      | `TRIGGER._BARBERSHOP`                      | SP_Barber.dat, SP_Pool.dat                                                                   |
| 1017 | BathroomExit                    | `TRIGGER._BATHROOMEXIT`                    | 1_08.dat                                                                                     |
| 1018 | BathroomLeftTrig                | `TRIGGER._BATHROOMLEFTTRIG`                | 1_08.dat                                                                                     |
| 1019 | BathroomRightTrig               | `TRIGGER._BATHROOMRIGHTTRIG`               | 1_08.dat                                                                                     |
| 1020 | BatterEight                     | `TRIGGER._BATTEREIGHT`                     | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1021 | BatterFive                      | `TRIGGER._BATTERFIVE`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1022 | BatterFour                      | `TRIGGER._BATTERFOUR`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1023 | BatterNine                      | `TRIGGER._BATTERNINE`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1024 | BatterOne                       | `TRIGGER._BATTERONE`                       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1025 | BatterSeven                     | `TRIGGER._BATTERSEVEN`                     | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1026 | BatterSix                       | `TRIGGER._BATTERSIX`                       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1027 | BatterThree                     | `TRIGGER._BATTERTHREE`                     | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1028 | BatterTwo                       | `TRIGGER._BATTERTWO`                       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1029 | BdrDoorDownstairs1              | `TRIGGER._BDRDOORDOWNSTAIRS1`              | BDorm_Doors.dat                                                                              |
| 1030 | BdrDoorDownstairs2              | `TRIGGER._BDRDOORDOWNSTAIRS2`              | BDorm_Doors.dat                                                                              |
| 1031 | BdrDoorDownstairs4              | `TRIGGER._BDRDOORDOWNSTAIRS4`              | BDorm_Doors.dat                                                                              |
| 1032 | BdrDoorDownstairs5              | `TRIGGER._BDRDOORDOWNSTAIRS5`              | BDorm_Doors.dat                                                                              |
| 1033 | BdrDoorDownstairs6              | `TRIGGER._BDRDOORDOWNSTAIRS6`              | BDorm_Doors.dat                                                                              |
| 1034 | BdrDoorDownstairs7              | `TRIGGER._BDRDOORDOWNSTAIRS7`              | BDorm_Doors.dat                                                                              |
| 1035 | BdrDoorDownstairs8              | `TRIGGER._BDRDOORDOWNSTAIRS8`              | BDorm_Doors.dat                                                                              |
| 1036 | BdrDoorL                        | `TRIGGER._BDRDOORL`                        | iSaveZones.dat, isc_offi.dat                                                                 |
| 1037 | BdrDoorL01                      | `TRIGGER._BDRDOORL01`                      | iSaveZones.dat                                                                               |
| 1038 | BdrDoorL02                      | `TRIGGER._BDRDOORL02`                      | iSaveZones.dat                                                                               |
| 1039 | BeachNoGoArea                   | `TRIGGER._BEACHNOGOAREA`                   | GoKart_Outdoor.dat                                                                           |
| 1040 | BeatriceCutsceneTrigger         | `TRIGGER._BEATRICECUTSCENETRIGGER`         | 1_08.dat                                                                                     |
| 1041 | BeatriceTrigger                 | `TRIGGER._BEATRICETRIGGER`                 | 1_08.dat                                                                                     |
| 1042 | BellTowerCamera                 | `TRIGGER._BELLTOWERCAMERA`                 | 6_B.dat                                                                                      |
| 1043 | BenchA                          | `TRIGGER._BENCHA`                          | ttest.dat                                                                                    |
| 1044 | BenchB                          | `TRIGGER._BENCHB`                          | ttest.dat                                                                                    |
| 1045 | BenchC                          | `TRIGGER._BENCHC`                          | ttest.dat                                                                                    |
| 1046 | BigTag1                         | `TRIGGER._BIGTAG1`                         | GraffitiTest.dat                                                                             |
| 1047 | BigTag2                         | `TRIGGER._BIGTAG2`                         | GraffitiTest.dat                                                                             |
| 1048 | BigTag3                         | `TRIGGER._BIGTAG3`                         | GraffitiTest.dat                                                                             |
| 1049 | BikeBusiness                    | `TRIGGER._BIKEBUSINESS`                    | AreaTran.dat                                                                                 |
| 1050 | BikeFire01                      | `TRIGGER._BIKEFIRE01`                      | 5_07.dat                                                                                     |
| 1051 | BikeFire02                      | `TRIGGER._BIKEFIRE02`                      | 5_07.dat                                                                                     |
| 1052 | BikeFire03                      | `TRIGGER._BIKEFIRE03`                      | 5_07.dat                                                                                     |
| 1053 | BikeFire04                      | `TRIGGER._BIKEFIRE04`                      | 5_07.dat                                                                                     |
| 1054 | BikeFire05                      | `TRIGGER._BIKEFIRE05`                      | 5_07.dat                                                                                     |
| 1055 | BikeFire06                      | `TRIGGER._BIKEFIRE06`                      | 5_07.dat                                                                                     |
| 1056 | BikeShop                        | `TRIGGER._BIKESHOP`                        | SP_Bike_Shop.dat                                                                             |
| 1057 | BitchDice                       | `TRIGGER._BITCHDICE`                       | 1_08.dat                                                                                     |
| 1058 | BitchFight1                     | `TRIGGER._BITCHFIGHT1`                     | 6_02.dat                                                                                     |
| 1059 | BitchFight2                     | `TRIGGER._BITCHFIGHT2`                     | 6_02.dat                                                                                     |
| 1060 | BleachersL                      | `TRIGGER._BLEACHERSL`                      | C5.dat, PhotoZoom.dat                                                                        |
| 1061 | BleachersR                      | `TRIGGER._BLEACHERSR`                      | C5.dat, PhotoZoom.dat                                                                        |
| 1062 | BonusTarget                     | `TRIGGER._BONUSTARGET`                     | MGBaseballToss.dat                                                                           |
| 1063 | BottleB                         | `TRIGGER._BOTTLEB`                         | ttest.dat                                                                                    |
| 1064 | BottleC                         | `TRIGGER._BOTTLEC`                         | ttest.dat                                                                                    |
| 1065 | BottleD                         | `TRIGGER._BOTTLED`                         | ttest.dat                                                                                    |
| 1066 | BottleE                         | `TRIGGER._BOTTLEE`                         | ttest.dat                                                                                    |
| 1067 | Box2ndFloor                     | `TRIGGER._BOX2NDFLOOR`                     | SP_BoxingRing.dat                                                                            |
| 1068 | BoxHalfTheRing                  | `TRIGGER._BOXHALFTHERING`                  | Boxing.dat                                                                                   |
| 1069 | BoxMain01                       | `TRIGGER._BOXMAIN01`                       | SP_BoxingRing.dat                                                                            |
| 1070 | BoxMain02                       | `TRIGGER._BOXMAIN02`                       | SP_BoxingRing.dat                                                                            |
| 1071 | BoxRopes                        | `TRIGGER._BOXROPES`                        | ttest.dat                                                                                    |
| 1072 | BoxStairs                       | `TRIGGER._BOXSTAIRS`                       | SP_BoxingRing.dat                                                                            |
| 1073 | BoxingTurfTrigger               | `TRIGGER._BOXINGTURFTRIGGER`               | eventsBoxing.dat                                                                             |
| 1074 | Boxing_Corner1                  | `TRIGGER._BOXING_CORNER1`                  | Boxing.dat                                                                                   |
| 1075 | Boxing_Corner2                  | `TRIGGER._BOXING_CORNER2`                  | Boxing.dat                                                                                   |
| 1076 | Boxing_Corner3                  | `TRIGGER._BOXING_CORNER3`                  | Boxing.dat                                                                                   |
| 1077 | Boxing_Corner4                  | `TRIGGER._BOXING_CORNER4`                  | Boxing.dat                                                                                   |
| 1078 | Boxing_Tether                   | `TRIGGER._BOXING_TETHER`                   | eventsBoxing.dat                                                                             |
| 1079 | Boxtest                         | `TRIGGER._BOXTEST`                         | SpawnTest.dat                                                                                |
| 1080 | BoysBathroom1                   | `TRIGGER._BOYSBATHROOM1`                   | eventsSchoolHalls.dat                                                                        |
| 1081 | BoysBathroom2                   | `TRIGGER._BOYSBATHROOM2`                   | eventsSchoolHalls.dat                                                                        |
| 1082 | BoysDormMain                    | `TRIGGER._BOYSDORMMAIN`                    | AreaTran.dat                                                                                 |
| 1083 | BoysDorm_GameRm                 | `TRIGGER._BOYSDORM_GAMERM`                 | SP_BoysDorm.dat                                                                              |
| 1084 | BoysDorm_Halls                  | `TRIGGER._BOYSDORM_HALLS`                  | SP_BoysDorm.dat                                                                              |
| 1085 | BoysDorm_JimmysRoom             | `TRIGGER._BOYSDORM_JIMMYSROOM`             | SP_BoysDorm.dat                                                                              |
| 1086 | BuckyCutsceneTrigger            | `TRIGGER._BUCKYCUTSCENETRIGGER`            | 1_08.dat                                                                                     |
| 1087 | BuckyTrigger                    | `TRIGGER._BUCKYTRIGGER`                    | 1_08.dat                                                                                     |
| 1088 | BullyTurf                       | `TRIGGER._BULLYTURF`                       | Population.dat                                                                               |
| 1089 | Burger                          | `TRIGGER._BURGER`                          | PhotoFilters.dat                                                                             |
| 1090 | BusDoors                        | `TRIGGER._BUSDOORS`                        | tschool_maindoors.dat                                                                        |
| 1091 | Bus_BUS                         | `TRIGGER._BUS_BUS`                         | MainMap_bus.dat                                                                              |
| 1092 | Bus_Loc1                        | `TRIGGER._BUS_LOC1`                        | MainMap_bus.dat                                                                              |
| 1093 | Bus_Loc3                        | `TRIGGER._BUS_LOC3`                        | MainMap_bus.dat                                                                              |
| 1094 | Bus_Loc4                        | `TRIGGER._BUS_LOC4`                        | MainMap_bus.dat                                                                              |
| 1095 | Bus_Loc5                        | `TRIGGER._BUS_LOC5`                        | MainMap_bus.dat                                                                              |
| 1096 | Bus_Loc6                        | `TRIGGER._BUS_LOC6`                        | MainMap_bus.dat                                                                              |
| 1097 | Bus_Loc7                        | `TRIGGER._BUS_LOC7`                        | MainMap_bus.dat                                                                              |
| 1098 | Bus_Loc8                        | `TRIGGER._BUS_LOC8`                        | MainMap_bus.dat                                                                              |
| 1099 | Bus_Loc9                        | `TRIGGER._BUS_LOC9`                        | MainMap_bus.dat                                                                              |
| 1100 | Bus_LocX                        | `TRIGGER._BUS_LOCX`                        | MainMap_bus.dat                                                                              |
| 1101 | BusinessBike                    | `TRIGGER._BUSINESSBIKE`                    | AreaTran.dat                                                                                 |
| 1102 | BusinessFirework                | `TRIGGER._BUSINESSFIREWORK`                | AreaTran.dat                                                                                 |
| 1103 | BusinessGrocery                 | `TRIGGER._BUSINESSGROCERY`                 | AreaTran.dat                                                                                 |
| 1104 | C3_MAT_BOUNDARY                 | `TRIGGER._C3_MAT_BOUNDARY`                 | C3.dat                                                                                       |
| 1105 | C5T_POP                         | `TRIGGER._C5T_POP`                         | Chapt5Trans.dat                                                                              |
| 1106 | C5_PedEvent01                   | `TRIGGER._C5_PEDEVENT01`                   | C5.dat                                                                                       |
| 1107 | C5_PedEvent02                   | `TRIGGER._C5_PEDEVENT02`                   | C5.dat                                                                                       |
| 1108 | C5_PedEvent03                   | `TRIGGER._C5_PEDEVENT03`                   | C5.dat                                                                                       |
| 1109 | C5_WorkingOut1                  | `TRIGGER._C5_WORKINGOUT1`                  | C5.dat                                                                                       |
| 1110 | C5_WorkingOut2                  | `TRIGGER._C5_WORKINGOUT2`                  | C5.dat                                                                                       |
| 1111 | C5_WorkingOut3                  | `TRIGGER._C5_WORKINGOUT3`                  | C5.dat                                                                                       |
| 1112 | C6_ShopBike                     | `TRIGGER._C6_SHOPBIKE`                     | C6.dat                                                                                       |
| 1113 | CARNY_ENTRANCE                  | `TRIGGER._CARNY_ENTRANCE`                  | MiniGameTrigger.dat                                                                          |
| 1114 | CARNY_GAMESAREA                 | `TRIGGER._CARNY_GAMESAREA`                 | MiniGameTrigger.dat                                                                          |
| 1115 | CARNY_GOKARTAREA                | `TRIGGER._CARNY_GOKARTAREA`                | MiniGameTrigger.dat                                                                          |
| 1116 | CHTrespass                      | `TRIGGER._CHTRESPASS`                      | mm_retirement.dat                                                                            |
| 1117 | CafBackTrigger                  | `TRIGGER._CAFBACKTRIGGER`                  | 1_08.dat                                                                                     |
| 1118 | CafTrigger                      | `TRIGGER._CAFTRIGGER`                      | eventsSchoolHalls.dat                                                                        |
| 1119 | Carn_Tunnel_Reverb              | `TRIGGER._CARN_TUNNEL_REVERB`              | SoundTriggers.dat                                                                            |
| 1120 | Carnival                        | `TRIGGER._CARNIVAL`                        | Population.dat                                                                               |
| 1121 | CatcherFive                     | `TRIGGER._CATCHERFIVE`                     | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1122 | CatcherFour                     | `TRIGGER._CATCHERFOUR`                     | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1123 | CatcherOne                      | `TRIGGER._CATCHERONE`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1124 | CatcherSeven                    | `TRIGGER._CATCHERSEVEN`                    | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1125 | CatcherSix                      | `TRIGGER._CATCHERSIX`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1126 | CatcherThree                    | `TRIGGER._CATCHERTHREE`                    | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1127 | CatcherTwo                      | `TRIGGER._CATCHERTWO`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 1128 | CellDoor                        | `TRIGGER._CELLDOOR`                        | iasylum.dat                                                                                  |
| 1129 | CellDoor12                      | `TRIGGER._CELLDOOR12`                      | iasylum.dat                                                                                  |
| 1130 | CellDoor13                      | `TRIGGER._CELLDOOR13`                      | iasylum.dat                                                                                  |
| 1131 | CellDoor14                      | `TRIGGER._CELLDOOR14`                      | iasylum.dat                                                                                  |
| 1132 | CellDoor15                      | `TRIGGER._CELLDOOR15`                      | iasylum.dat                                                                                  |
| 1133 | CellDoor16                      | `TRIGGER._CELLDOOR16`                      | iasylum.dat                                                                                  |
| 1134 | CellDoor17                      | `TRIGGER._CELLDOOR17`                      | iasylum.dat                                                                                  |
| 1135 | CellDoor18                      | `TRIGGER._CELLDOOR18`                      | iasylum.dat                                                                                  |
| 1136 | CellDoor19                      | `TRIGGER._CELLDOOR19`                      | iasylum.dat                                                                                  |
| 1137 | CellDoor20                      | `TRIGGER._CELLDOOR20`                      | iasylum.dat                                                                                  |
| 1138 | CellDoor21                      | `TRIGGER._CELLDOOR21`                      | iasylum.dat                                                                                  |
| 1139 | Cemetary                        | `TRIGGER._CEMETARY`                        | SoundTriggers.dat                                                                            |
| 1140 | Chair1                          | `TRIGGER._CHAIR1`                          | PedTest.dat                                                                                  |
| 1141 | Chair2                          | `TRIGGER._CHAIR2`                          | PedTest.dat                                                                                  |
| 1142 | ChangeRoom                      | `TRIGGER._CHANGEROOM`                      | 1_08.dat                                                                                     |
| 1143 | CheerleadersTrigger             | `TRIGGER._CHEERLEADERSTRIGGER`             | 1_08.dat                                                                                     |
| 1144 | ChemPlantAcid01                 | `TRIGGER._CHEMPLANTACID01`                 | ChemPlantAcid01.dat                                                                          |
| 1145 | ChemPlantLower                  | `TRIGGER._CHEMPLANTLOWER`                  | SP_Chem_Plant.dat                                                                            |
| 1146 | ChemPlantMain                   | `TRIGGER._CHEMPLANTMAIN`                   | SP_Chem_Plant.dat                                                                            |
| 1147 | ChemPlantStairTunnel            | `TRIGGER._CHEMPLANTSTAIRTUNNEL`            | SP_Chem_Plant.dat                                                                            |
| 1148 | Chemical_Plant_Roof             | `TRIGGER._CHEMICAL_PLANT_ROOF`             | SoundTriggers.dat                                                                            |
| 1149 | ChezLouis                       | `TRIGGER._CHEZLOUIS`                       | trich_doors.dat                                                                              |
| 1150 | ChristmasTreeExclude            | `TRIGGER._CHRISTMASTREEEXCLUDE`            | ChristmasTree.dat                                                                            |
| 1151 | CityHall                        | `TRIGGER._CITYHALL`                        | PhotoFilters.dat                                                                             |
| 1152 | CityHallTarg                    | `TRIGGER._CITYHALLTARG`                    | PAn_Main.dat                                                                                 |
| 1153 | Coaster                         | `TRIGGER._COASTER`                         | tcarni.dat                                                                                   |
| 1154 | CoasterExitTrigger              | `TRIGGER._COASTEREXITTRIGGER`              | CarnivalRides.dat                                                                            |
| 1155 | ComicBedExclude                 | `TRIGGER._COMICBEDEXCLUDE`                 | Store.dat                                                                                    |
| 1156 | ComicPopTrig                    | `TRIGGER._COMICPOPTRIG`                    | Store.dat                                                                                    |
| 1157 | ComicShop                       | `TRIGGER._COMICSHOP`                       | SP_Comic_Shop_Rich.dat                                                                       |
| 1158 | ComicShopExclude                | `TRIGGER._COMICSHOPEXCLUDE`                | Population.dat                                                                               |
| 1159 | CopCar                          | `TRIGGER._COPCAR`                          | 6_02.dat                                                                                     |
| 1160 | Corner_Check1                   | `TRIGGER._CORNER_CHECK1`                   | Boxing.dat                                                                                   |
| 1161 | Corner_Check3                   | `TRIGGER._CORNER_CHECK3`                   | Boxing.dat                                                                                   |
| 1162 | CrateBrk                        | `TRIGGER._CRATEBRK`                        | ttest.dat                                                                                    |
| 1163 | Cutscene02                      | `TRIGGER._CUTSCENE02`                      | 2_09.dat                                                                                     |
| 1164 | DISABLED_SV_LibMain             | `TRIGGER._DISABLED_SV_LIBMAIN`             | AreaTran.dat                                                                                 |
| 1165 | DRBrace                         | `TRIGGER._DRBRACE`                         | 2_B.dat                                                                                      |
| 1166 | DRBrace01                       | `TRIGGER._DRBRACE01`                       | 2_B.dat                                                                                      |
| 1167 | DRPDoor                         | `TRIGGER._DRPDOOR`                         | iSaveZones.dat                                                                               |
| 1168 | DRPDoor01                       | `TRIGGER._DRPDOOR01`                       | iSaveZones.dat                                                                               |
| 1169 | DT_ASYLUM_BACK_EXIT             | `TRIGGER._DT_ASYLUM_BACK_EXIT`             | iasylum.dat                                                                                  |
| 1170 | DT_ASYLUM_EXITL                 | `TRIGGER._DT_ASYLUM_EXITL`                 | iasylum.dat                                                                                  |
| 1171 | DT_ASYLUM_FRONT_DOOR            | `TRIGGER._DT_ASYLUM_FRONT_DOOR`            | PAn_Main.dat                                                                                 |
| 1172 | DT_ASYLUM_SIDE_EXIT             | `TRIGGER._DT_ASYLUM_SIDE_EXIT`             | PAn_Main.dat                                                                                 |
| 1173 | DT_BMXGarage                    | `TRIGGER._DT_BMXGARAGE`                    | tbusines_doors.dat                                                                           |
| 1174 | DT_BMXGarageDoor                | `TRIGGER._DT_BMXGARAGEDOOR`                | tBMX.dat                                                                                     |
| 1175 | DT_CarnCurt01                   | `TRIGGER._DT_CARNCURT01`                   | tcarni.dat                                                                                   |
| 1176 | DT_CarnCurt02                   | `TRIGGER._DT_CARNCURT02`                   | Store.dat                                                                                    |
| 1177 | DT_ChemPlant_DoorL              | `TRIGGER._DT_CHEMPLANT_DOORL`              | iChemPlant.dat                                                                               |
| 1178 | DT_ComicShop                    | `TRIGGER._DT_COMICSHOP`                    | Population.dat                                                                               |
| 1179 | DT_DormExitDoorL                | `TRIGGER._DT_DORMEXITDOORL`                | BDorm_Doors.dat                                                                              |
| 1180 | DT_DropOutAlley                 | `TRIGGER._DT_DROPOUTALLEY`                 | Population.dat                                                                               |
| 1181 | DT_FreakEntrance                | `TRIGGER._DT_FREAKENTRANCE`                | tcarni.dat                                                                                   |
| 1182 | DT_FreakExit                    | `TRIGGER._DT_FREAKEXIT`                    | tcarni.dat                                                                                   |
| 1183 | DT_FreakShow_Entrance           | `TRIGGER._DT_FREAKSHOW_ENTRANCE`           | FreakShow.dat                                                                                |
| 1184 | DT_FreakShow_Exit               | `TRIGGER._DT_FREAKSHOW_EXIT`               | FreakShow.dat                                                                                |
| 1185 | DT_FunhouseTheaterCarnival      | `TRIGGER._DT_FUNHOUSETHEATERCARNIVAL`      | ifunhous.dat                                                                                 |
| 1186 | DT_GASSTATION                   | `TRIGGER._DT_GASSTATION`                   | Population.dat                                                                               |
| 1187 | DT_GreaserAlley                 | `TRIGGER._DT_GREASERALLEY`                 | Population.dat                                                                               |
| 1188 | DT_ISCHOOL_BIO                  | `TRIGGER._DT_ISCHOOL_BIO`                  | ischool_doors.dat                                                                            |
| 1189 | DT_ISCHOOL_CHEM                 | `TRIGGER._DT_ISCHOOL_CHEM`                 | ischool_doors.dat                                                                            |
| 1190 | DT_Janitor_MainExit             | `TRIGGER._DT_JANITOR_MAINEXIT`             | Janitors.dat                                                                                 |
| 1191 | DT_Janitor_SchoolExit           | `TRIGGER._DT_JANITOR_SCHOOLEXIT`           | Janitors.dat                                                                                 |
| 1192 | DT_LibraryExitR                 | `TRIGGER._DT_LIBRARYEXITR`                 | isc_lib.dat                                                                                  |
| 1193 | DT_Medium_001                   | `TRIGGER._DT_MEDIUM_001`                   | tags.dat                                                                                     |
| 1194 | DT_Medium_002                   | `TRIGGER._DT_MEDIUM_002`                   | tags.dat                                                                                     |
| 1195 | DT_Medium_003                   | `TRIGGER._DT_MEDIUM_003`                   | tags.dat                                                                                     |
| 1196 | DT_Medium_004                   | `TRIGGER._DT_MEDIUM_004`                   | tags.dat                                                                                     |
| 1197 | DT_Medium_005                   | `TRIGGER._DT_MEDIUM_005`                   | tags.dat                                                                                     |
| 1198 | DT_Medium_006                   | `TRIGGER._DT_MEDIUM_006`                   | tags.dat                                                                                     |
| 1199 | DT_Medium_007                   | `TRIGGER._DT_MEDIUM_007`                   | tags.dat                                                                                     |
| 1200 | DT_Medium_008                   | `TRIGGER._DT_MEDIUM_008`                   | tags.dat                                                                                     |
| 1201 | DT_Medium_009                   | `TRIGGER._DT_MEDIUM_009`                   | tags.dat                                                                                     |
| 1202 | DT_Medium_010                   | `TRIGGER._DT_MEDIUM_010`                   | tags.dat                                                                                     |
| 1203 | DT_Medium_011                   | `TRIGGER._DT_MEDIUM_011`                   | tags.dat                                                                                     |
| 1204 | DT_Medium_012                   | `TRIGGER._DT_MEDIUM_012`                   | tags.dat                                                                                     |
| 1205 | DT_Medium_013                   | `TRIGGER._DT_MEDIUM_013`                   | tags.dat                                                                                     |
| 1206 | DT_Medium_014                   | `TRIGGER._DT_MEDIUM_014`                   | tags.dat                                                                                     |
| 1207 | DT_Medium_015                   | `TRIGGER._DT_MEDIUM_015`                   | tags.dat                                                                                     |
| 1208 | DT_Medium_016                   | `TRIGGER._DT_MEDIUM_016`                   | tags.dat                                                                                     |
| 1209 | DT_Medium_017                   | `TRIGGER._DT_MEDIUM_017`                   | tags.dat                                                                                     |
| 1210 | DT_Medium_019                   | `TRIGGER._DT_MEDIUM_019`                   | tags.dat                                                                                     |
| 1211 | DT_Medium_020                   | `TRIGGER._DT_MEDIUM_020`                   | tags.dat                                                                                     |
| 1212 | DT_Medium_021                   | `TRIGGER._DT_MEDIUM_021`                   | tags.dat                                                                                     |
| 1213 | DT_Medium_022                   | `TRIGGER._DT_MEDIUM_022`                   | tags.dat                                                                                     |
| 1214 | DT_Medium_023                   | `TRIGGER._DT_MEDIUM_023`                   | tags.dat                                                                                     |
| 1215 | DT_Medium_024                   | `TRIGGER._DT_MEDIUM_024`                   | tags.dat                                                                                     |
| 1216 | DT_Medium_025                   | `TRIGGER._DT_MEDIUM_025`                   | tags.dat                                                                                     |
| 1217 | DT_Observatory                  | `TRIGGER._DT_OBSERVATORY`                  | PAn_Main.dat                                                                                 |
| 1218 | DT_PrepToMain                   | `TRIGGER._DT_PREPTOMAIN`                   | PAn_Prep.dat                                                                                 |
| 1219 | DT_SpawnTest3                   | `TRIGGER._DT_SPAWNTEST3`                   | SpawnTest.dat                                                                                |
| 1220 | DT_TINDUST_CHEMEX_DOOR          | `TRIGGER._DT_TINDUST_CHEMEX_DOOR`          | PAn_Main.dat                                                                                 |
| 1221 | DT_Tenement_Window              | `TRIGGER._DT_TENEMENT_WINDOW`              | tenements.dat                                                                                |
| 1222 | DT_auditorium_doorL             | `TRIGGER._DT_AUDITORIUM_DOORL`             | eventsAuditorium.dat                                                                         |
| 1223 | DT_autoshop_doorL               | `TRIGGER._DT_AUTOSHOP_DOORL`               | eventsAutoShop.dat                                                                           |
| 1224 | DT_barber_exit                  | `TRIGGER._DT_BARBER_EXIT`                  | ibarber.dat                                                                                  |
| 1225 | DT_classr_doorL                 | `TRIGGER._DT_CLASSR_DOORL`                 | eventsClassroom.dat                                                                          |
| 1226 | DT_gdorm_DoorLExit              | `TRIGGER._DT_GDORM_DOORLEXIT`              | Gdorm.dat                                                                                    |
| 1227 | DT_gdorm_doorL                  | `TRIGGER._DT_GDORM_DOORL`                  | Gdorm.dat                                                                                    |
| 1228 | DT_gym_doorL                    | `TRIGGER._DT_GYM_DOORL`                    | eventsGymAndPool.dat                                                                         |
| 1229 | DT_iSafeDrop_DoorL              | `TRIGGER._DT_ISAFEDROP_DOORL`              | iSaveZones.dat                                                                               |
| 1230 | DT_iSafeGrsr_DoorL              | `TRIGGER._DT_ISAFEGRSR_DOORL`              | iSaveZones.dat                                                                               |
| 1231 | DT_iSafeJock_DoorL              | `TRIGGER._DT_ISAFEJOCK_DOORL`              | iSaveZones.dat                                                                               |
| 1232 | DT_iSafeNerd_DoorL              | `TRIGGER._DT_ISAFENERD_DOORL`              | iSaveZones.dat                                                                               |
| 1233 | DT_iSafePrep_DoorL              | `TRIGGER._DT_ISAFEPREP_DOORL`              | iSaveZones.dat                                                                               |
| 1234 | DT_ibkshop_Door                 | `TRIGGER._DT_IBKSHOP_DOOR`                 | Store.dat                                                                                    |
| 1235 | DT_iboxing_DoorL                | `TRIGGER._DT_IBOXING_DOORL`                | iboxing.dat                                                                                  |
| 1236 | DT_iclothp_doorL                | `TRIGGER._DT_ICLOTHP_DOORL`                | icloth_p.dat                                                                                 |
| 1237 | DT_iclothr_DoorL                | `TRIGGER._DT_ICLOTHR_DOORL`                | icloth_r.dat                                                                                 |
| 1238 | DT_icomshp_Basement             | `TRIGGER._DT_ICOMSHP_BASEMENT`             | Store.dat                                                                                    |
| 1239 | DT_icomshp_Door                 | `TRIGGER._DT_ICOMSHP_DOOR`                 | Store.dat                                                                                    |
| 1240 | DT_ifunhous_FMDoor              | `TRIGGER._DT_IFUNHOUS_FMDOOR`              | ifunhous.dat                                                                                 |
| 1241 | DT_ifunhous_FMDoorA             | `TRIGGER._DT_IFUNHOUS_FMDOORA`             | ifunhous.dat                                                                                 |
| 1242 | DT_igrocery_Door                | `TRIGGER._DT_IGROCERY_DOOR`                | Store.dat                                                                                    |
| 1243 | DT_indoor_TattooShop            | `TRIGGER._DT_INDOOR_TATTOOSHOP`            | tindustrial_doors.dat                                                                        |
| 1244 | DT_indoor_whouseFront           | `TRIGGER._DT_INDOOR_WHOUSEFRONT`           | tindustrial_doors.dat                                                                        |
| 1245 | DT_indoor_whouseRoof            | `TRIGGER._DT_INDOOR_WHOUSEROOF`            | tindustrial_doors.dat                                                                        |
| 1246 | DT_ischool_Art                  | `TRIGGER._DT_ISCHOOL_ART`                  | ischool_doors.dat                                                                            |
| 1247 | DT_ischool_AuditorBalc          | `TRIGGER._DT_ISCHOOL_AUDITORBALC`          | ischool_doors.dat                                                                            |
| 1248 | DT_ischool_AuditorDoorL         | `TRIGGER._DT_ISCHOOL_AUDITORDOORL`         | ischool_doors.dat                                                                            |
| 1249 | DT_ischool_BackDoorLeft         | `TRIGGER._DT_ISCHOOL_BACKDOORLEFT`         | ischool_doors.dat                                                                            |
| 1250 | DT_ischool_BackDoorRight        | `TRIGGER._DT_ISCHOOL_BACKDOORRIGHT`        | ischool_doors.dat                                                                            |
| 1251 | DT_ischool_Classroom            | `TRIGGER._DT_ISCHOOL_CLASSROOM`            | ischool_doors.dat                                                                            |
| 1252 | DT_ischool_Door01               | `TRIGGER._DT_ISCHOOL_DOOR01`               | ischool_doors.dat                                                                            |
| 1253 | DT_ischool_FrontDoorL           | `TRIGGER._DT_ISCHOOL_FRONTDOORL`           | ischool_doors.dat                                                                            |
| 1254 | DT_ischool_FrontDoorRight       | `TRIGGER._DT_ISCHOOL_FRONTDOORRIGHT`       | ischool_doors.dat                                                                            |
| 1255 | DT_ischool_HallWind             | `TRIGGER._DT_ISCHOOL_HALLWIND`             | ischool_doors.dat                                                                            |
| 1256 | DT_ischool_Janitor              | `TRIGGER._DT_ISCHOOL_JANITOR`              | ischool_doors.dat                                                                            |
| 1257 | DT_ischool_RoofDoor             | `TRIGGER._DT_ISCHOOL_ROOFDOOR`             | ischool_doors.dat                                                                            |
| 1258 | DT_ischool_Staff                | `TRIGGER._DT_ISCHOOL_STAFF`                | ischool_doors.dat                                                                            |
| 1259 | DT_observatory_doorL            | `TRIGGER._DT_OBSERVATORY_DOORL`            | eventsObservatory.dat                                                                        |
| 1260 | DT_phair_doorL                  | `TRIGGER._DT_PHAIR_DOORL`                  | eventsPoorHair.dat                                                                           |
| 1261 | DT_pool_doorL                   | `TRIGGER._DT_POOL_DOORL`                   | eventsGymAndPool.dat                                                                         |
| 1262 | DT_salon_exit                   | `TRIGGER._DT_SALON_EXIT`                   | ibarber.dat                                                                                  |
| 1263 | DT_staff_doorL                  | `TRIGGER._DT_STAFF_DOORL`                  | eventsStaffRoom.dat                                                                          |
| 1264 | DT_tBMX_enter                   | `TRIGGER._DT_TBMX_ENTER`                   | tindustrial_doors.dat                                                                        |
| 1265 | DT_tBMX_leave                   | `TRIGGER._DT_TBMX_LEAVE`                   | tBMX.dat                                                                                     |
| 1266 | DT_tbusines_BikeShopDoor        | `TRIGGER._DT_TBUSINES_BIKESHOPDOOR`        | tbusines_doors.dat                                                                           |
| 1267 | DT_tbusines_ClothDoor           | `TRIGGER._DT_TBUSINES_CLOTHDOOR`           | tbusines_doors.dat                                                                           |
| 1268 | DT_tbusines_ComicShopDoor       | `TRIGGER._DT_TBUSINES_COMICSHOPDOOR`       | tbusines_doors.dat                                                                           |
| 1269 | DT_tbusines_FirewShopDoor       | `TRIGGER._DT_TBUSINES_FIREWSHOPDOOR`       | tbusines_doors.dat                                                                           |
| 1270 | DT_tbusines_GenShop1Door        | `TRIGGER._DT_TBUSINES_GENSHOP1DOOR`        | tbusines_doors.dat                                                                           |
| 1271 | DT_tbusines_GenShop2Door        | `TRIGGER._DT_TBUSINES_GENSHOP2DOOR`        | tbusines_doors.dat                                                                           |
| 1272 | DT_tbusines_SafeNerd            | `TRIGGER._DT_TBUSINES_SAFENERD`            | tbusines_doors.dat                                                                           |
| 1273 | DT_tbusiness_FirewBusDoor       | `TRIGGER._DT_TBUSINESS_FIREWBUSDOOR`       | tbusines_doors.dat                                                                           |
| 1274 | DT_tbusiness_Recorddoor         | `TRIGGER._DT_TBUSINESS_RECORDDOOR`         | tbusines_doors.dat                                                                           |
| 1275 | DT_tbusiness_barber             | `TRIGGER._DT_TBUSINESS_BARBER`             | tbusines_doors.dat                                                                           |
| 1276 | DT_tind_SafeDrop                | `TRIGGER._DT_TIND_SAFEDROP`                | tindustrial_doors.dat                                                                        |
| 1277 | DT_tpoor_BMX                    | `TRIGGER._DT_TPOOR_BMX`                    | tbusines_doors.dat                                                                           |
| 1278 | DT_tpoor_Barber                 | `TRIGGER._DT_TPOOR_BARBER`                 | tbusines_doors.dat                                                                           |
| 1279 | DT_tpoor_SafeGreaser            | `TRIGGER._DT_TPOOR_SAFEGREASER`            | tbusines_doors.dat                                                                           |
| 1280 | DT_tpoor_tenwindow              | `TRIGGER._DT_TPOOR_TENWINDOW`              | tbusines_doors.dat                                                                           |
| 1281 | DT_trich_BarberDoor             | `TRIGGER._DT_TRICH_BARBERDOOR`             | trich_doors.dat                                                                              |
| 1282 | DT_trich_BikeShopDoor           | `TRIGGER._DT_TRICH_BIKESHOPDOOR`           | trich_doors.dat                                                                              |
| 1283 | DT_trich_BoxingDoor01           | `TRIGGER._DT_TRICH_BOXINGDOOR01`           | trich_doors.dat                                                                              |
| 1284 | DT_trich_BoxingDoor02           | `TRIGGER._DT_TRICH_BOXINGDOOR02`           | trich_doors.dat                                                                              |
| 1285 | DT_trich_ClothRichDoor          | `TRIGGER._DT_TRICH_CLOTHRICHDOOR`          | trich_doors.dat                                                                              |
| 1286 | DT_trich_FirewShopDoor          | `TRIGGER._DT_TRICH_FIREWSHOPDOOR`          | trich_doors.dat                                                                              |
| 1287 | DT_trich_GenShopDoor            | `TRIGGER._DT_TRICH_GENSHOPDOOR`            | trich_doors.dat                                                                              |
| 1288 | DT_trich_SafePrep               | `TRIGGER._DT_TRICH_SAFEPREP`               | trich_doors.dat                                                                              |
| 1289 | DT_tschool_AutoShopL            | `TRIGGER._DT_TSCHOOL_AUTOSHOPL`            | tschool_doors.dat                                                                            |
| 1290 | DT_tschool_BoysDormL            | `TRIGGER._DT_TSCHOOL_BOYSDORML`            | tschool_doors.dat                                                                            |
| 1291 | DT_tschool_ExtWind              | `TRIGGER._DT_TSCHOOL_EXTWIND`              | tschool_doors.dat                                                                            |
| 1292 | DT_tschool_GirlsDormL           | `TRIGGER._DT_TSCHOOL_GIRLSDORML`           | tschool_doors.dat                                                                            |
| 1293 | DT_tschool_GirlsDormSideL       | `TRIGGER._DT_TSCHOOL_GIRLSDORMSIDEL`       | tschool_doors.dat                                                                            |
| 1294 | DT_tschool_GymL                 | `TRIGGER._DT_TSCHOOL_GYML`                 | tschool_doors.dat                                                                            |
| 1295 | DT_tschool_LibraryL             | `TRIGGER._DT_TSCHOOL_LIBRARYL`             | tschool_doors.dat                                                                            |
| 1296 | DT_tschool_PoolL                | `TRIGGER._DT_TSCHOOL_POOLL`                | tschool_doors.dat                                                                            |
| 1297 | DT_tschool_PreppyL              | `TRIGGER._DT_TSCHOOL_PREPPYL`              | tschool_doors.dat                                                                            |
| 1298 | DT_tschool_RoofDoor             | `TRIGGER._DT_TSCHOOL_ROOFDOOR`             | tschool_doors.dat                                                                            |
| 1299 | DT_tschool_SafeJock             | `TRIGGER._DT_TSCHOOL_SAFEJOCK`             | tschool_doors.dat                                                                            |
| 1300 | DT_tschool_SchoolFrontDoorL     | `TRIGGER._DT_TSCHOOL_SCHOOLFRONTDOORL`     | tschool_doors.dat                                                                            |
| 1301 | DT_tschool_SchoolLeftBackDoor   | `TRIGGER._DT_TSCHOOL_SCHOOLLEFTBACKDOOR`   | tschool_doors.dat                                                                            |
| 1302 | DT_tschool_SchoolRightBackDoor  | `TRIGGER._DT_TSCHOOL_SCHOOLRIGHTBACKDOOR`  | tschool_doors.dat                                                                            |
| 1303 | DT_tschool_SchoolRightFrontDoor | `TRIGGER._DT_TSCHOOL_SCHOOLRIGHTFRONTDOOR` | tschool_doors.dat                                                                            |
| 1304 | DT_tschool_SchoolSideDoorL      | `TRIGGER._DT_TSCHOOL_SCHOOLSIDEDOORL`      | tschool_doors.dat                                                                            |
| 1305 | DT_whouse_front                 | `TRIGGER._DT_WHOUSE_FRONT`                 | iwarehouse.dat                                                                               |
| 1306 | DT_whouse_roof                  | `TRIGGER._DT_WHOUSE_ROOF`                  | iwarehouse.dat                                                                               |
| 1307 | DePopBeachAreaRace              | `TRIGGER._DEPOPBEACHAREARACE`              | GoKart_Outdoor.dat                                                                           |
| 1308 | DePopIndustrialAreaRace         | `TRIGGER._DEPOPINDUSTRIALAREARACE`         | GoKart_Outdoor.dat                                                                           |
| 1309 | DePopRichAreaRace               | `TRIGGER._DEPOPRICHAREARACE`               | GoKart_Outdoor.dat                                                                           |
| 1310 | Disabled_SV_AutoMain            | `TRIGGER._DISABLED_SV_AUTOMAIN`            | AreaTran.dat                                                                                 |
| 1311 | Disabled_SV_BoxingRich          | `TRIGGER._DISABLED_SV_BOXINGRICH`          | AreaTran.dat                                                                                 |
| 1312 | Disabled_SV_ClothMain           | `TRIGGER._DISABLED_SV_CLOTHMAIN`           | AreaTran.dat                                                                                 |
| 1313 | Disabled_SV_EnglishSchool       | `TRIGGER._DISABLED_SV_ENGLISHSCHOOL`       | AreaTran.dat                                                                                 |
| 1314 | Disabled_SV_GymMain             | `TRIGGER._DISABLED_SV_GYMMAIN`             | AreaTran.dat                                                                                 |
| 1315 | Disabled_SV_PrincipalSchool     | `TRIGGER._DISABLED_SV_PRINCIPALSCHOOL`     | AreaTran.dat                                                                                 |
| 1316 | Disabled_SV_Staff               | `TRIGGER._DISABLED_SV_STAFF`               | AreaTran.dat                                                                                 |
| 1317 | Door_PrepHouse_Foyer            | `TRIGGER._DOOR_PREPHOUSE_FOYER`            | PAn_Prep.dat                                                                                 |
| 1318 | Door_PrepHouse_FoyerOut         | `TRIGGER._DOOR_PREPHOUSE_FOYEROUT`         | PAn_Prep.dat                                                                                 |
| 1319 | Door_PrepHouse_Gamble           | `TRIGGER._DOOR_PREPHOUSE_GAMBLE`           | PAn_Prep.dat                                                                                 |
| 1320 | Door_PrepHouse_Lounge           | `TRIGGER._DOOR_PREPHOUSE_LOUNGE`           | PAn_Prep.dat                                                                                 |
| 1321 | Door_PrepHouse_Lounge_02        | `TRIGGER._DOOR_PREPHOUSE_LOUNGE_02`        | PAn_Prep.dat                                                                                 |
| 1322 | Door_PrepHouse_Stairs           | `TRIGGER._DOOR_PREPHOUSE_STAIRS`           | PAn_Prep.dat                                                                                 |
| 1323 | Door_PrepHouse_Stairs_Lower     | `TRIGGER._DOOR_PREPHOUSE_STAIRS_LOWER`     | PAn_Prep.dat                                                                                 |
| 1324 | Door_PrepHouse_Stairs_Upper     | `TRIGGER._DOOR_PREPHOUSE_STAIRS_UPPER`     | PAn_Prep.dat                                                                                 |
| 1325 | DormChemistrySet                | `TRIGGER._DORMCHEMISTRYSET`                | eventsBDorm.dat                                                                              |
| 1326 | DormDoorTrig1                   | `TRIGGER._DORMDOORTRIG1`                   | eventsBDorm.dat                                                                              |
| 1327 | DormDoorTrig2                   | `TRIGGER._DORMDOORTRIG2`                   | eventsBDorm.dat                                                                              |
| 1328 | DormDoorTrig3                   | `TRIGGER._DORMDOORTRIG3`                   | eventsBDorm.dat                                                                              |
| 1329 | DormDoorTrig4                   | `TRIGGER._DORMDOORTRIG4`                   | eventsBDorm.dat                                                                              |
| 1330 | DormExitDoorR                   | `TRIGGER._DORMEXITDOORR`                   | BDorm_Doors.dat                                                                              |
| 1331 | DormTVTrig                      | `TRIGGER._DORMTVTRIG`                      | eventsBDorm.dat                                                                              |
| 1332 | DownTown                        | `TRIGGER._DOWNTOWN`                        | Population.dat                                                                               |
| 1333 | DowntownGameArea                | `TRIGGER._DOWNTOWNGAMEAREA`                | GraffitiPunishment.dat                                                                       |
| 1334 | Dumpster                        | `TRIGGER._DUMPSTER`                        | ttest.dat                                                                                    |
| 1335 | DunkBackBoard                   | `TRIGGER._DUNKBACKBOARD`                   | MGDunkTank.dat                                                                               |
| 1336 | DunkBttn                        | `TRIGGER._DUNKBTTN`                        | MGDunkTank.dat                                                                               |
| 1337 | DunkSeat                        | `TRIGGER._DUNKSEAT`                        | MGDunkTank.dat                                                                               |
| 1338 | DunkTank                        | `TRIGGER._DUNKTANK`                        | MGDunkTank.dat                                                                               |
| 1339 | DunkTankExcluder                | `TRIGGER._DUNKTANKEXCLUDER`                | MGDunkTank.dat                                                                               |
| 1340 | ESCDoorL                        | `TRIGGER._ESCDOORL`                        | iSaveZones.dat, isc_lib.dat                                                                  |
| 1341 | ESCDoorL04                      | `TRIGGER._ESCDOORL04`                      | iSaveZones.dat                                                                               |
| 1342 | ESCDoorL05                      | `TRIGGER._ESCDOORL05`                      | iSaveZones.dat, trich.dat                                                                    |
| 1343 | ESCDoorL06                      | `TRIGGER._ESCDOORL06`                      | iSaveZones.dat                                                                               |
| 1344 | ESCDoorR                        | `TRIGGER._ESCDOORR`                        | iSaveZones.dat, iasylum.dat                                                                  |
| 1345 | ESCDoorR05                      | `TRIGGER._ESCDOORR05`                      | trich.dat                                                                                    |
| 1346 | EVENING_MUSIC_TRIGGER           | `TRIGGER._EVENING_MUSIC_TRIGGER`           | School_Exterior.dat                                                                          |
| 1347 | EasyDrugs_Trash01               | `TRIGGER._EASYDRUGS_TRASH01`               | EasyDrugs.dat                                                                                |
| 1348 | EasyDrugs_Trash02               | `TRIGGER._EASYDRUGS_TRASH02`               | EasyDrugs.dat                                                                                |
| 1349 | EasyDrugs_Trash03               | `TRIGGER._EASYDRUGS_TRASH03`               | EasyDrugs.dat                                                                                |
| 1350 | EasyDrugs_Trash04               | `TRIGGER._EASYDRUGS_TRASH04`               | EasyDrugs.dat                                                                                |
| 1351 | EasyDrugs_Trash05               | `TRIGGER._EASYDRUGS_TRASH05`               | EasyDrugs.dat                                                                                |
| 1352 | EasyDrugs_Trash06               | `TRIGGER._EASYDRUGS_TRASH06`               | EasyDrugs.dat                                                                                |
| 1353 | EggBDorm                        | `TRIGGER._EGGBDORM`                        | tschool_maindoors.dat                                                                        |
| 1354 | EggGDorm                        | `TRIGGER._EGGGDORM`                        | tschool_maindoors.dat                                                                        |
| 1355 | EntryToWondMeat                 | `TRIGGER._ENTRYTOWONDMEAT`                 | 6_02.dat                                                                                     |
| 1356 | EquipmentRoom                   | `TRIGGER._EQUIPMENTROOM`                   | C5.dat, PhotoZoom.dat                                                                        |
| 1357 | ExitFerrisTrigger               | `TRIGGER._EXITFERRISTRIGGER`               | CarnivalRides.dat                                                                            |
| 1358 | ExitToWondMeat                  | `TRIGGER._EXITTOWONDMEAT`                  | 6_02.dat                                                                                     |
| 1359 | FMDoor                          | `TRIGGER._FMDOOR`                          | iSaveZones.dat, iasylum.dat                                                                  |
| 1360 | FMDoor01                        | `TRIGGER._FMDOOR01`                        | iSaveZones.dat                                                                               |
| 1361 | FMDoor01N                       | `TRIGGER._FMDOOR01N`                       | Store.dat                                                                                    |
| 1362 | FMDoor02                        | `TRIGGER._FMDOOR02`                        | iasylum.dat                                                                                  |
| 1363 | FMDoor03                        | `TRIGGER._FMDOOR03`                        | iasylum.dat                                                                                  |
| 1364 | FMDoor04                        | `TRIGGER._FMDOOR04`                        | iasylum.dat                                                                                  |
| 1365 | FMDoor05                        | `TRIGGER._FMDOOR05`                        | iasylum.dat                                                                                  |
| 1366 | FMDoor06                        | `TRIGGER._FMDOOR06`                        | iasylum.dat                                                                                  |
| 1367 | FMDoor07                        | `TRIGGER._FMDOOR07`                        | iasylum.dat                                                                                  |
| 1368 | FMDoor08                        | `TRIGGER._FMDOOR08`                        | iasylum.dat                                                                                  |
| 1369 | FMDoorN                         | `TRIGGER._FMDOORN`                         | Store.dat                                                                                    |
| 1370 | FMDoorN01                       | `TRIGGER._FMDOORN01`                       | Store.dat                                                                                    |
| 1371 | FRAFFY                          | `TRIGGER._FRAFFY`                          | FraffyMachine.dat                                                                            |
| 1372 | FUNHOUSE_CURTAIN_OPEN           | `TRIGGER._FUNHOUSE_CURTAIN_OPEN`           | funhouse.dat                                                                                 |
| 1373 | FUNHOUSE_GRAVECONTROL           | `TRIGGER._FUNHOUSE_GRAVECONTROL`           | funhouse.dat                                                                                 |
| 1374 | FUNHOUSE_GRAVES                 | `TRIGGER._FUNHOUSE_GRAVES`                 | funhouse.dat                                                                                 |
| 1375 | FUNHOUSE_GRAVEYARD              | `TRIGGER._FUNHOUSE_GRAVEYARD`              | funhouse.dat                                                                                 |
| 1376 | FUNHOUSE_GRAVE_TO_MAZE_TRANS    | `TRIGGER._FUNHOUSE_GRAVE_TO_MAZE_TRANS`    | funhouse.dat                                                                                 |
| 1377 | FUNHOUSE_MAZE                   | `TRIGGER._FUNHOUSE_MAZE`                   | funhouse.dat                                                                                 |
| 1378 | FUNHOUSE_MAZE_TO_GRAVE_TRANS    | `TRIGGER._FUNHOUSE_MAZE_TO_GRAVE_TRANS`    | funhouse.dat                                                                                 |
| 1379 | FUNHOUSE_MINE                   | `TRIGGER._FUNHOUSE_MINE`                   | funhouse.dat                                                                                 |
| 1380 | FUNHOUSE_MINE_ROCKS             | `TRIGGER._FUNHOUSE_MINE_ROCKS`             | funhouse.dat                                                                                 |
| 1381 | FUNHOUSE_MINE_STEAM_01          | `TRIGGER._FUNHOUSE_MINE_STEAM_01`          | funhouse.dat                                                                                 |
| 1382 | FUNHOUSE_MINE_STEAM_02          | `TRIGGER._FUNHOUSE_MINE_STEAM_02`          | funhouse.dat                                                                                 |
| 1383 | FUNHOUSE_MINE_STEAM_03          | `TRIGGER._FUNHOUSE_MINE_STEAM_03`          | funhouse.dat                                                                                 |
| 1384 | FUNHOUSE_PILLOW_ROOM            | `TRIGGER._FUNHOUSE_PILLOW_ROOM`            | funhouse.dat                                                                                 |
| 1385 | FUNHOUSE_P_TO_G_TRANS           | `TRIGGER._FUNHOUSE_P_TO_G_TRANS`           | funhouse.dat                                                                                 |
| 1386 | FUNHOUSE_SCAFFOLD               | `TRIGGER._FUNHOUSE_SCAFFOLD`               | funhouse.dat                                                                                 |
| 1387 | FUNHOUSE_UPSIDEDOWN_ROOM        | `TRIGGER._FUNHOUSE_UPSIDEDOWN_ROOM`        | funhouse.dat                                                                                 |
| 1388 | FUNHOUSE_U_TO_G_TRANS           | `TRIGGER._FUNHOUSE_U_TO_G_TRANS`           | funhouse.dat                                                                                 |
| 1389 | FUNHOUSE_VORTEX_ENTRANCE        | `TRIGGER._FUNHOUSE_VORTEX_ENTRANCE`        | funhouse.dat                                                                                 |
| 1390 | FactoryEntrance                 | `TRIGGER._FACTORYENTRANCE`                 | 6_02.dat                                                                                     |
| 1391 | Ferris                          | `TRIGGER._FERRIS`                          | tcarni.dat                                                                                   |
| 1392 | FieldOverride                   | `TRIGGER._FIELDOVERRIDE`                   | Population.dat                                                                               |
| 1393 | FightingArea                    | `TRIGGER._FIGHTINGAREA`                    | 1_06.dat                                                                                     |
| 1394 | FinalFightTrig                  | `TRIGGER._FINALFIGHTTRIG`                  | 3_06New.dat                                                                                  |
| 1395 | FinalPosCheck                   | `TRIGGER._FINALPOSCHECK`                   | 1_06.dat                                                                                     |
| 1396 | FireworkBusiness                | `TRIGGER._FIREWORKBUSINESS`                | AreaTran.dat                                                                                 |
| 1397 | FlagLeftSchool                  | `TRIGGER._FLAGLEFTSCHOOL`                  | C5.dat, PhotoZoom.dat                                                                        |
| 1398 | FlagRightSchool                 | `TRIGGER._FLAGRIGHTSCHOOL`                 | C5.dat, PhotoZoom.dat                                                                        |
| 1399 | Flea                            | `TRIGGER._FLEA`                            | PhotoFilters.dat                                                                             |
| 1400 | FootFieldTrig                   | `TRIGGER._FOOTFIELDTRIG`                   | Football_Paths.dat                                                                           |
| 1401 | FootballField                   | `TRIGGER._FOOTBALLFIELD`                   | 4_B2.dat                                                                                     |
| 1402 | FootballFieldEntrance           | `TRIGGER._FOOTBALLFIELDENTRANCE`           | C5.dat                                                                                       |
| 1403 | Forest                          | `TRIGGER._FOREST`                          | SoundTriggers.dat                                                                            |
| 1404 | FortuneTeller                   | `TRIGGER._FORTUNETELLER`                   | trich.dat                                                                                    |
| 1405 | FountainCutscene                | `TRIGGER._FOUNTAINCUTSCENE`                | 1_08.dat                                                                                     |
| 1406 | FreakShow_AmbEnter              | `TRIGGER._FREAKSHOW_AMBENTER`              | SP_FreakShow.dat                                                                             |
| 1407 | FreakShow_AmbExit               | `TRIGGER._FREAKSHOW_AMBEXIT`               | SP_FreakShow.dat                                                                             |
| 1408 | FreakShow_Errie01               | `TRIGGER._FREAKSHOW_ERRIE01`               | SP_FreakShow.dat                                                                             |
| 1409 | FreakShow_Errie02               | `TRIGGER._FREAKSHOW_ERRIE02`               | SP_FreakShow.dat                                                                             |
| 1410 | FreakShow_MidgetFight           | `TRIGGER._FREAKSHOW_MIDGETFIGHT`           | FreakShow.dat                                                                                |
| 1411 | FreakShow_Midgets               | `TRIGGER._FREAKSHOW_MIDGETS`               | FreakShow.dat                                                                                |
| 1412 | FunTeeth                        | `TRIGGER._FUNTEETH`                        | tcarni.dat                                                                                   |
| 1413 | Funhouse_Auditorium             | `TRIGGER._FUNHOUSE_AUDITORIUM`             | SP_HouseOfMirrors.dat                                                                        |
| 1414 | Funhouse_ControlRm_Graveyard    | `TRIGGER._FUNHOUSE_CONTROLRM_GRAVEYARD`    | SP_HouseOfMirrors.dat                                                                        |
| 1415 | Funhouse_HauntedMaze            | `TRIGGER._FUNHOUSE_HAUNTEDMAZE`            | SP_HouseOfMirrors.dat                                                                        |
| 1416 | Funhouse_MineShaft              | `TRIGGER._FUNHOUSE_MINESHAFT`              | SP_HouseOfMirrors.dat                                                                        |
| 1417 | Funhouse_Sound_Graveyard        | `TRIGGER._FUNHOUSE_SOUND_GRAVEYARD`        | SP_HouseOfMirrors.dat                                                                        |
| 1418 | Funhouse_Tounge                 | `TRIGGER._FUNHOUSE_TOUNGE`                 | SP_HouseOfMirrors.dat                                                                        |
| 1419 | Funhouse_UpsideDown             | `TRIGGER._FUNHOUSE_UPSIDEDOWN`             | SP_HouseOfMirrors.dat                                                                        |
| 1420 | Funhouse_Vortex                 | `TRIGGER._FUNHOUSE_VORTEX`                 | SP_HouseOfMirrors.dat                                                                        |
| 1421 | Funhouse_Whackamole             | `TRIGGER._FUNHOUSE_WHACKAMOLE`             | SP_HouseOfMirrors.dat                                                                        |
| 1422 | GC1A_GameArea                   | `TRIGGER._GC1A_GAMEAREA`                   | GraffitiPunishment.dat                                                                       |
| 1423 | GDormBackDr                     | `TRIGGER._GDORMBACKDR`                     | C5.dat, PhotoZoom.dat                                                                        |
| 1424 | GDormEntrance                   | `TRIGGER._GDORMENTRANCE`                   | C5.dat, PhotoZoom.dat                                                                        |
| 1425 | GDormExitExclude                | `TRIGGER._GDORMEXITEXCLUDE`                | Global.dat                                                                                   |
| 1426 | GDormTarg                       | `TRIGGER._GDORMTARG`                       | PAn_Main.dat                                                                                 |
| 1427 | GDorm_GirlsOnly                 | `TRIGGER._GDORM_GIRLSONLY`                 | Gdorm.dat                                                                                    |
| 1428 | GDorm_PopOverride               | `TRIGGER._GDORM_POPOVERRIDE`               | Gdorm.dat                                                                                    |
| 1429 | GDorm_Stall01                   | `TRIGGER._GDORM_STALL01`                   | Gdorm.dat                                                                                    |
| 1430 | GDorm_Stall02                   | `TRIGGER._GDORM_STALL02`                   | Gdorm.dat                                                                                    |
| 1431 | GDorm_UpperDoor                 | `TRIGGER._GDORM_UPPERDOOR`                 | Gdorm.dat                                                                                    |
| 1432 | GDorm_UpperDoorStorage          | `TRIGGER._GDORM_UPPERDOORSTORAGE`          | Gdorm.dat                                                                                    |
| 1433 | GREASERS_JET01                  | `TRIGGER._GREASERS_JET01`                  | 3_B.dat                                                                                      |
| 1434 | GREASERS_JET02                  | `TRIGGER._GREASERS_JET02`                  | 3_B.dat                                                                                      |
| 1435 | GREASERS_JET03                  | `TRIGGER._GREASERS_JET03`                  | 3_B.dat                                                                                      |
| 1436 | GREASERS_JET04                  | `TRIGGER._GREASERS_JET04`                  | 3_B.dat                                                                                      |
| 1437 | GREASERS_JET05                  | `TRIGGER._GREASERS_JET05`                  | 3_B.dat                                                                                      |
| 1438 | GarageRoofTrig                  | `TRIGGER._GARAGEROOFTRIG`                  | 6_02.dat                                                                                     |
| 1439 | GarageTrig                      | `TRIGGER._GARAGETRIG`                      | 6_02.dat                                                                                     |
| 1440 | Garage_BusinessArea             | `TRIGGER._GARAGE_BUSINESSAREA`             | Garages.dat                                                                                  |
| 1441 | Garage_PoorArea                 | `TRIGGER._GARAGE_POORAREA`                 | Garages.dat                                                                                  |
| 1442 | Garage_RichArea                 | `TRIGGER._GARAGE_RICHAREA`                 | Garages.dat                                                                                  |
| 1443 | Garage_SchoolGrounds            | `TRIGGER._GARAGE_SCHOOLGROUNDS`            | Garages.dat                                                                                  |
| 1444 | GarbCanA                        | `TRIGGER._GARBCANA`                        | ttest.dat                                                                                    |
| 1445 | GaryTrigger                     | `TRIGGER._GARYTRIGGER`                     | 1_02.dat                                                                                     |
| 1446 | GasSign                         | `TRIGGER._GASSIGN`                         | ttest.dat                                                                                    |
| 1447 | GasStop1                        | `TRIGGER._GASSTOP1`                        | mm_retirement.dat                                                                            |
| 1448 | GasStop2                        | `TRIGGER._GASSTOP2`                        | mm_retirement.dat                                                                            |
| 1449 | GirlsBathroom1                  | `TRIGGER._GIRLSBATHROOM1`                  | eventsSchoolHalls.dat                                                                        |
| 1450 | GirlsBathroom2                  | `TRIGGER._GIRLSBATHROOM2`                  | eventsSchoolHalls.dat                                                                        |
| 1451 | GirlsDormTrig                   | `TRIGGER._GIRLSDORMTRIG`                   | 6_02.dat                                                                                     |
| 1452 | GirlsDorm_Attic                 | `TRIGGER._GIRLSDORM_ATTIC`                 | SP_Girls_Dorm.dat                                                                            |
| 1453 | GirlsTrig                       | `TRIGGER._GIRLSTRIG`                       | 6_02.dat                                                                                     |
| 1454 | GlassDome                       | `TRIGGER._GLASSDOME`                       | C5.dat, PhotoZoom.dat                                                                        |
| 1455 | GnomeB                          | `TRIGGER._GNOMEB`                          | ttest.dat                                                                                    |
| 1456 | GnomeD                          | `TRIGGER._GNOMED`                          | ttest.dat                                                                                    |
| 1457 | GoKartTrack_Amb                 | `TRIGGER._GOKARTTRACK_AMB`                 | SP_TGOKart.dat                                                                               |
| 1458 | GordYell                        | `TRIGGER._GORDYELL`                        | 3_06New.dat                                                                                  |
| 1459 | GraveYard                       | `TRIGGER._GRAVEYARD`                       | Population.dat                                                                               |
| 1460 | GreaserBathroom                 | `TRIGGER._GREASERBATHROOM`                 | SP_iGrsrS.dat                                                                                |
| 1461 | GreaserMainRoom                 | `TRIGGER._GREASERMAINROOM`                 | SP_iGrsrS.dat                                                                                |
| 1462 | GreaserTag                      | `TRIGGER._GREASERTAG`                      | GraffitiTest.dat                                                                             |
| 1463 | GreaserTagArea                  | `TRIGGER._GREASERTAGAREA`                  | GraffitiTest.dat                                                                             |
| 1464 | Greasers                        | `TRIGGER._GREASERS`                        | Population.dat                                                                               |
| 1465 | GroceryBusiness                 | `TRIGGER._GROCERYBUSINESS`                 | AreaTran.dat                                                                                 |
| 1466 | GroceryStore                    | `TRIGGER._GROCERYSTORE`                    | SP_GroceryStore.dat                                                                          |
| 1467 | GymPoolHall                     | `TRIGGER._GYMPOOLHALL`                     | SP_Pool.dat                                                                                  |
| 1468 | GymPool_PopOverride             | `TRIGGER._GYMPOOL_POPOVERRIDE`             | isc_pool.dat                                                                                 |
| 1469 | Gym_BoysChange                  | `TRIGGER._GYM_BOYSCHANGE`                  | SP_Pool.dat                                                                                  |
| 1470 | Gym_GirlsChange                 | `TRIGGER._GYM_GIRLSCHANGE`                 | SP_Pool.dat                                                                                  |
| 1471 | Gym_Main                        | `TRIGGER._GYM_MAIN`                        | SP_Pool.dat                                                                                  |
| 1472 | Gym_Pool01                      | `TRIGGER._GYM_POOL01`                      | SP_Pool.dat                                                                                  |
| 1473 | Gym_Pool02                      | `TRIGGER._GYM_POOL02`                      | SP_Pool.dat                                                                                  |
| 1474 | Gymnasium                       | `TRIGGER._GYMNASIUM`                       | C5.dat, PhotoZoom.dat                                                                        |
| 1475 | GymnasiumBack                   | `TRIGGER._GYMNASIUMBACK`                   | C5.dat, PhotoZoom.dat                                                                        |
| 1476 | HSdinger                        | `TRIGGER._HSDINGER`                        | HighStrikerProps.dat                                                                         |
| 1477 | HairPoorRm01                    | `TRIGGER._HAIRPOORRM01`                    | SP_Poor_Hair.dat                                                                             |
| 1478 | HairPoorRm02                    | `TRIGGER._HAIRPOORRM02`                    | SP_Poor_Hair.dat                                                                             |
| 1479 | HallsPopTrigger                 | `TRIGGER._HALLSPOPTRIGGER`                 | eventsSchoolHalls.dat                                                                        |
| 1480 | HarringtonTrig                  | `TRIGGER._HARRINGTONTRIG`                  | 6_02.dat                                                                                     |
| 1481 | HattrickDoor                    | `TRIGGER._HATTRICKDOOR`                    | trich_doors.dat                                                                              |
| 1482 | Hattrick_gate                   | `TRIGGER._HATTRICK_GATE`                   | trich.dat                                                                                    |
| 1483 | HighGround                      | `TRIGGER._HIGHGROUND`                      | 1_06.dat                                                                                     |
| 1484 | HighStrikerExcluder             | `TRIGGER._HIGHSTRIKEREXCLUDER`             | CarnStrik.dat                                                                                |
| 1485 | HoboTrigger                     | `TRIGGER._HOBOTRIGGER`                     | 1_06.dat                                                                                     |
| 1486 | HouseThirdFloor                 | `TRIGGER._HOUSETHIRDFLOOR`                 | PAn_Prep.dat                                                                                 |
| 1487 | IA_medium01                     | `TRIGGER._IA_MEDIUM01`                     | tags.dat                                                                                     |
| 1488 | IA_medium02                     | `TRIGGER._IA_MEDIUM02`                     | tags.dat                                                                                     |
| 1489 | IA_medium03                     | `TRIGGER._IA_MEDIUM03`                     | tags.dat                                                                                     |
| 1490 | IA_medium04                     | `TRIGGER._IA_MEDIUM04`                     | tags.dat                                                                                     |
| 1491 | IA_medium05                     | `TRIGGER._IA_MEDIUM05`                     | tags.dat                                                                                     |
| 1492 | IA_medium06                     | `TRIGGER._IA_MEDIUM06`                     | tags.dat                                                                                     |
| 1493 | IA_medium07                     | `TRIGGER._IA_MEDIUM07`                     | tags.dat                                                                                     |
| 1494 | IBOXING_SWEATER_TRIG            | `TRIGGER._IBOXING_SWEATER_TRIG`            | iboxing.dat                                                                                  |
| 1495 | INPOOLAREA                      | `TRIGGER._INPOOLAREA`                      | eventsGymAndPool.dat                                                                         |
| 1496 | Incin                           | `TRIGGER._INCIN`                           | ttest.dat                                                                                    |
| 1497 | Ind_DoorStr02                   | `TRIGGER._IND_DOORSTR02`                   | tindustrial_doors.dat                                                                        |
| 1498 | Ind_DoorStr1                    | `TRIGGER._IND_DOORSTR1`                    | tindustrial_doors.dat                                                                        |
| 1499 | Ind_MedicalDoor                 | `TRIGGER._IND_MEDICALDOOR`                 | tindustrial_doors.dat                                                                        |
| 1500 | Ind_PoliceDoor                  | `TRIGGER._IND_POLICEDOOR`                  | tindustrial_doors.dat                                                                        |
| 1501 | Ind_SpazMeats                   | `TRIGGER._IND_SPAZMEATS`                   | SoundTriggers.dat                                                                            |
| 1502 | IndustrialArea_DropOutEnclave   | `TRIGGER._INDUSTRIALAREA_DROPOUTENCLAVE`   | Population.dat                                                                               |
| 1503 | IndustrialBarricade             | `TRIGGER._INDUSTRIALBARRICADE`             | Barricade_Triggers.dat                                                                       |
| 1504 | IndustrialGates                 | `TRIGGER._INDUSTRIALGATES`                 | 6_02.dat                                                                                     |
| 1505 | IndustrialNoGoArea              | `TRIGGER._INDUSTRIALNOGOAREA`              | GoKart_Outdoor.dat                                                                           |
| 1506 | Industrial_Docks                | `TRIGGER._INDUSTRIAL_DOCKS`                | Population.dat                                                                               |
| 1507 | Industrial_Sawmill              | `TRIGGER._INDUSTRIAL_SAWMILL`              | Population.dat                                                                               |
| 1508 | InstBatter                      | `TRIGGER._INSTBATTER`                      | MGBaseballToss.dat                                                                           |
| 1509 | InstCatcher                     | `TRIGGER._INSTCATCHER`                     | MGBaseballToss.dat                                                                           |
| 1510 | InstUmpire                      | `TRIGGER._INSTUMPIRE`                      | MGBaseballToss.dat                                                                           |
| 1511 | JOHNNYONTHESPOT                 | `TRIGGER._JOHNNYONTHESPOT`                 | Global.dat                                                                                   |
| 1512 | JainitorsRoom                   | `TRIGGER._JAINITORSROOM`                   | SP_School_Hallways.dat                                                                       |
| 1513 | JanDoor02                       | `TRIGGER._JANDOOR02`                       | ischool_doors.dat                                                                            |
| 1514 | JanDoors00                      | `TRIGGER._JANDOORS00`                      | Janitors.dat                                                                                 |
| 1515 | JanDoors01                      | `TRIGGER._JANDOORS01`                      | Janitors.dat                                                                                 |
| 1516 | JanDoors02                      | `TRIGGER._JANDOORS02`                      | Janitors.dat                                                                                 |
| 1517 | JanDoors03b                     | `TRIGGER._JANDOORS03B`                     | Janitors.dat                                                                                 |
| 1518 | JanElectricProxy                | `TRIGGER._JANELECTRICPROXY`                | Janitors.dat                                                                                 |
| 1519 | JanExtraFire                    | `TRIGGER._JANEXTRAFIRE`                    | Janitors.dat                                                                                 |
| 1520 | JanFire01                       | `TRIGGER._JANFIRE01`                       | Janitors.dat                                                                                 |
| 1521 | JanFire02                       | `TRIGGER._JANFIRE02`                       | Janitors.dat                                                                                 |
| 1522 | JanSteamProxy                   | `TRIGGER._JANSTEAMPROXY`                   | Janitors.dat                                                                                 |
| 1523 | JanSwtch00                      | `TRIGGER._JANSWTCH00`                      | Janitors.dat                                                                                 |
| 1524 | JanSwtch01                      | `TRIGGER._JANSWTCH01`                      | Janitors.dat                                                                                 |
| 1525 | JanSwtch02                      | `TRIGGER._JANSWTCH02`                      | Janitors.dat                                                                                 |
| 1526 | JanSwtch03a                     | `TRIGGER._JANSWTCH03A`                     | Janitors.dat                                                                                 |
| 1527 | JockHideOut                     | `TRIGGER._JOCKHIDEOUT`                     | SP_iJockS.dat                                                                                |
| 1528 | Jocks                           | `TRIGGER._JOCKS`                           | Population.dat                                                                               |
| 1529 | Jocks_FootballField             | `TRIGGER._JOCKS_FOOTBALLFIELD`             | Population.dat                                                                               |
| 1530 | JohnnyRamble02                  | `TRIGGER._JOHNNYRAMBLE02`                  | 3_B.dat                                                                                      |
| 1531 | LM1_GameArea                    | `TRIGGER._LM1_GAMEAREA`                    | LawnMowing.dat                                                                               |
| 1532 | LM2_GameArea                    | `TRIGGER._LM2_GAMEAREA`                    | LawnMowing.dat                                                                               |
| 1533 | LM3_Depop                       | `TRIGGER._LM3_DEPOP`                       | LawnMowing.dat                                                                               |
| 1534 | LM3_GameArea                    | `TRIGGER._LM3_GAMEAREA`                    | LawnMowing.dat                                                                               |
| 1535 | LM4_GameArea                    | `TRIGGER._LM4_GAMEAREA`                    | LawnMowing.dat                                                                               |
| 1536 | LM5_GameArea                    | `TRIGGER._LM5_GAMEAREA`                    | LawnMowing.dat                                                                               |
| 1537 | LackeySetA                      | `TRIGGER._LACKEYSETA`                      | 1_08.dat                                                                                     |
| 1538 | LackeySetB                      | `TRIGGER._LACKEYSETB`                      | 1_08.dat                                                                                     |
| 1539 | LackeySetC                      | `TRIGGER._LACKEYSETC`                      | 1_08.dat                                                                                     |
| 1540 | LackeySetD                      | `TRIGGER._LACKEYSETD`                      | 1_08.dat                                                                                     |
| 1541 | LackeySetE                      | `TRIGGER._LACKEYSETE`                      | 1_08.dat                                                                                     |
| 1542 | LawnMowerTrigger                | `TRIGGER._LAWNMOWERTRIGGER`                | mm_retirement.dat                                                                            |
| 1543 | LckrGymA01                      | `TRIGGER._LCKRGYMA01`                      | isc_pool.dat                                                                                 |
| 1544 | LckrGymA02                      | `TRIGGER._LCKRGYMA02`                      | isc_pool.dat                                                                                 |
| 1545 | LckrGymA03                      | `TRIGGER._LCKRGYMA03`                      | isc_pool.dat                                                                                 |
| 1546 | LckrGymB                        | `TRIGGER._LCKRGYMB`                        | isc_pool.dat                                                                                 |
| 1547 | LckrGymB01                      | `TRIGGER._LCKRGYMB01`                      | isc_pool.dat                                                                                 |
| 1548 | LckrGymB02                      | `TRIGGER._LCKRGYMB02`                      | isc_pool.dat                                                                                 |
| 1549 | LckrGymB03                      | `TRIGGER._LCKRGYMB03`                      | isc_pool.dat                                                                                 |
| 1550 | LckrGymM                        | `TRIGGER._LCKRGYMM`                        | isc_pool.dat                                                                                 |
| 1551 | LibTarg                         | `TRIGGER._LIBTARG`                         | PAn_Main.dat                                                                                 |
| 1552 | LibTrig                         | `TRIGGER._LIBTRIG`                         | 6_02.dat                                                                                     |
| 1553 | LibraryArch                     | `TRIGGER._LIBRARYARCH`                     | C5.dat, PhotoZoom.dat                                                                        |
| 1554 | LibraryL                        | `TRIGGER._LIBRARYL`                        | C5.dat, PhotoZoom.dat                                                                        |
| 1555 | LibraryR                        | `TRIGGER._LIBRARYR`                        | C5.dat, PhotoZoom.dat                                                                        |
| 1556 | Library_Inner                   | `TRIGGER._LIBRARY_INNER`                   | SP_Library.dat                                                                               |
| 1557 | Library_Outer                   | `TRIGGER._LIBRARY_OUTER`                   | SP_Library.dat                                                                               |
| 1558 | Library_Tunnels                 | `TRIGGER._LIBRARY_TUNNELS`                 | SP_Library.dat                                                                               |
| 1559 | LifeGrd                         | `TRIGGER._LIFEGRD`                         | ttest.dat                                                                                    |
| 1560 | LockerTest                      | `TRIGGER._LOCKERTEST`                      | SpawnTest.dat                                                                                |
| 1561 | LowCorona                       | `TRIGGER._LOWCORONA`                       | 1_06.dat                                                                                     |
| 1562 | LunchLadyTrigger                | `TRIGGER._LUNCHLADYTRIGGER`                | eventsCafeteria.dat                                                                          |
| 1563 | MGL2_01_GameArea                | `TRIGGER._MGL2_01_GAMEAREA`                | MGLawnMowing2P.dat                                                                           |
| 1564 | MGL2_02_GameArea                | `TRIGGER._MGL2_02_GAMEAREA`                | MGLawnMowing2P.dat                                                                           |
| 1565 | MGL2_03_GameArea                | `TRIGGER._MGL2_03_GAMEAREA`                | MGLawnMowing2P.dat                                                                           |
| 1566 | MGL2_04_GameArea                | `TRIGGER._MGL2_04_GAMEAREA`                | MGLawnMowing2P.dat                                                                           |
| 1567 | MGL2_05_GameArea                | `TRIGGER._MGL2_05_GAMEAREA`                | MGLawnMowing2P.dat                                                                           |
| 1568 | MGS2_Bonus01                    | `TRIGGER._MGS2_BONUS01`                    | MGShooting2P.dat                                                                             |
| 1569 | MGS2_Bottle01                   | `TRIGGER._MGS2_BOTTLE01`                   | MGShooting2P.dat                                                                             |
| 1570 | MGS2_Bottle02                   | `TRIGGER._MGS2_BOTTLE02`                   | MGShooting2P.dat                                                                             |
| 1571 | MGS2_Bottle03                   | `TRIGGER._MGS2_BOTTLE03`                   | MGShooting2P.dat                                                                             |
| 1572 | MGS2_Bottle04                   | `TRIGGER._MGS2_BOTTLE04`                   | MGShooting2P.dat                                                                             |
| 1573 | MGS2_Bottle05                   | `TRIGGER._MGS2_BOTTLE05`                   | MGShooting2P.dat                                                                             |
| 1574 | MGS2_Bottle06                   | `TRIGGER._MGS2_BOTTLE06`                   | MGShooting2P.dat                                                                             |
| 1575 | MGS2_Bottle07                   | `TRIGGER._MGS2_BOTTLE07`                   | MGShooting2P.dat                                                                             |
| 1576 | MGS2_Bottle08                   | `TRIGGER._MGS2_BOTTLE08`                   | MGShooting2P.dat                                                                             |
| 1577 | MGS2_Cowboy01                   | `TRIGGER._MGS2_COWBOY01`                   | MGShooting2P.dat                                                                             |
| 1578 | MGS2_Cowboy02                   | `TRIGGER._MGS2_COWBOY02`                   | MGShooting2P.dat                                                                             |
| 1579 | MGS2_Cowboy03                   | `TRIGGER._MGS2_COWBOY03`                   | MGShooting2P.dat                                                                             |
| 1580 | MGS2_Cowboy04                   | `TRIGGER._MGS2_COWBOY04`                   | MGShooting2P.dat                                                                             |
| 1581 | MGS2_Robber01                   | `TRIGGER._MGS2_ROBBER01`                   | MGShooting2P.dat                                                                             |
| 1582 | MGS2_Robber02                   | `TRIGGER._MGS2_ROBBER02`                   | MGShooting2P.dat                                                                             |
| 1583 | MGS2_Robber03                   | `TRIGGER._MGS2_ROBBER03`                   | MGShooting2P.dat                                                                             |
| 1584 | MGS2_Robber04                   | `TRIGGER._MGS2_ROBBER04`                   | MGShooting2P.dat                                                                             |
| 1585 | MGS2_TutBottle                  | `TRIGGER._MGS2_TUTBOTTLE`                  | MGShooting2P.dat                                                                             |
| 1586 | MGS2_TutCowboy                  | `TRIGGER._MGS2_TUTCOWBOY`                  | MGShooting2P.dat                                                                             |
| 1587 | MGS2_TutRobber                  | `TRIGGER._MGS2_TUTROBBER`                  | MGShooting2P.dat                                                                             |
| 1588 | MGS_Bonus01                     | `TRIGGER._MGS_BONUS01`                     | MGShooting.dat                                                                               |
| 1589 | MGS_Bottle01                    | `TRIGGER._MGS_BOTTLE01`                    | MGShooting.dat                                                                               |
| 1590 | MGS_Bottle02                    | `TRIGGER._MGS_BOTTLE02`                    | MGShooting.dat                                                                               |
| 1591 | MGS_Bottle03                    | `TRIGGER._MGS_BOTTLE03`                    | MGShooting.dat                                                                               |
| 1592 | MGS_Bottle04                    | `TRIGGER._MGS_BOTTLE04`                    | MGShooting.dat                                                                               |
| 1593 | MGS_Bottle05                    | `TRIGGER._MGS_BOTTLE05`                    | MGShooting.dat                                                                               |
| 1594 | MGS_Bottle06                    | `TRIGGER._MGS_BOTTLE06`                    | MGShooting.dat                                                                               |
| 1595 | MGS_Bottle07                    | `TRIGGER._MGS_BOTTLE07`                    | MGShooting.dat                                                                               |
| 1596 | MGS_Bottle08                    | `TRIGGER._MGS_BOTTLE08`                    | MGShooting.dat                                                                               |
| 1597 | MGS_Cowboy01                    | `TRIGGER._MGS_COWBOY01`                    | MGShooting.dat                                                                               |
| 1598 | MGS_Cowboy02                    | `TRIGGER._MGS_COWBOY02`                    | MGShooting.dat                                                                               |
| 1599 | MGS_Cowboy03                    | `TRIGGER._MGS_COWBOY03`                    | MGShooting.dat                                                                               |
| 1600 | MGS_Cowboy04                    | `TRIGGER._MGS_COWBOY04`                    | MGShooting.dat                                                                               |
| 1601 | MGS_Robber01                    | `TRIGGER._MGS_ROBBER01`                    | MGShooting.dat                                                                               |
| 1602 | MGS_Robber02                    | `TRIGGER._MGS_ROBBER02`                    | MGShooting.dat                                                                               |
| 1603 | MGS_Robber03                    | `TRIGGER._MGS_ROBBER03`                    | MGShooting.dat                                                                               |
| 1604 | MGS_Robber04                    | `TRIGGER._MGS_ROBBER04`                    | MGShooting.dat                                                                               |
| 1605 | MGS_TutBottle                   | `TRIGGER._MGS_TUTBOTTLE`                   | MGShooting.dat                                                                               |
| 1606 | MGS_TutCowboy                   | `TRIGGER._MGS_TUTCOWBOY`                   | MGShooting.dat                                                                               |
| 1607 | MGS_TutRobber                   | `TRIGGER._MGS_TUTROBBER`                   | MGShooting.dat                                                                               |
| 1608 | MailmanTrigger                  | `TRIGGER._MAILMANTRIGGER`                  | mm_retirement.dat                                                                            |
| 1609 | MainAuto                        | `TRIGGER._MAINAUTO`                        | AreaTran.dat                                                                                 |
| 1610 | MainBoysDorm                    | `TRIGGER._MAINBOYSDORM`                    | AreaTran.dat                                                                                 |
| 1611 | MainGym                         | `TRIGGER._MAINGYM`                         | AreaTran.dat                                                                                 |
| 1612 | MainPrep                        | `TRIGGER._MAINPREP`                        | AreaTran.dat                                                                                 |
| 1613 | MainSchool                      | `TRIGGER._MAINSCHOOL`                      | AreaTran.dat                                                                                 |
| 1614 | ManicCopCar                     | `TRIGGER._MANICCOPCAR`                     | 3_06New.dat                                                                                  |
| 1615 | MeatPlant_boltcutters_FDoorC01  | `TRIGGER._MEATPLANT_BOLTCUTTERS_FDOORC01`  | PAn_Main.dat                                                                                 |
| 1616 | MeatPlant_hide_FDoorC02         | `TRIGGER._MEATPLANT_HIDE_FDOORC02`         | PAn_Main.dat                                                                                 |
| 1617 | MeatPlant_hide_FDoorC03         | `TRIGGER._MEATPLANT_HIDE_FDOORC03`         | PAn_Main.dat                                                                                 |
| 1618 | Midway_ShootGallery             | `TRIGGER._MIDWAY_SHOOTGALLERY`             | SP_Midway.dat                                                                                |
| 1619 | Mourge                          | `TRIGGER._MOURGE`                          | SP_Asylum.dat                                                                                |
| 1620 | NLock01A                        | `TRIGGER._NLOCK01A`                        | ischool_lockers.dat, ttest.dat                                                               |
| 1621 | NLock01A01                      | `TRIGGER._NLOCK01A01`                      | ischool_lockers.dat                                                                          |
| 1622 | NLock01A02                      | `TRIGGER._NLOCK01A02`                      | ischool_lockers.dat                                                                          |
| 1623 | NLock01B                        | `TRIGGER._NLOCK01B`                        | ischool_lockers.dat                                                                          |
| 1624 | NLock01B01                      | `TRIGGER._NLOCK01B01`                      | ischool_lockers.dat                                                                          |
| 1625 | NLock01B02                      | `TRIGGER._NLOCK01B02`                      | ischool_lockers.dat                                                                          |
| 1626 | NLock01B04                      | `TRIGGER._NLOCK01B04`                      | ischool_lockers.dat                                                                          |
| 1627 | NLock01B05                      | `TRIGGER._NLOCK01B05`                      | ischool_lockers.dat                                                                          |
| 1628 | NLock01B06                      | `TRIGGER._NLOCK01B06`                      | ischool_lockers.dat                                                                          |
| 1629 | NLock01B07                      | `TRIGGER._NLOCK01B07`                      | ischool_lockers.dat                                                                          |
| 1630 | NLock02A                        | `TRIGGER._NLOCK02A`                        | ischool_lockers.dat                                                                          |
| 1631 | NLock02A01                      | `TRIGGER._NLOCK02A01`                      | ischool_lockers.dat                                                                          |
| 1632 | NLock02A02                      | `TRIGGER._NLOCK02A02`                      | ischool_lockers.dat                                                                          |
| 1633 | NLock02A03                      | `TRIGGER._NLOCK02A03`                      | ischool_lockers.dat                                                                          |
| 1634 | NLock02B                        | `TRIGGER._NLOCK02B`                        | ischool_lockers.dat                                                                          |
| 1635 | NLock02B01                      | `TRIGGER._NLOCK02B01`                      | ischool_lockers.dat                                                                          |
| 1636 | NLock02B02                      | `TRIGGER._NLOCK02B02`                      | ischool_lockers.dat                                                                          |
| 1637 | NLock02B03                      | `TRIGGER._NLOCK02B03`                      | ischool_lockers.dat                                                                          |
| 1638 | NLock02B04                      | `TRIGGER._NLOCK02B04`                      | ischool_lockers.dat                                                                          |
| 1639 | NLock02B05                      | `TRIGGER._NLOCK02B05`                      | ischool_lockers.dat                                                                          |
| 1640 | NLock02B06                      | `TRIGGER._NLOCK02B06`                      | ischool_lockers.dat                                                                          |
| 1641 | NLock02B07                      | `TRIGGER._NLOCK02B07`                      | ischool_lockers.dat                                                                          |
| 1642 | NLock02B08                      | `TRIGGER._NLOCK02B08`                      | ischool_lockers.dat                                                                          |
| 1643 | NLock02B09                      | `TRIGGER._NLOCK02B09`                      | ischool_lockers.dat                                                                          |
| 1644 | NLock02B10                      | `TRIGGER._NLOCK02B10`                      | ischool_lockers.dat                                                                          |
| 1645 | NLock03B                        | `TRIGGER._NLOCK03B`                        | ttest.dat                                                                                    |
| 1646 | NerdComputerRoom                | `TRIGGER._NERDCOMPUTERROOM`                | SP_Comic_Shop_Rich.dat, SP_iNerdS.dat                                                        |
| 1647 | NerdEncounter                   | `TRIGGER._NERDENCOUNTER`                   | RobertoTest.dat                                                                              |
| 1648 | NerdMainRoom                    | `TRIGGER._NERDMAINROOM`                    | SP_Comic_Shop_Rich.dat, SP_iNerdS.dat                                                        |
| 1649 | NerdPath_AsySwtch               | `TRIGGER._NERDPATH_ASYSWTCH`               | PAn_Main.dat                                                                                 |
| 1650 | NerdPath_AsySwtch02             | `TRIGGER._NERDPATH_ASYSWTCH02`             | PAn_Main.dat                                                                                 |
| 1651 | NerdPath_BRDoor                 | `TRIGGER._NERDPATH_BRDOOR`                 | PAn_Main.dat                                                                                 |
| 1652 | NerdSmallRoom                   | `TRIGGER._NERDSMALLROOM`                   | SP_Comic_Shop_Rich.dat                                                                       |
| 1653 | NerdStairwell                   | `TRIGGER._NERDSTAIRWELL`                   | SP_Comic_Shop_Rich.dat, SP_iNerdS.dat                                                        |
| 1654 | Nerds                           | `TRIGGER._NERDS`                           | Population.dat                                                                               |
| 1655 | New_Gate                        | `TRIGGER._NEW_GATE`                        | New.dat                                                                                      |
| 1656 | NursingPond                     | `TRIGGER._NURSINGPOND`                     | NursingPond.dat                                                                              |
| 1657 | Observatory_Amb                 | `TRIGGER._OBSERVATORY_AMB`                 | SP_Observatory.dat                                                                           |
| 1658 | OutsideSchool1                  | `TRIGGER._OUTSIDESCHOOL1`                  | Population.dat                                                                               |
| 1659 | PAlleyPiss1                     | `TRIGGER._PALLEYPISS1`                     | PAn_Main.dat                                                                                 |
| 1660 | PAlleyPiss2                     | `TRIGGER._PALLEYPISS2`                     | PAn_Main.dat                                                                                 |
| 1661 | PAlleyPiss3                     | `TRIGGER._PALLEYPISS3`                     | PAn_Main.dat                                                                                 |
| 1662 | PAlleyPiss4                     | `TRIGGER._PALLEYPISS4`                     | PAn_Main.dat                                                                                 |
| 1663 | PAn_Prep_Armor01                | `TRIGGER._PAN_PREP_ARMOR01`                | PAn_Prep.dat                                                                                 |
| 1664 | PAn_Prep_Armor02                | `TRIGGER._PAN_PREP_ARMOR02`                | PAn_Prep.dat                                                                                 |
| 1665 | PAn_Prep_Armor03                | `TRIGGER._PAN_PREP_ARMOR03`                | PAn_Prep.dat                                                                                 |
| 1666 | PAn_Prep_Armor04                | `TRIGGER._PAN_PREP_ARMOR04`                | PAn_Prep.dat                                                                                 |
| 1667 | PAn_Prep_Armor05                | `TRIGGER._PAN_PREP_ARMOR05`                | PAn_Prep.dat                                                                                 |
| 1668 | PAn_Prep_Armor06                | `TRIGGER._PAN_PREP_ARMOR06`                | PAn_Prep.dat                                                                                 |
| 1669 | PAn_Prep_ESCDoorR               | `TRIGGER._PAN_PREP_ESCDOORR`               | PAn_Prep.dat                                                                                 |
| 1670 | PAn_Prep_Weed                   | `TRIGGER._PAN_PREP_WEED`                   | PAn_Prep.dat                                                                                 |
| 1671 | PAnim_FlyTrap                   | `TRIGGER._PANIM_FLYTRAP`                   | PAn_Prep.dat                                                                                 |
| 1672 | PETEYPIER                       | `TRIGGER._PETEYPIER`                       | trich.dat                                                                                    |
| 1673 | PLAYER_ROOM                     | `TRIGGER._PLAYER_ROOM`                     | BoysDorm.dat                                                                                 |
| 1674 | POORAREA_SODA_01                | `TRIGGER._POORAREA_SODA_01`                | SndBnkLoad.dat                                                                               |
| 1675 | POOR_TENEMENTS                  | `TRIGGER._POOR_TENEMENTS`                  | Population.dat                                                                               |
| 1676 | PO_House                        | `TRIGGER._PO_HOUSE`                        | Global.dat                                                                                   |
| 1677 | POfficeExclude                  | `TRIGGER._POFFICEEXCLUDE`                  | PriOffice.dat                                                                                |
| 1678 | PREPHOUSE_PLANTAREA             | `TRIGGER._PREPHOUSE_PLANTAREA`             | SP_Prep_House.dat                                                                            |
| 1679 | PR_CarStart01                   | `TRIGGER._PR_CARSTART01`                   | PaperRoute.dat                                                                               |
| 1680 | PR_CarStart02                   | `TRIGGER._PR_CARSTART02`                   | PaperRoute.dat                                                                               |
| 1681 | PR_CarStart03                   | `TRIGGER._PR_CARSTART03`                   | PaperRoute.dat                                                                               |
| 1682 | PR_CarStart04                   | `TRIGGER._PR_CARSTART04`                   | PaperRoute.dat                                                                               |
| 1683 | PR_CarStart05                   | `TRIGGER._PR_CARSTART05`                   | PaperRoute.dat                                                                               |
| 1684 | PR_CheckEquip                   | `TRIGGER._PR_CHECKEQUIP`                   | PaperRoute.dat                                                                               |
| 1685 | PR_DogStart00                   | `TRIGGER._PR_DOGSTART00`                   | PaperRoute.dat                                                                               |
| 1686 | PR_DogStart01                   | `TRIGGER._PR_DOGSTART01`                   | PaperRoute.dat                                                                               |
| 1687 | PR_DogStart02                   | `TRIGGER._PR_DOGSTART02`                   | PaperRoute.dat                                                                               |
| 1688 | PR_DogStart03                   | `TRIGGER._PR_DOGSTART03`                   | PaperRoute.dat                                                                               |
| 1689 | PR_DogStart04                   | `TRIGGER._PR_DOGSTART04`                   | PaperRoute.dat                                                                               |
| 1690 | PR_HattrickYard                 | `TRIGGER._PR_HATTRICKYARD`                 | PaperRoute.dat                                                                               |
| 1691 | PR_HillTop                      | `TRIGGER._PR_HILLTOP`                      | PaperRoute.dat                                                                               |
| 1692 | PR_JoggerTrigger                | `TRIGGER._PR_JOGGERTRIGGER`                | PaperRoute.dat                                                                               |
| 1693 | PR_MailManStart01               | `TRIGGER._PR_MAILMANSTART01`               | PaperRoute.dat                                                                               |
| 1694 | PR_MailManStart02               | `TRIGGER._PR_MAILMANSTART02`               | PaperRoute.dat                                                                               |
| 1695 | PR_MailManStart03               | `TRIGGER._PR_MAILMANSTART03`               | PaperRoute.dat                                                                               |
| 1696 | PR_OldLadyNorthStart            | `TRIGGER._PR_OLDLADYNORTHSTART`            | PaperRoute.dat                                                                               |
| 1697 | PR_OldLadySouthStart            | `TRIGGER._PR_OLDLADYSOUTHSTART`            | PaperRoute.dat                                                                               |
| 1698 | PR_PaperPickupTrigger           | `TRIGGER._PR_PAPERPICKUPTRIGGER`           | PaperRoute.dat                                                                               |
| 1699 | PSecretary                      | `TRIGGER._PSECRETARY`                      | PriOffice.dat                                                                                |
| 1700 | PTrig                           | `TRIGGER._PTRIG`                           | SecTrig.dat                                                                                  |
| 1701 | PUN_BDORM                       | `TRIGGER._PUN_BDORM`                       | Global.dat                                                                                   |
| 1702 | PUN_GDORM                       | `TRIGGER._PUN_GDORM`                       | Global.dat                                                                                   |
| 1703 | PaperRoute_Excluder             | `TRIGGER._PAPERROUTE_EXCLUDER`             | PaperRoute.dat                                                                               |
| 1704 | ParkingArchway                  | `TRIGGER._PARKINGARCHWAY`                  | C5.dat, PhotoZoom.dat                                                                        |
| 1705 | Picnic                          | `TRIGGER._PICNIC`                          | ttest.dat                                                                                    |
| 1706 | PokerTbl                        | `TRIGGER._POKERTBL`                        | ttest.dat                                                                                    |
| 1707 | PoorArea                        | `TRIGGER._POORAREA`                        | Population.dat                                                                               |
| 1708 | PoorArea_Medium_001             | `TRIGGER._POORAREA_MEDIUM_001`             | tags.dat                                                                                     |
| 1709 | PoorArea_Medium_002             | `TRIGGER._POORAREA_MEDIUM_002`             | tags.dat                                                                                     |
| 1710 | PoorArea_Medium_004             | `TRIGGER._POORAREA_MEDIUM_004`             | tags.dat                                                                                     |
| 1711 | PoorArea_Medium_005             | `TRIGGER._POORAREA_MEDIUM_005`             | tags.dat                                                                                     |
| 1712 | PoorArea_Medium_006             | `TRIGGER._POORAREA_MEDIUM_006`             | tags.dat                                                                                     |
| 1713 | PoorArea_Medium_007             | `TRIGGER._POORAREA_MEDIUM_007`             | tags.dat                                                                                     |
| 1714 | PoorArea_Medium_008             | `TRIGGER._POORAREA_MEDIUM_008`             | tags.dat                                                                                     |
| 1715 | PoorArea_Medium_009             | `TRIGGER._POORAREA_MEDIUM_009`             | tags.dat                                                                                     |
| 1716 | PoorArea_Medium_010             | `TRIGGER._POORAREA_MEDIUM_010`             | tags.dat                                                                                     |
| 1717 | PoorArea_Medium_013             | `TRIGGER._POORAREA_MEDIUM_013`             | tags.dat                                                                                     |
| 1718 | PoorArea_Medium_014             | `TRIGGER._POORAREA_MEDIUM_014`             | tags.dat                                                                                     |
| 1719 | PoorArea_Medium_015             | `TRIGGER._POORAREA_MEDIUM_015`             | tags.dat                                                                                     |
| 1720 | PoorArea_Medium_016             | `TRIGGER._POORAREA_MEDIUM_016`             | tags.dat                                                                                     |
| 1721 | PoorArea_Medium_017             | `TRIGGER._POORAREA_MEDIUM_017`             | tags.dat                                                                                     |
| 1722 | PoorArea_Medium_018             | `TRIGGER._POORAREA_MEDIUM_018`             | tags.dat                                                                                     |
| 1723 | PoorArea_Medium_019             | `TRIGGER._POORAREA_MEDIUM_019`             | tags.dat                                                                                     |
| 1724 | PoorArea_Medium_020             | `TRIGGER._POORAREA_MEDIUM_020`             | tags.dat                                                                                     |
| 1725 | PoorArea_Medium_021             | `TRIGGER._POORAREA_MEDIUM_021`             | tags.dat                                                                                     |
| 1726 | PoorArea_Medium_022             | `TRIGGER._POORAREA_MEDIUM_022`             | tags.dat                                                                                     |
| 1727 | PoorArea_Medium_023             | `TRIGGER._POORAREA_MEDIUM_023`             | tags.dat                                                                                     |
| 1728 | PoorArea_Medium_024             | `TRIGGER._POORAREA_MEDIUM_024`             | tags.dat                                                                                     |
| 1729 | PoorArea_Medium_025             | `TRIGGER._POORAREA_MEDIUM_025`             | tags.dat                                                                                     |
| 1730 | PoorArea_Medium_026             | `TRIGGER._POORAREA_MEDIUM_026`             | tags.dat                                                                                     |
| 1731 | PoorArea_Medium_027             | `TRIGGER._POORAREA_MEDIUM_027`             | tags.dat                                                                                     |
| 1732 | PoorArea_Medium_028             | `TRIGGER._POORAREA_MEDIUM_028`             | tags.dat                                                                                     |
| 1733 | PoorArea_Medium_029             | `TRIGGER._POORAREA_MEDIUM_029`             | tags.dat                                                                                     |
| 1734 | PoorArea_Medium_030             | `TRIGGER._POORAREA_MEDIUM_030`             | tags.dat                                                                                     |
| 1735 | PoorBarricade                   | `TRIGGER._POORBARRICADE`                   | Barricade_Triggers.dat                                                                       |
| 1736 | PoorClothing_Change             | `TRIGGER._POORCLOTHING_CHANGE`             | SP_Poor_Cloth.dat                                                                            |
| 1737 | PoorClothing_Main               | `TRIGGER._POORCLOTHING_MAIN`               | SP_Poor_Cloth.dat                                                                            |
| 1738 | PoorDepop                       | `TRIGGER._POORDEPOP`                       | GraffitiPunishment.dat                                                                       |
| 1739 | PoorGameArea                    | `TRIGGER._POORGAMEAREA`                    | GraffitiPunishment.dat                                                                       |
| 1740 | PoorTarg1                       | `TRIGGER._POORTARG1`                       | PAn_Main.dat                                                                                 |
| 1741 | PoorTarg2                       | `TRIGGER._POORTARG2`                       | PAn_Main.dat                                                                                 |
| 1742 | PoorTrainTunnel                 | `TRIGGER._POORTRAINTUNNEL`                 | SoundTriggers.dat                                                                            |
| 1743 | Poor_DropTurf1                  | `TRIGGER._POOR_DROPTURF1`                  | Population.dat                                                                               |
| 1744 | PopRoads1                       | `TRIGGER._POPROADS1`                       | Population.dat                                                                               |
| 1745 | PortaPoo                        | `TRIGGER._PORTAPOO`                        | ttest.dat                                                                                    |
| 1746 | PowerStationTrig                | `TRIGGER._POWERSTATIONTRIG`                | 6_02.dat                                                                                     |
| 1747 | Powerplant_Sequrity             | `TRIGGER._POWERPLANT_SEQURITY`             | SoundTriggers.dat                                                                            |
| 1748 | Pr_HilltopExcluder              | `TRIGGER._PR_HILLTOPEXCLUDER`              | PaperRoute.dat                                                                               |
| 1749 | PrepHouse_Atrium                | `TRIGGER._PREPHOUSE_ATRIUM`                | SP_Prep_House.dat                                                                            |
| 1750 | PrepHouse_Entrance              | `TRIGGER._PREPHOUSE_ENTRANCE`              | SP_Prep_House.dat                                                                            |
| 1751 | PrepHouse_Main2nd               | `TRIGGER._PREPHOUSE_MAIN2ND`               | SP_Prep_House.dat                                                                            |
| 1752 | PrepHouse_MainRoom              | `TRIGGER._PREPHOUSE_MAINROOM`              | SP_Prep_House.dat                                                                            |
| 1753 | PrephouseExterior               | `TRIGGER._PREPHOUSEEXTERIOR`               | SP_Prep_House.dat                                                                            |
| 1754 | PreppyL                         | `TRIGGER._PREPPYL`                         | C5.dat, PhotoZoom.dat                                                                        |
| 1755 | PreppyR                         | `TRIGGER._PREPPYR`                         | C5.dat, PhotoZoom.dat                                                                        |
| 1756 | Preps                           | `TRIGGER._PREPS`                           | Population.dat                                                                               |
| 1757 | Principle01                     | `TRIGGER._PRINCIPLE01`                     | SP_Principal.dat                                                                             |
| 1758 | Principle02                     | `TRIGGER._PRINCIPLE02`                     | SP_Principal.dat                                                                             |
| 1759 | Principle03                     | `TRIGGER._PRINCIPLE03`                     | SP_Principal.dat                                                                             |
| 1760 | Principle04                     | `TRIGGER._PRINCIPLE04`                     | SP_Principal.dat                                                                             |
| 1761 | Principle_AMB                   | `TRIGGER._PRINCIPLE_AMB`                   | SP_Principal.dat, SP_School_Hallways.dat                                                     |
| 1762 | RAIL_GDORM01                    | `TRIGGER._RAIL_GDORM01`                    | Gdorm.dat                                                                                    |
| 1763 | RAIL_GDORM02                    | `TRIGGER._RAIL_GDORM02`                    | Gdorm.dat                                                                                    |
| 1764 | RAIL_HALLWAY01                  | `TRIGGER._RAIL_HALLWAY01`                  | ischool_doors.dat                                                                            |
| 1765 | RAIL_HALLWAY02                  | `TRIGGER._RAIL_HALLWAY02`                  | ischool_doors.dat                                                                            |
| 1766 | RAIL_HALLWAY03                  | `TRIGGER._RAIL_HALLWAY03`                  | ischool_doors.dat                                                                            |
| 1767 | RAIL_HALLWAY04                  | `TRIGGER._RAIL_HALLWAY04`                  | ischool_doors.dat                                                                            |
| 1768 | RAIL_HHOUSE01                   | `TRIGGER._RAIL_HHOUSE01`                   | Global.dat                                                                                   |
| 1769 | RAIL_RICH01                     | `TRIGGER._RAIL_RICH01`                     | trich.dat                                                                                    |
| 1770 | RAIL_RICH02                     | `TRIGGER._RAIL_RICH02`                     | trich.dat                                                                                    |
| 1771 | RAIL_RICH03                     | `TRIGGER._RAIL_RICH03`                     | trich.dat                                                                                    |
| 1772 | RAIL_RICH04                     | `TRIGGER._RAIL_RICH04`                     | trich.dat                                                                                    |
| 1773 | RAIL_RICH05                     | `TRIGGER._RAIL_RICH05`                     | trich.dat                                                                                    |
| 1774 | RAIL_RICH06                     | `TRIGGER._RAIL_RICH06`                     | trich.dat                                                                                    |
| 1775 | RAIL_SCHOOL01                   | `TRIGGER._RAIL_SCHOOL01`                   | tschool_maindoors.dat                                                                        |
| 1776 | RAIL_SCHOOL02                   | `TRIGGER._RAIL_SCHOOL02`                   | tschool_maindoors.dat                                                                        |
| 1777 | RA_DoorStr02                    | `TRIGGER._RA_DOORSTR02`                    | trich_doors.dat                                                                              |
| 1778 | RA_DoorStr05                    | `TRIGGER._RA_DOORSTR05`                    | trich_doors.dat                                                                              |
| 1779 | RA_DoorStr06                    | `TRIGGER._RA_DOORSTR06`                    | trich_doors.dat                                                                              |
| 1780 | RA_DoorStr07                    | `TRIGGER._RA_DOORSTR07`                    | trich_doors.dat                                                                              |
| 1781 | RA_DoorStr08                    | `TRIGGER._RA_DOORSTR08`                    | trich_doors.dat                                                                              |
| 1782 | RA_DoorStr09                    | `TRIGGER._RA_DOORSTR09`                    | trich_doors.dat                                                                              |
| 1783 | RA_Medium01                     | `TRIGGER._RA_MEDIUM01`                     | tags.dat                                                                                     |
| 1784 | RA_Medium02                     | `TRIGGER._RA_MEDIUM02`                     | tags.dat                                                                                     |
| 1785 | RA_Medium03                     | `TRIGGER._RA_MEDIUM03`                     | tags.dat                                                                                     |
| 1786 | RA_Medium04                     | `TRIGGER._RA_MEDIUM04`                     | tags.dat                                                                                     |
| 1787 | RA_Medium05                     | `TRIGGER._RA_MEDIUM05`                     | tags.dat                                                                                     |
| 1788 | RA_Medium06                     | `TRIGGER._RA_MEDIUM06`                     | tags.dat                                                                                     |
| 1789 | RA_Medium07                     | `TRIGGER._RA_MEDIUM07`                     | tags.dat                                                                                     |
| 1790 | RA_Medium08                     | `TRIGGER._RA_MEDIUM08`                     | tags.dat                                                                                     |
| 1791 | RA_Medium10                     | `TRIGGER._RA_MEDIUM10`                     | tags.dat                                                                                     |
| 1792 | RA_Medium11                     | `TRIGGER._RA_MEDIUM11`                     | tags.dat                                                                                     |
| 1793 | RA_Medium12                     | `TRIGGER._RA_MEDIUM12`                     | tags.dat                                                                                     |
| 1794 | RA_Medium13                     | `TRIGGER._RA_MEDIUM13`                     | tags.dat                                                                                     |
| 1795 | RA_Medium14                     | `TRIGGER._RA_MEDIUM14`                     | tags.dat                                                                                     |
| 1796 | RA_Medium15                     | `TRIGGER._RA_MEDIUM15`                     | tags.dat                                                                                     |
| 1797 | RA_Medium16                     | `TRIGGER._RA_MEDIUM16`                     | tags.dat                                                                                     |
| 1798 | RA_Medium17                     | `TRIGGER._RA_MEDIUM17`                     | tags.dat                                                                                     |
| 1799 | RA_Medium18                     | `TRIGGER._RA_MEDIUM18`                     | tags.dat                                                                                     |
| 1800 | RA_Medium19                     | `TRIGGER._RA_MEDIUM19`                     | tags.dat                                                                                     |
| 1801 | RA_Medium20                     | `TRIGGER._RA_MEDIUM20`                     | tags.dat                                                                                     |
| 1802 | RA_Medium21                     | `TRIGGER._RA_MEDIUM21`                     | tags.dat                                                                                     |
| 1803 | RA_Medium22                     | `TRIGGER._RA_MEDIUM22`                     | tags.dat                                                                                     |
| 1804 | RA_Medium23                     | `TRIGGER._RA_MEDIUM23`                     | tags.dat                                                                                     |
| 1805 | RA_Medium24                     | `TRIGGER._RA_MEDIUM24`                     | tags.dat                                                                                     |
| 1806 | RA_PrepDoor02                   | `TRIGGER._RA_PREPDOOR02`                   | trich_doors.dat                                                                              |
| 1807 | RA_PrepDoor03                   | `TRIGGER._RA_PREPDOOR03`                   | trich_doors.dat                                                                              |
| 1808 | RA_PrepDoor04                   | `TRIGGER._RA_PREPDOOR04`                   | trich_doors.dat                                                                              |
| 1809 | RA_PrepDoor05                   | `TRIGGER._RA_PREPDOOR05`                   | trich_doors.dat                                                                              |
| 1810 | RA_PrepDoor06                   | `TRIGGER._RA_PREPDOOR06`                   | trich_doors.dat                                                                              |
| 1811 | RA_PrepDoor07                   | `TRIGGER._RA_PREPDOOR07`                   | trich_doors.dat                                                                              |
| 1812 | RA_PrepDoor08                   | `TRIGGER._RA_PREPDOOR08`                   | trich_doors.dat                                                                              |
| 1813 | RA_PrepDoor09                   | `TRIGGER._RA_PREPDOOR09`                   | trich_doors.dat                                                                              |
| 1814 | RA_PrepDoor10                   | `TRIGGER._RA_PREPDOOR10`                   | trich_doors.dat                                                                              |
| 1815 | RA_PrepDoor11                   | `TRIGGER._RA_PREPDOOR11`                   | trich_doors.dat                                                                              |
| 1816 | RA_PrepDoor12                   | `TRIGGER._RA_PREPDOOR12`                   | trich_doors.dat                                                                              |
| 1817 | RA_PrepDoor13                   | `TRIGGER._RA_PREPDOOR13`                   | trich_doors.dat                                                                              |
| 1818 | RA_PrepDoor14                   | `TRIGGER._RA_PREPDOOR14`                   | trich_doors.dat                                                                              |
| 1819 | RA_PrepDoor15                   | `TRIGGER._RA_PREPDOOR15`                   | trich_doors.dat                                                                              |
| 1820 | RA_medium09                     | `TRIGGER._RA_MEDIUM09`                     | tags.dat                                                                                     |
| 1821 | RCLTH_Trigger                   | `TRIGGER._RCLTH_TRIGGER`                   | icloth_r.dat                                                                                 |
| 1822 | RG_FW_enter_m                   | `TRIGGER._RG_FW_ENTER_M`                   | trich_doors.dat                                                                              |
| 1823 | RG_FW_enter_s                   | `TRIGGER._RG_FW_ENTER_S`                   | trich_doors.dat                                                                              |
| 1824 | RG_FW_exit_m                    | `TRIGGER._RG_FW_EXIT_M`                    | trich_doors.dat                                                                              |
| 1825 | RG_FW_exit_s                    | `TRIGGER._RG_FW_EXIT_S`                    | trich_doors.dat                                                                              |
| 1826 | RG_RC_enter_m                   | `TRIGGER._RG_RC_ENTER_M`                   | trich_doors.dat                                                                              |
| 1827 | RG_RC_enter_s                   | `TRIGGER._RG_RC_ENTER_S`                   | trich_doors.dat                                                                              |
| 1828 | RG_RC_exit_m                    | `TRIGGER._RG_RC_EXIT_M`                    | trich_doors.dat                                                                              |
| 1829 | RG_RC_exit_s                    | `TRIGGER._RG_RC_EXIT_S`                    | trich_doors.dat                                                                              |
| 1830 | RG_SQ_enter_m                   | `TRIGGER._RG_SQ_ENTER_M`                   | trich_doors.dat                                                                              |
| 1831 | RG_SQ_exit_m                    | `TRIGGER._RG_SQ_EXIT_M`                    | trich_doors.dat                                                                              |
| 1832 | RICH_SODA_01                    | `TRIGGER._RICH_SODA_01`                    | SndBnkLoad.dat                                                                               |
| 1833 | RMailbox                        | `TRIGGER._RMAILBOX`                        | ttest.dat                                                                                    |
| 1834 | RT_Tether                       | `TRIGGER._RT_TETHER`                       | Population.dat                                                                               |
| 1835 | Race3BrakeTutorial              | `TRIGGER._RACE3BRAKETUTORIAL`              | GoKart.dat                                                                                   |
| 1836 | RetirementTrigger               | `TRIGGER._RETIREMENTTRIGGER`               | Population.dat                                                                               |
| 1837 | RichArea                        | `TRIGGER._RICHAREA`                        | Population.dat                                                                               |
| 1838 | RichArea_DownTown               | `TRIGGER._RICHAREA_DOWNTOWN`               | Population.dat                                                                               |
| 1839 | RichBoxing                      | `TRIGGER._RICHBOXING`                      | AreaTran.dat                                                                                 |
| 1840 | RichClothing_Change             | `TRIGGER._RICHCLOTHING_CHANGE`             | SP_Rich_Cloth.dat                                                                            |
| 1841 | RichClothing_Main               | `TRIGGER._RICHCLOTHING_MAIN`               | SP_Rich_Cloth.dat                                                                            |
| 1842 | RichFolkTrigger                 | `TRIGGER._RICHFOLKTRIGGER`                 | mm_retirement.dat                                                                            |
| 1843 | RichNoGoArea                    | `TRIGGER._RICHNOGOAREA`                    | GoKart_Outdoor.dat                                                                           |
| 1844 | Rich_Area_Corner_Courtyard      | `TRIGGER._RICH_AREA_CORNER_COURTYARD`      | Population.dat                                                                               |
| 1845 | Rich_GreaserAlley               | `TRIGGER._RICH_GREASERALLEY`               | Population.dat                                                                               |
| 1846 | Rich_GreaserAlley2              | `TRIGGER._RICH_GREASERALLEY2`              | Population.dat                                                                               |
| 1847 | Rich_MailBox01                  | `TRIGGER._RICH_MAILBOX01`                  | Mailboxes_Rich.dat                                                                           |
| 1848 | Rich_MailBox23                  | `TRIGGER._RICH_MAILBOX23`                  | Mailboxes_Rich.dat                                                                           |
| 1849 | Rich_MailBox24                  | `TRIGGER._RICH_MAILBOX24`                  | Mailboxes_Rich.dat                                                                           |
| 1850 | Rich_MailBox25                  | `TRIGGER._RICH_MAILBOX25`                  | Mailboxes_Rich.dat                                                                           |
| 1851 | Rich_Mailbox02                  | `TRIGGER._RICH_MAILBOX02`                  | Mailboxes_Rich.dat                                                                           |
| 1852 | Rich_Mailbox03                  | `TRIGGER._RICH_MAILBOX03`                  | Mailboxes_Rich.dat                                                                           |
| 1853 | Rich_Mailbox04                  | `TRIGGER._RICH_MAILBOX04`                  | Mailboxes_Rich.dat                                                                           |
| 1854 | Rich_Mailbox05                  | `TRIGGER._RICH_MAILBOX05`                  | Mailboxes_Rich.dat                                                                           |
| 1855 | Rich_Mailbox06                  | `TRIGGER._RICH_MAILBOX06`                  | Mailboxes_Rich.dat                                                                           |
| 1856 | Rich_Mailbox07                  | `TRIGGER._RICH_MAILBOX07`                  | Mailboxes_Rich.dat                                                                           |
| 1857 | Rich_Mailbox08                  | `TRIGGER._RICH_MAILBOX08`                  | Mailboxes_Rich.dat                                                                           |
| 1858 | Rich_Mailbox09                  | `TRIGGER._RICH_MAILBOX09`                  | Mailboxes_Rich.dat                                                                           |
| 1859 | Rich_Mailbox10                  | `TRIGGER._RICH_MAILBOX10`                  | Mailboxes_Rich.dat                                                                           |
| 1860 | Rich_Mailbox11                  | `TRIGGER._RICH_MAILBOX11`                  | Mailboxes_Rich.dat                                                                           |
| 1861 | Rich_Mailbox12                  | `TRIGGER._RICH_MAILBOX12`                  | Mailboxes_Rich.dat                                                                           |
| 1862 | Rich_Mailbox13                  | `TRIGGER._RICH_MAILBOX13`                  | Mailboxes_Rich.dat                                                                           |
| 1863 | Rich_Mailbox14                  | `TRIGGER._RICH_MAILBOX14`                  | Mailboxes_Rich.dat                                                                           |
| 1864 | Rich_Mailbox15                  | `TRIGGER._RICH_MAILBOX15`                  | Mailboxes_Rich.dat                                                                           |
| 1865 | Rich_Mailbox16                  | `TRIGGER._RICH_MAILBOX16`                  | Mailboxes_Rich.dat                                                                           |
| 1866 | Rich_Mailbox17                  | `TRIGGER._RICH_MAILBOX17`                  | Mailboxes_Rich.dat                                                                           |
| 1867 | Rich_Mailbox18                  | `TRIGGER._RICH_MAILBOX18`                  | Mailboxes_Rich.dat                                                                           |
| 1868 | Rich_Mailbox19                  | `TRIGGER._RICH_MAILBOX19`                  | Mailboxes_Rich.dat                                                                           |
| 1869 | Rich_Mailbox20                  | `TRIGGER._RICH_MAILBOX20`                  | Mailboxes_Rich.dat                                                                           |
| 1870 | Rich_Mailbox21                  | `TRIGGER._RICH_MAILBOX21`                  | Mailboxes_Rich.dat                                                                           |
| 1871 | Rich_Mailbox22                  | `TRIGGER._RICH_MAILBOX22`                  | Mailboxes_Rich.dat                                                                           |
| 1872 | Rich_target1                    | `TRIGGER._RICH_TARGET1`                    | PAn_Rich.dat                                                                                 |
| 1873 | Rich_target2                    | `TRIGGER._RICH_TARGET2`                    | PAn_Rich.dat                                                                                 |
| 1874 | Rich_target3                    | `TRIGGER._RICH_TARGET3`                    | PAn_Rich.dat                                                                                 |
| 1875 | RingArea                        | `TRIGGER._RINGAREA`                        | 1_06.dat                                                                                     |
| 1876 | RunningThiefTrigger             | `TRIGGER._RUNNINGTHIEFTRIGGER`             | 1_08.dat                                                                                     |
| 1877 | SAVEBOOKSCHOOL                  | `TRIGGER._SAVEBOOKSCHOOL`                  | eventsSchoolHalls.dat                                                                        |
| 1878 | SCFount                         | `TRIGGER._SCFOUNT`                         | ttest.dat                                                                                    |
| 1879 | SCHOOLPROP_SODA_01              | `TRIGGER._SCHOOLPROP_SODA_01`              | SndBnkLoad.dat                                                                               |
| 1880 | SCHOOLPROP_SODA_02              | `TRIGGER._SCHOOLPROP_SODA_02`              | SndBnkLoad.dat                                                                               |
| 1881 | SCLock01                        | `TRIGGER._SCLOCK01`                        | ttest.dat                                                                                    |
| 1882 | SCLock02                        | `TRIGGER._SCLOCK02`                        | ttest.dat                                                                                    |
| 1883 | SCLock03                        | `TRIGGER._SCLOCK03`                        | ttest.dat                                                                                    |
| 1884 | SC_Crest                        | `TRIGGER._SC_CREST`                        | ttest.dat                                                                                    |
| 1885 | SCgrdoor                        | `TRIGGER._SCGRDOOR`                        | tschool_garagedoors.dat                                                                      |
| 1886 | SCgrdoor01                      | `TRIGGER._SCGRDOOR01`                      | tschool_garagedoors.dat                                                                      |
| 1887 | SCgrdoor02                      | `TRIGGER._SCGRDOOR02`                      | tschool_garagedoors.dat                                                                      |
| 1888 | SGTargBTrig                     | `TRIGGER._SGTARGBTRIG`                     | ttest.dat                                                                                    |
| 1889 | SG_Medium01                     | `TRIGGER._SG_MEDIUM01`                     | tags.dat                                                                                     |
| 1890 | SG_Medium02                     | `TRIGGER._SG_MEDIUM02`                     | tags.dat                                                                                     |
| 1891 | SG_Medium03                     | `TRIGGER._SG_MEDIUM03`                     | tags.dat                                                                                     |
| 1892 | SG_Medium04                     | `TRIGGER._SG_MEDIUM04`                     | tags.dat                                                                                     |
| 1893 | SG_Medium05                     | `TRIGGER._SG_MEDIUM05`                     | tags.dat                                                                                     |
| 1894 | SG_Medium06                     | `TRIGGER._SG_MEDIUM06`                     | tags.dat                                                                                     |
| 1895 | SG_Medium07                     | `TRIGGER._SG_MEDIUM07`                     | tags.dat                                                                                     |
| 1896 | SG_Medium08                     | `TRIGGER._SG_MEDIUM08`                     | tags.dat                                                                                     |
| 1897 | SG_Medium09                     | `TRIGGER._SG_MEDIUM09`                     | tags.dat                                                                                     |
| 1898 | SG_Medium10                     | `TRIGGER._SG_MEDIUM10`                     | tags.dat                                                                                     |
| 1899 | SG_Medium11                     | `TRIGGER._SG_MEDIUM11`                     | tags.dat                                                                                     |
| 1900 | SG_Medium12                     | `TRIGGER._SG_MEDIUM12`                     | tags.dat                                                                                     |
| 1901 | SG_Medium14                     | `TRIGGER._SG_MEDIUM14`                     | tags.dat                                                                                     |
| 1902 | SG_Medium15                     | `TRIGGER._SG_MEDIUM15`                     | tags.dat                                                                                     |
| 1903 | SG_Medium16                     | `TRIGGER._SG_MEDIUM16`                     | tags.dat                                                                                     |
| 1904 | SG_Medium17                     | `TRIGGER._SG_MEDIUM17`                     | tags.dat                                                                                     |
| 1905 | SG_Medium18                     | `TRIGGER._SG_MEDIUM18`                     | tags.dat                                                                                     |
| 1906 | SG_Medium19                     | `TRIGGER._SG_MEDIUM19`                     | tags.dat                                                                                     |
| 1907 | SG_Medium20                     | `TRIGGER._SG_MEDIUM20`                     | tags.dat                                                                                     |
| 1908 | SH_Medium01                     | `TRIGGER._SH_MEDIUM01`                     | tags_hallways.dat                                                                            |
| 1909 | SH_Medium02                     | `TRIGGER._SH_MEDIUM02`                     | tags_hallways.dat                                                                            |
| 1910 | SH_Medium03                     | `TRIGGER._SH_MEDIUM03`                     | tags_hallways.dat                                                                            |
| 1911 | SH_Medium04                     | `TRIGGER._SH_MEDIUM04`                     | tags_hallways.dat                                                                            |
| 1912 | SH_Medium05                     | `TRIGGER._SH_MEDIUM05`                     | tags_hallways.dat                                                                            |
| 1913 | SH_Medium07                     | `TRIGGER._SH_MEDIUM07`                     | tags_hallways.dat                                                                            |
| 1914 | SH_Medium08                     | `TRIGGER._SH_MEDIUM08`                     | tags_hallways.dat                                                                            |
| 1915 | SH_Medium09                     | `TRIGGER._SH_MEDIUM09`                     | tags_hallways.dat                                                                            |
| 1916 | SND_BEACH                       | `TRIGGER._SND_BEACH`                       | SoundBankTriggers.dat                                                                        |
| 1917 | SND_BUSINESS_AREA               | `TRIGGER._SND_BUSINESS_AREA`               | SoundBankTriggers.dat                                                                        |
| 1918 | SND_CARNIVAL_AREA               | `TRIGGER._SND_CARNIVAL_AREA`               | SoundBankTriggers.dat                                                                        |
| 1919 | SND_CarnTunnelBank              | `TRIGGER._SND_CARNTUNNELBANK`              | SoundBankTriggers.dat                                                                        |
| 1920 | SND_DAM                         | `TRIGGER._SND_DAM`                         | SoundBankTriggers.dat                                                                        |
| 1921 | SND_DOCKYARD                    | `TRIGGER._SND_DOCKYARD`                    | SoundBankTriggers.dat                                                                        |
| 1922 | SND_INDUSTRIAL_AREA             | `TRIGGER._SND_INDUSTRIAL_AREA`             | SoundBankTriggers.dat                                                                        |
| 1923 | SND_POOR_AREA                   | `TRIGGER._SND_POOR_AREA`                   | SoundBankTriggers.dat                                                                        |
| 1924 | SND_RICHPARKSPRINKLERS          | `TRIGGER._SND_RICHPARKSPRINKLERS`          | SoundBankTriggers.dat                                                                        |
| 1925 | SND_RICH_AREA                   | `TRIGGER._SND_RICH_AREA`                   | SoundBankTriggers.dat                                                                        |
| 1926 | SND_Roundhouse                  | `TRIGGER._SND_ROUNDHOUSE`                  | SoundBankTriggers.dat                                                                        |
| 1927 | SND_SCHOOLPOND                  | `TRIGGER._SND_SCHOOLPOND`                  | SoundBankTriggers.dat                                                                        |
| 1928 | SND_SCHOOLTUNNEL01              | `TRIGGER._SND_SCHOOLTUNNEL01`              | SoundBankTriggers.dat                                                                        |
| 1929 | SND_SCHOOLTUNNEL02              | `TRIGGER._SND_SCHOOLTUNNEL02`              | SoundBankTriggers.dat                                                                        |
| 1930 | SND_SCHOOLTUNNEL03              | `TRIGGER._SND_SCHOOLTUNNEL03`              | SoundBankTriggers.dat                                                                        |
| 1931 | SND_SCHOOL_AREA                 | `TRIGGER._SND_SCHOOL_AREA`                 | SoundBankTriggers.dat                                                                        |
| 1932 | SND_SCHOOL_ROOF                 | `TRIGGER._SND_SCHOOL_ROOF`                 | SoundBankTriggers.dat                                                                        |
| 1933 | SND_WATER                       | `TRIGGER._SND_WATER`                       | SoundBankTriggers.dat                                                                        |
| 1934 | SOCCER_SHOOT_OUT_01             | `TRIGGER._SOCCER_SHOOT_OUT_01`             | PAn_Main.dat                                                                                 |
| 1935 | SOCCER_SHOOT_OUT_02             | `TRIGGER._SOCCER_SHOOT_OUT_02`             | PAn_Main.dat                                                                                 |
| 1936 | SO_Medium01                     | `TRIGGER._SO_MEDIUM01`                     | tags.dat                                                                                     |
| 1937 | SO_Medium02                     | `TRIGGER._SO_MEDIUM02`                     | tags.dat                                                                                     |
| 1938 | SO_Medium03                     | `TRIGGER._SO_MEDIUM03`                     | tags.dat                                                                                     |
| 1939 | SO_Medium04                     | `TRIGGER._SO_MEDIUM04`                     | tags.dat                                                                                     |
| 1940 | SO_Medium05                     | `TRIGGER._SO_MEDIUM05`                     | tags.dat                                                                                     |
| 1941 | ST1_dePopSnowArea               | `TRIGGER._ST1_DEPOPSNOWAREA`               | P_Snow1.dat                                                                                  |
| 1942 | ST2_dePopSnowArea               | `TRIGGER._ST2_DEPOPSNOWAREA`               | P_Snow2.dat                                                                                  |
| 1943 | ST3_dePopSnowArea               | `TRIGGER._ST3_DEPOPSNOWAREA`               | P_Snow3.dat                                                                                  |
| 1944 | ST4_dePopSnowArea               | `TRIGGER._ST4_DEPOPSNOWAREA`               | P_Snow4.dat                                                                                  |
| 1945 | ST5_dePopSnowArea               | `TRIGGER._ST5_DEPOPSNOWAREA`               | P_Snow5.dat                                                                                  |
| 1946 | ST6_dePopSnowArea               | `TRIGGER._ST6_DEPOPSNOWAREA`               | P_Snow6.dat                                                                                  |
| 1947 | STEALTH_PORTAPOTTY              | `TRIGGER._STEALTH_PORTAPOTTY`              | SpawnTest.dat                                                                                |
| 1948 | ST_CRATE_01                     | `TRIGGER._ST_CRATE_01`                     | SpawnTest.dat                                                                                |
| 1949 | ST_CRATE_02                     | `TRIGGER._ST_CRATE_02`                     | SpawnTest.dat                                                                                |
| 1950 | ST_CRATE_03                     | `TRIGGER._ST_CRATE_03`                     | SpawnTest.dat                                                                                |
| 1951 | ST_DOOR                         | `TRIGGER._ST_DOOR`                         | SpawnTest.dat                                                                                |
| 1952 | SV_BDormCrawl                   | `TRIGGER._SV_BDORMCRAWL`                   | AreaTran.dat                                                                                 |
| 1953 | SV_BioSchool                    | `TRIGGER._SV_BIOSCHOOL`                    | AreaTran.dat                                                                                 |
| 1954 | SV_CarnivalFunhouse             | `TRIGGER._SV_CARNIVALFUNHOUSE`             | AreaTran.dat                                                                                 |
| 1955 | SV_ChemSchool                   | `TRIGGER._SV_CHEMSCHOOL`                   | AreaTran.dat                                                                                 |
| 1956 | SV_ExtBDormCrawl                | `TRIGGER._SV_EXTBDORMCRAWL`                | AreaTran.dat                                                                                 |
| 1957 | SV_GirlsDorm                    | `TRIGGER._SV_GIRLSDORM`                    | AreaTran.dat                                                                                 |
| 1958 | SV_GirlsDormExit                | `TRIGGER._SV_GIRLSDORMEXIT`                | AreaTran.dat                                                                                 |
| 1959 | SandCasl                        | `TRIGGER._SANDCASL`                        | ttest.dat                                                                                    |
| 1960 | SaveBookBoysDorm                | `TRIGGER._SAVEBOOKBOYSDORM`                | BoysDorm.dat                                                                                 |
| 1961 | SaveBookDropouts                | `TRIGGER._SAVEBOOKDROPOUTS`                | SaveLocs.dat                                                                                 |
| 1962 | SaveBookGreasers                | `TRIGGER._SAVEBOOKGREASERS`                | SaveLocs.dat                                                                                 |
| 1963 | SaveBookJocks                   | `TRIGGER._SAVEBOOKJOCKS`                   | SaveLocs.dat                                                                                 |
| 1964 | SaveBookNerds                   | `TRIGGER._SAVEBOOKNERDS`                   | SaveLocs.dat                                                                                 |
| 1965 | SaveBookPreps                   | `TRIGGER._SAVEBOOKPREPS`                   | SaveLocs.dat                                                                                 |
| 1966 | ScGate_Observatory              | `TRIGGER._SCGATE_OBSERVATORY`              | tschool_maindoors.dat                                                                        |
| 1967 | SchoolArea                      | `TRIGGER._SCHOOLAREA`                      | Population.dat                                                                               |
| 1968 | SchoolBackR                     | `TRIGGER._SCHOOLBACKR`                     | C5.dat, PhotoZoom.dat                                                                        |
| 1969 | SchoolBikeTrig                  | `TRIGGER._SCHOOLBIKETRIG`                  | Population.dat                                                                               |
| 1970 | SchoolBio                       | `TRIGGER._SCHOOLBIO`                       | AreaTran.dat                                                                                 |
| 1971 | SchoolBoysWash                  | `TRIGGER._SCHOOLBOYSWASH`                  | SP_School_Hallways.dat                                                                       |
| 1972 | SchoolBoysWash2                 | `TRIGGER._SCHOOLBOYSWASH2`                 | SP_School_Hallways.dat                                                                       |
| 1973 | SchoolCaf1                      | `TRIGGER._SCHOOLCAF1`                      | AreaTran.dat                                                                                 |
| 1974 | SchoolCaf2                      | `TRIGGER._SCHOOLCAF2`                      | AreaTran.dat                                                                                 |
| 1975 | SchoolCafeteria                 | `TRIGGER._SCHOOLCAFETERIA`                 | SP_School_Hallways.dat                                                                       |
| 1976 | SchoolChem                      | `TRIGGER._SCHOOLCHEM`                      | AreaTran.dat                                                                                 |
| 1977 | SchoolDepop                     | `TRIGGER._SCHOOLDEPOP`                     | GraffitiPunishment.dat                                                                       |
| 1978 | SchoolEnglish                   | `TRIGGER._SCHOOLENGLISH`                   | AreaTran.dat                                                                                 |
| 1979 | SchoolEntrL1                    | `TRIGGER._SCHOOLENTRL1`                    | C5.dat, PhotoZoom.dat                                                                        |
| 1980 | SchoolEntrL2                    | `TRIGGER._SCHOOLENTRL2`                    | C5.dat, PhotoZoom.dat                                                                        |
| 1981 | SchoolEntrR1                    | `TRIGGER._SCHOOLENTRR1`                    | C5.dat, PhotoZoom.dat                                                                        |
| 1982 | SchoolEntrR2                    | `TRIGGER._SCHOOLENTRR2`                    | C5.dat, PhotoZoom.dat                                                                        |
| 1983 | SchoolEntranceTrig              | `TRIGGER._SCHOOLENTRANCETRIG`              | 6_02.dat                                                                                     |
| 1984 | SchoolGameArea                  | `TRIGGER._SCHOOLGAMEAREA`                  | GraffitiPunishment.dat                                                                       |
| 1985 | SchoolGirlsWash                 | `TRIGGER._SCHOOLGIRLSWASH`                 | SP_School_Hallways.dat                                                                       |
| 1986 | SchoolGirlsWash2                | `TRIGGER._SCHOOLGIRLSWASH2`                | SP_School_Hallways.dat                                                                       |
| 1987 | SchoolHallRoofStairway          | `TRIGGER._SCHOOLHALLROOFSTAIRWAY`          | SP_School_Hallways.dat                                                                       |
| 1988 | SchoolHalls01                   | `TRIGGER._SCHOOLHALLS01`                   | SP_School_Hallways.dat                                                                       |
| 1989 | SchoolHalls02                   | `TRIGGER._SCHOOLHALLS02`                   | SP_School_Hallways.dat                                                                       |
| 1990 | SchoolMain                      | `TRIGGER._SCHOOLMAIN`                      | AreaTran.dat                                                                                 |
| 1991 | SchoolMainAtrium                | `TRIGGER._SCHOOLMAINATRIUM`                | SP_School_Hallways.dat                                                                       |
| 1992 | SchoolNurse                     | `TRIGGER._SCHOOLNURSE`                     | AreaTran.dat                                                                                 |
| 1993 | SchoolPrincipal                 | `TRIGGER._SCHOOLPRINCIPAL`                 | AreaTran.dat                                                                                 |
| 1994 | SchoolRoofTrig                  | `TRIGGER._SCHOOLROOFTRIG`                  | 6_02.dat                                                                                     |
| 1995 | SchoolSecondFloor               | `TRIGGER._SCHOOLSECONDFLOOR`               | C5.dat, PhotoZoom.dat                                                                        |
| 1996 | SchoolSideTrig                  | `TRIGGER._SCHOOLSIDETRIG`                  | 6_02.dat                                                                                     |
| 1997 | SchoolStoreExc                  | `TRIGGER._SCHOOLSTOREEXC`                  | eventsSchoolHalls.dat                                                                        |
| 1998 | SchoolTower                     | `TRIGGER._SCHOOLTOWER`                     | C5.dat, PhotoZoom.dat                                                                        |
| 1999 | SchoolTrig                      | `TRIGGER._SCHOOLTRIG`                      | 6_02.dat                                                                                     |
| 2000 | School_Basketball_Court         | `TRIGGER._SCHOOL_BASKETBALL_COURT`         | Population.dat                                                                               |
| 2001 | School_Turret                   | `TRIGGER._SCHOOL_TURRET`                   | SP_MainMap.dat                                                                               |
| 2002 | School_TurretTripod             | `TRIGGER._SCHOOL_TURRETTRIPOD`             | SP_MainMap.dat                                                                               |
| 2003 | Silo                            | `TRIGGER._SILO`                            | PhotoFilters.dat                                                                             |
| 2004 | SmallCrate1                     | `TRIGGER._SMALLCRATE1`                     | SpawnTest.dat                                                                                |
| 2005 | SmallCrate10                    | `TRIGGER._SMALLCRATE10`                    | SpawnTest.dat                                                                                |
| 2006 | SmallCrate11                    | `TRIGGER._SMALLCRATE11`                    | SpawnTest.dat                                                                                |
| 2007 | SmallCrate2                     | `TRIGGER._SMALLCRATE2`                     | SpawnTest.dat                                                                                |
| 2008 | SmallCrate3                     | `TRIGGER._SMALLCRATE3`                     | SpawnTest.dat                                                                                |
| 2009 | SmallCrate5                     | `TRIGGER._SMALLCRATE5`                     | SpawnTest.dat                                                                                |
| 2010 | SmallCrate6                     | `TRIGGER._SMALLCRATE6`                     | SpawnTest.dat                                                                                |
| 2011 | SmallCrate7                     | `TRIGGER._SMALLCRATE7`                     | SpawnTest.dat                                                                                |
| 2012 | SmallCrate9                     | `TRIGGER._SMALLCRATE9`                     | SpawnTest.dat                                                                                |
| 2013 | Snowman                         | `TRIGGER._SNOWMAN`                         | ttest.dat                                                                                    |
| 2014 | SouvienrShop                    | `TRIGGER._SOUVIENRSHOP`                    | SP_Souvenir.dat                                                                              |
| 2015 | SpawnKiss                       | `TRIGGER._SPAWNKISS`                       | RobertoTest.dat                                                                              |
| 2016 | SpawnTest_Door1                 | `TRIGGER._SPAWNTEST_DOOR1`                 | SpawnTest.dat                                                                                |
| 2017 | SpawnTest_Door2                 | `TRIGGER._SPAWNTEST_DOOR2`                 | SpawnTest.dat                                                                                |
| 2018 | SpawnTest_Trig1                 | `TRIGGER._SPAWNTEST_TRIG1`                 | SpawnTest.dat                                                                                |
| 2019 | Spud_Cannon_Bottom              | `TRIGGER._SPUD_CANNON_BOTTOM`              | TFight01.dat                                                                                 |
| 2020 | Spud_Cannon_Top                 | `TRIGGER._SPUD_CANNON_TOP`                 | TFight01.dat                                                                                 |
| 2021 | Squid                           | `TRIGGER._SQUID`                           | tcarni.dat                                                                                   |
| 2022 | Stable                          | `TRIGGER._STABLE`                          | ttest.dat                                                                                    |
| 2023 | Stag1Trig                       | `TRIGGER._STAG1TRIG`                       | 3_06New.dat                                                                                  |
| 2024 | Stag2Trig                       | `TRIGGER._STAG2TRIG`                       | 3_06New.dat                                                                                  |
| 2025 | StalDoor01                      | `TRIGGER._STALDOOR01`                      | 1_05.dat                                                                                     |
| 2026 | StalDoor02                      | `TRIGGER._STALDOOR02`                      | 1_05.dat                                                                                     |
| 2027 | StalDoor11                      | `TRIGGER._STALDOOR11`                      | 1_05.dat                                                                                     |
| 2028 | StatueL                         | `TRIGGER._STATUEL`                         | C5.dat, PhotoZoom.dat                                                                        |
| 2029 | StatueR                         | `TRIGGER._STATUER`                         | C5.dat, PhotoZoom.dat                                                                        |
| 2030 | StoreCarn_Area                  | `TRIGGER._STORECARN_AREA`                  | CarnStore.dat                                                                                |
| 2031 | Store_BarberPoor_Area           | `TRIGGER._STORE_BARBERPOOR_AREA`           | ibarber.dat                                                                                  |
| 2032 | Store_Barber_Area               | `TRIGGER._STORE_BARBER_AREA`               | ibarber.dat                                                                                  |
| 2033 | Store_DT_BikeArea               | `TRIGGER._STORE_DT_BIKEAREA`               | Store.dat                                                                                    |
| 2034 | Store_DT_ComicArea              | `TRIGGER._STORE_DT_COMICAREA`              | Store.dat                                                                                    |
| 2035 | Store_DT_GeneralArea            | `TRIGGER._STORE_DT_GENERALAREA`            | Store.dat                                                                                    |
| 2036 | Store_HairSalon_Area            | `TRIGGER._STORE_HAIRSALON_AREA`            | ibarber.dat                                                                                  |
| 2037 | TEMPCar1                        | `TRIGGER._TEMPCAR1`                        | P_Snow4.dat, P_Snow5.dat, P_Snow6.dat                                                        |
| 2038 | TEMPCar2                        | `TRIGGER._TEMPCAR2`                        | P_Snow4.dat, P_Snow5.dat, P_Snow6.dat                                                        |
| 2039 | TEMPCar3                        | `TRIGGER._TEMPCAR3`                        | P_Snow4.dat, P_Snow6.dat                                                                     |
| 2040 | TENEMENTS_FIRE_ESCAPE_CAMERA    | `TRIGGER._TENEMENTS_FIRE_ESCAPE_CAMERA`    | tenements.dat                                                                                |
| 2041 | TEN_FIRE01                      | `TRIGGER._TEN_FIRE01`                      | TenErrands.dat                                                                               |
| 2042 | TEN_FIRE02                      | `TRIGGER._TEN_FIRE02`                      | TenErrands.dat                                                                               |
| 2043 | TEN_FIRE03                      | `TRIGGER._TEN_FIRE03`                      | TenErrands.dat                                                                               |
| 2044 | TEN_FIRE04                      | `TRIGGER._TEN_FIRE04`                      | TenErrands.dat                                                                               |
| 2045 | TEN_FIRE05                      | `TRIGGER._TEN_FIRE05`                      | TenErrands.dat                                                                               |
| 2046 | TEN_FIRE06                      | `TRIGGER._TEN_FIRE06`                      | TenErrands.dat                                                                               |
| 2047 | TEN_FIRE07                      | `TRIGGER._TEN_FIRE07`                      | TenErrands.dat                                                                               |
| 2048 | TEN_FIRE08                      | `TRIGGER._TEN_FIRE08`                      | TenErrands.dat                                                                               |
| 2049 | TEN_FIRE09                      | `TRIGGER._TEN_FIRE09`                      | TenErrands.dat                                                                               |
| 2050 | TEN_FIRE10                      | `TRIGGER._TEN_FIRE10`                      | TenErrands.dat                                                                               |
| 2051 | TF02_Fight1                     | `TRIGGER._TF02_FIGHT1`                     | TFight02.dat                                                                                 |
| 2052 | TF02_Fight2                     | `TRIGGER._TF02_FIGHT2`                     | TFight02.dat                                                                                 |
| 2053 | TFIGHT01_Barricade              | `TRIGGER._TFIGHT01_BARRICADE`              | TFight01.dat                                                                                 |
| 2054 | TFIGHT01_Cannon_Nerd            | `TRIGGER._TFIGHT01_CANNON_NERD`            | TFight01.dat                                                                                 |
| 2055 | TFIGHT01_Door1                  | `TRIGGER._TFIGHT01_DOOR1`                  | TFight01.dat                                                                                 |
| 2056 | TFIGHT01_Door2                  | `TRIGGER._TFIGHT01_DOOR2`                  | TFight01.dat                                                                                 |
| 2057 | TFIGHT01_Door3                  | `TRIGGER._TFIGHT01_DOOR3`                  | TFight01.dat                                                                                 |
| 2058 | TFIGHT01_Door4                  | `TRIGGER._TFIGHT01_DOOR4`                  | TFight01.dat                                                                                 |
| 2059 | TINDUST_ASYLUM                  | `TRIGGER._TINDUST_ASYLUM`                  | tindustrial.dat                                                                              |
| 2060 | TINDUST_BAR_DOOR_01             | `TRIGGER._TINDUST_BAR_DOOR_01`             | PAn_Main.dat                                                                                 |
| 2061 | TINDUST_BAR_DOOR_02             | `TRIGGER._TINDUST_BAR_DOOR_02`             | PAn_Main.dat                                                                                 |
| 2062 | TINDUST_BAR_DOOR_03             | `TRIGGER._TINDUST_BAR_DOOR_03`             | PAn_Main.dat                                                                                 |
| 2063 | TINDUST_BAR_DOOR_PORT           | `TRIGGER._TINDUST_BAR_DOOR_PORT`           | PAn_Main.dat                                                                                 |
| 2064 | TINDUST_BAR_DOOR_SWITCH_01      | `TRIGGER._TINDUST_BAR_DOOR_SWITCH_01`      | PAn_Main.dat                                                                                 |
| 2065 | TINDUST_BAR_DOOR_SWITCH_02      | `TRIGGER._TINDUST_BAR_DOOR_SWITCH_02`      | PAn_Main.dat                                                                                 |
| 2066 | TINDUST_BAR_DOOR_SWITCH_03      | `TRIGGER._TINDUST_BAR_DOOR_SWITCH_03`      | PAn_Main.dat                                                                                 |
| 2067 | TINDUST_BAR_DOOR_SWITCH_PORT    | `TRIGGER._TINDUST_BAR_DOOR_SWITCH_PORT`    | PAn_Main.dat                                                                                 |
| 2068 | TINDUST_ELECTRIC_SHUTOFF        | `TRIGGER._TINDUST_ELECTRIC_SHUTOFF`        | PAn_Main.dat                                                                                 |
| 2069 | TINDUST_FIRE_DOOR_01            | `TRIGGER._TINDUST_FIRE_DOOR_01`            | PAn_Main.dat                                                                                 |
| 2070 | TINDUST_FIRE_DOOR_02            | `TRIGGER._TINDUST_FIRE_DOOR_02`            | PAn_Main.dat                                                                                 |
| 2071 | TINDUST_GATE_SWITCH             | `TRIGGER._TINDUST_GATE_SWITCH`             | PAn_Main.dat                                                                                 |
| 2072 | TINDUST_POWER_SWITCH_01         | `TRIGGER._TINDUST_POWER_SWITCH_01`         | PAn_Main.dat                                                                                 |
| 2073 | TINDUST_POWER_SWITCH_02         | `TRIGGER._TINDUST_POWER_SWITCH_02`         | PAn_Main.dat                                                                                 |
| 2074 | TINDUST_REDSTAR_GATE_01         | `TRIGGER._TINDUST_REDSTAR_GATE_01`         | PAn_Main.dat                                                                                 |
| 2075 | TINDUST_REDSTAR_SECURITY_DOOR   | `TRIGGER._TINDUST_REDSTAR_SECURITY_DOOR`   | PAn_Main.dat                                                                                 |
| 2076 | TINDUST_SHDOOR_03               | `TRIGGER._TINDUST_SHDOOR_03`               | PAn_Main.dat                                                                                 |
| 2077 | TINDUST_SHDOOR_04               | `TRIGGER._TINDUST_SHDOOR_04`               | PAn_Main.dat                                                                                 |
| 2078 | TINDUST_SHDOOR_05               | `TRIGGER._TINDUST_SHDOOR_05`               | PAn_Main.dat                                                                                 |
| 2079 | TINDUST_SHDOOR_06               | `TRIGGER._TINDUST_SHDOOR_06`               | PAn_Main.dat                                                                                 |
| 2080 | TINDUST_SHDOOR_07               | `TRIGGER._TINDUST_SHDOOR_07`               | PAn_Main.dat                                                                                 |
| 2081 | TINDUST_TRAIN_SWITCH_01         | `TRIGGER._TINDUST_TRAIN_SWITCH_01`         | PAn_Main.dat                                                                                 |
| 2082 | TINDUST_TRAIN_SWITCH_02         | `TRIGGER._TINDUST_TRAIN_SWITCH_02`         | PAn_Main.dat                                                                                 |
| 2083 | TPHOTO_FIRE                     | `TRIGGER._TPHOTO_FIRE`                     | tphoto.dat                                                                                   |
| 2084 | TPHOTO_FIREG                    | `TRIGGER._TPHOTO_FIREG`                    | tphotoglass.dat                                                                              |
| 2085 | TadBackDoorL                    | `TRIGGER._TADBACKDOORL`                    | trich_doors.dat                                                                              |
| 2086 | TadBackDoorR                    | `TRIGGER._TADBACKDOORR`                    | trich_doors.dat                                                                              |
| 2087 | TadFrontDoorL                   | `TRIGGER._TADFRONTDOORL`                   | trich_doors.dat                                                                              |
| 2088 | TadFrontDoorR                   | `TRIGGER._TADFRONTDOORR`                   | trich_doors.dat                                                                              |
| 2089 | TadGates02                      | `TRIGGER._TADGATES02`                      | trich.dat                                                                                    |
| 2090 | TadShud                         | `TRIGGER._TADSHUD`                         | trich_doors.dat                                                                              |
| 2091 | TadShud01                       | `TRIGGER._TADSHUD01`                       | trich_doors.dat                                                                              |
| 2092 | TadShud02                       | `TRIGGER._TADSHUD02`                       | trich_doors.dat                                                                              |
| 2093 | TadShud03                       | `TRIGGER._TADSHUD03`                       | trich_doors.dat                                                                              |
| 2094 | TadShud04                       | `TRIGGER._TADSHUD04`                       | trich_doors.dat                                                                              |
| 2095 | TadShud05                       | `TRIGGER._TADSHUD05`                       | trich_doors.dat                                                                              |
| 2096 | Tenements_Balcony               | `TRIGGER._TENEMENTS_BALCONY`               | SP_Tenement.dat                                                                              |
| 2097 | Tenements_Bathroom              | `TRIGGER._TENEMENTS_BATHROOM`              | SP_Tenement.dat                                                                              |
| 2098 | Tenements_Hall01                | `TRIGGER._TENEMENTS_HALL01`                | SP_Tenement.dat                                                                              |
| 2099 | Tenements_Hall02                | `TRIGGER._TENEMENTS_HALL02`                | SP_Tenement.dat                                                                              |
| 2100 | Tenements_Hall03                | `TRIGGER._TENEMENTS_HALL03`                | SP_Tenement.dat                                                                              |
| 2101 | Tenements_Hole                  | `TRIGGER._TENEMENTS_HOLE`                  | SP_Tenement.dat                                                                              |
| 2102 | Tenements_Hole02                | `TRIGGER._TENEMENTS_HOLE02`                | SP_Tenement.dat                                                                              |
| 2103 | Tenements_Rm01                  | `TRIGGER._TENEMENTS_RM01`                  | SP_Tenement.dat                                                                              |
| 2104 | Tenements_Rm02                  | `TRIGGER._TENEMENTS_RM02`                  | SP_Tenement.dat                                                                              |
| 2105 | Tenements_Rm03                  | `TRIGGER._TENEMENTS_RM03`                  | SP_Tenement.dat                                                                              |
| 2106 | Tenements_Rm04                  | `TRIGGER._TENEMENTS_RM04`                  | SP_Tenement.dat                                                                              |
| 2107 | Tenements_Rm05                  | `TRIGGER._TENEMENTS_RM05`                  | SP_Tenement.dat                                                                              |
| 2108 | Tenements_Rm06                  | `TRIGGER._TENEMENTS_RM06`                  | SP_Tenement.dat                                                                              |
| 2109 | Tenements_Rm07                  | `TRIGGER._TENEMENTS_RM07`                  | SP_Tenement.dat                                                                              |
| 2110 | Tenements_Rm08                  | `TRIGGER._TENEMENTS_RM08`                  | SP_Tenement.dat                                                                              |
| 2111 | Tenements_Rm09                  | `TRIGGER._TENEMENTS_RM09`                  | SP_Tenement.dat                                                                              |
| 2112 | Tenements_Rm10                  | `TRIGGER._TENEMENTS_RM10`                  | SP_Tenement.dat                                                                              |
| 2113 | Tenements_Rm11                  | `TRIGGER._TENEMENTS_RM11`                  | SP_Tenement.dat                                                                              |
| 2114 | Tenements_Rm12                  | `TRIGGER._TENEMENTS_RM12`                  | SP_Tenement.dat                                                                              |
| 2115 | Tenements_Rm13                  | `TRIGGER._TENEMENTS_RM13`                  | SP_Tenement.dat                                                                              |
| 2116 | Tenements_base_stair            | `TRIGGER._TENEMENTS_BASE_STAIR`            | SP_Tenement.dat                                                                              |
| 2117 | Tenements_basement              | `TRIGGER._TENEMENTS_BASEMENT`              | SP_Tenement.dat                                                                              |
| 2118 | TennFrid                        | `TRIGGER._TENNFRID`                        | ttest.dat                                                                                    |
| 2119 | TennWash                        | `TRIGGER._TENNWASH`                        | ttest.dat                                                                                    |
| 2120 | TestBikeGraffiti                | `TRIGGER._TESTBIKEGRAFFITI`                | TestBikeObjectives.dat                                                                       |
| 2121 | TestMailboxTarget               | `TRIGGER._TESTMAILBOXTARGET`               | TestMailboxTarget.dat                                                                        |
| 2122 | TestProjDetectionWall           | `TRIGGER._TESTPROJDETECTIONWALL`           | TestProjDetection.dat                                                                        |
| 2123 | TestTriggerEvent                | `TRIGGER._TESTTRIGGEREVENT`                | TestTriggerEvent.dat                                                                         |
| 2124 | TetherD101                      | `TRIGGER._TETHERD101`                      | 4_B2.dat                                                                                     |
| 2125 | TetherD102                      | `TRIGGER._TETHERD102`                      | 4_B2.dat                                                                                     |
| 2126 | TetherD103                      | `TRIGGER._TETHERD103`                      | 4_B2.dat                                                                                     |
| 2127 | TetherD104                      | `TRIGGER._TETHERD104`                      | 4_B2.dat                                                                                     |
| 2128 | TetherD105                      | `TRIGGER._TETHERD105`                      | 4_B2.dat                                                                                     |
| 2129 | TetherD201                      | `TRIGGER._TETHERD201`                      | 4_B2.dat                                                                                     |
| 2130 | TetherD202                      | `TRIGGER._TETHERD202`                      | 4_B2.dat                                                                                     |
| 2131 | TetherD203                      | `TRIGGER._TETHERD203`                      | 4_B2.dat                                                                                     |
| 2132 | TetherD204                      | `TRIGGER._TETHERD204`                      | 4_B2.dat                                                                                     |
| 2133 | TetherD205                      | `TRIGGER._TETHERD205`                      | 4_B2.dat                                                                                     |
| 2134 | TetherD301                      | `TRIGGER._TETHERD301`                      | 4_B2.dat                                                                                     |
| 2135 | TetherD302                      | `TRIGGER._TETHERD302`                      | 4_B2.dat                                                                                     |
| 2136 | TetherD303                      | `TRIGGER._TETHERD303`                      | 4_B2.dat                                                                                     |
| 2137 | TetherD304                      | `TRIGGER._TETHERD304`                      | 4_B2.dat                                                                                     |
| 2138 | TetherD305                      | `TRIGGER._TETHERD305`                      | 4_B2.dat                                                                                     |
| 2139 | Theatre                         | `TRIGGER._THEATRE`                         | PhotoFilters.dat                                                                             |
| 2140 | ThievesTrigger                  | `TRIGGER._THIEVESTRIGGER`                  | 1_08.dat                                                                                     |
| 2141 | ThirdFight                      | `TRIGGER._THIRDFIGHT`                      | 3_06New.dat                                                                                  |
| 2142 | TicketPickup                    | `TRIGGER._TICKETPICKUP`                    | RobertoTest.dat                                                                              |
| 2143 | Toys                            | `TRIGGER._TOYS`                            | PhotoFilters.dat                                                                             |
| 2144 | TrainYard                       | `TRIGGER._TRAINYARD`                       | SoundTriggers.dat                                                                            |
| 2145 | Transmitter                     | `TRIGGER._TRANSMITTER`                     | 1_06.dat                                                                                     |
| 2146 | TriggerArea                     | `TRIGGER._TRIGGERAREA`                     | 1_06.dat                                                                                     |
| 2147 | TrophyL                         | `TRIGGER._TROPHYL`                         | C5.dat, PhotoZoom.dat                                                                        |
| 2148 | TrophyR                         | `TRIGGER._TROPHYR`                         | C5.dat, PhotoZoom.dat                                                                        |
| 2149 | UmpireFive                      | `TRIGGER._UMPIREFIVE`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 2150 | UmpireFour                      | `TRIGGER._UMPIREFOUR`                      | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 2151 | UmpireOne                       | `TRIGGER._UMPIREONE`                       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 2152 | UmpireSeven                     | `TRIGGER._UMPIRESEVEN`                     | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 2153 | UmpireSix                       | `TRIGGER._UMPIRESIX`                       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 2154 | UmpireThree                     | `TRIGGER._UMPIRETHREE`                     | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 2155 | UmpireTwo                       | `TRIGGER._UMPIRETWO`                       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 2156 | WM_GoKartCreate                 | `TRIGGER._WM_GOKARTCREATE`                 | SP_MainMap.dat                                                                               |
| 2157 | WareHouse_Amb01                 | `TRIGGER._WAREHOUSE_AMB01`                 | SP_WareHouse.dat                                                                             |
| 2158 | Water                           | `TRIGGER._WATER`                           | PhotoFilters.dat                                                                             |
| 2159 | Wires                           | `TRIGGER._WIRES`                           | PhotoFilters.dat                                                                             |
| 2160 | ZoneBusiness                    | `TRIGGER._ZONEBUSINESS`                    | MainMapZones.dat                                                                             |
| 2161 | ZoneCarnival                    | `TRIGGER._ZONECARNIVAL`                    | MainMapZones.dat                                                                             |
| 2162 | ZoneIndustrial                  | `TRIGGER._ZONEINDUSTRIAL`                  | MainMapZones.dat                                                                             |
| 2163 | ZonePoor                        | `TRIGGER._ZONEPOOR`                        | MainMapZones.dat                                                                             |
| 2164 | ZoneRich                        | `TRIGGER._ZONERICH`                        | MainMapZones.dat                                                                             |
| 2165 | ZoneSchool                      | `TRIGGER._ZONESCHOOL`                      | MainMapZones.dat                                                                             |
| 2166 | \_SSI_00                        | `TRIGGER.__SSI_00`                         | stopsigns.dat                                                                                |
| 2167 | \_SSI_01                        | `TRIGGER.__SSI_01`                         | stopsigns.dat                                                                                |
| 2168 | \_SSI_02                        | `TRIGGER.__SSI_02`                         | stopsigns.dat                                                                                |
| 2169 | \_SSI_03                        | `TRIGGER.__SSI_03`                         | stopsigns.dat                                                                                |
| 2170 | \_SSI_04                        | `TRIGGER.__SSI_04`                         | stopsigns.dat                                                                                |
| 2171 | \_SSI_05                        | `TRIGGER.__SSI_05`                         | stopsigns.dat                                                                                |
| 2172 | \_SSI_06                        | `TRIGGER.__SSI_06`                         | stopsigns.dat                                                                                |
| 2173 | \_SSI_07                        | `TRIGGER.__SSI_07`                         | stopsigns.dat                                                                                |
| 2174 | \_SSI_08                        | `TRIGGER.__SSI_08`                         | stopsigns.dat                                                                                |
| 2175 | \_SSI_09                        | `TRIGGER.__SSI_09`                         | stopsigns.dat                                                                                |
| 2176 | \_SSI_10                        | `TRIGGER.__SSI_10`                         | stopsigns.dat                                                                                |
| 2177 | \_SSI_11                        | `TRIGGER.__SSI_11`                         | stopsigns.dat                                                                                |
| 2178 | \_SSI_12                        | `TRIGGER.__SSI_12`                         | stopsigns.dat                                                                                |
| 2179 | \_SSI_13                        | `TRIGGER.__SSI_13`                         | stopsigns.dat                                                                                |
| 2180 | \_SSI_14                        | `TRIGGER.__SSI_14`                         | stopsigns.dat                                                                                |
| 2181 | \_SSI_15                        | `TRIGGER.__SSI_15`                         | stopsigns.dat                                                                                |
| 2182 | \_SSI_16                        | `TRIGGER.__SSI_16`                         | stopsigns.dat                                                                                |
| 2183 | \_SSI_17                        | `TRIGGER.__SSI_17`                         | stopsigns.dat                                                                                |
| 2184 | \_SSI_18                        | `TRIGGER.__SSI_18`                         | stopsigns.dat                                                                                |
| 2185 | \_SSI_19                        | `TRIGGER.__SSI_19`                         | stopsigns.dat                                                                                |
| 2186 | \_SSI_20                        | `TRIGGER.__SSI_20`                         | stopsigns.dat                                                                                |
| 2187 | \_SSI_21                        | `TRIGGER.__SSI_21`                         | stopsigns.dat                                                                                |
| 2188 | \_SSI_22                        | `TRIGGER.__SSI_22`                         | stopsigns.dat                                                                                |
| 2189 | \_SSI_23                        | `TRIGGER.__SSI_23`                         | stopsigns.dat                                                                                |
| 2190 | \_SSI_24                        | `TRIGGER.__SSI_24`                         | stopsigns.dat                                                                                |
| 2191 | \_SSI_25                        | `TRIGGER.__SSI_25`                         | stopsigns.dat                                                                                |
| 2192 | \_SSI_26                        | `TRIGGER.__SSI_26`                         | stopsigns.dat                                                                                |
| 2193 | \_SSI_27                        | `TRIGGER.__SSI_27`                         | stopsigns.dat                                                                                |
| 2194 | \_SSI_28                        | `TRIGGER.__SSI_28`                         | stopsigns.dat                                                                                |
| 2195 | \_SSI_29                        | `TRIGGER.__SSI_29`                         | stopsigns.dat                                                                                |
| 2196 | \_SSI_30                        | `TRIGGER.__SSI_30`                         | stopsigns.dat                                                                                |
| 2197 | \_SSI_31                        | `TRIGGER.__SSI_31`                         | stopsigns.dat                                                                                |
| 2198 | auditorium_doorR                | `TRIGGER._AUDITORIUM_DOORR`                | eventsAuditorium.dat                                                                         |
| 2199 | barricade102                    | `TRIGGER._BARRICADE102`                    | 3_01A.dat                                                                                    |
| 2200 | boysDormCourtyard               | `TRIGGER._BOYSDORMCOURTYARD`               | tschool_maindoors.dat                                                                        |
| 2201 | bu_DoorStr10                    | `TRIGGER._BU_DOORSTR10`                    | tbusines_doors.dat                                                                           |
| 2202 | bu_PrepDoor13                   | `TRIGGER._BU_PREPDOOR13`                   | tbusines_doors.dat                                                                           |
| 2203 | bu_PrepDoor14                   | `TRIGGER._BU_PREPDOOR14`                   | tbusines_doors.dat                                                                           |
| 2204 | bu_PrepDoor15                   | `TRIGGER._BU_PREPDOOR15`                   | tbusines_doors.dat                                                                           |
| 2205 | bu_PrepDoor16                   | `TRIGGER._BU_PREPDOOR16`                   | tbusines_doors.dat                                                                           |
| 2206 | bu_PrepDoor17                   | `TRIGGER._BU_PREPDOOR17`                   | tbusines_doors.dat                                                                           |
| 2207 | bu_PrepDoor18                   | `TRIGGER._BU_PREPDOOR18`                   | tbusines_doors.dat                                                                           |
| 2208 | bu_PrepDoor19                   | `TRIGGER._BU_PREPDOOR19`                   | tbusines_doors.dat                                                                           |
| 2209 | bu_PrepDoor20                   | `TRIGGER._BU_PREPDOOR20`                   | tbusines_doors.dat                                                                           |
| 2210 | bu_PrepDoor21                   | `TRIGGER._BU_PREPDOOR21`                   | tbusines_doors.dat                                                                           |
| 2211 | bu_PrepDoor22                   | `TRIGGER._BU_PREPDOOR22`                   | tbusines_doors.dat                                                                           |
| 2212 | bu_PrepDoor23                   | `TRIGGER._BU_PREPDOOR23`                   | tbusines_doors.dat                                                                           |
| 2213 | bu_PrepDoor24                   | `TRIGGER._BU_PREPDOOR24`                   | tbusines_doors.dat                                                                           |
| 2214 | bu_PrepDoor25                   | `TRIGGER._BU_PREPDOOR25`                   | tbusines_doors.dat                                                                           |
| 2215 | carnGate01                      | `TRIGGER._CARNGATE01`                      | tcarni.dat                                                                                   |
| 2216 | carnGate02                      | `TRIGGER._CARNGATE02`                      | tcarni.dat                                                                                   |
| 2217 | carnGate03                      | `TRIGGER._CARNGATE03`                      | tcarni.dat                                                                                   |
| 2218 | carnGate04                      | `TRIGGER._CARNGATE04`                      | tcarni.dat                                                                                   |
| 2219 | crate01                         | `TRIGGER._CRATE01`                         | mlee_pickups.dat                                                                             |
| 2220 | dowtownDepop                    | `TRIGGER._DOWTOWNDEPOP`                    | GraffitiPunishment.dat                                                                       |
| 2221 | funCurtn                        | `TRIGGER._FUNCURTN`                        | ifunhous.dat                                                                                 |
| 2222 | funCurtn01                      | `TRIGGER._FUNCURTN01`                      | ifunhous.dat                                                                                 |
| 2223 | fun_MazeEntryDoor               | `TRIGGER._FUN_MAZEENTRYDOOR`               | ifunhous.dat                                                                                 |
| 2224 | gd_GameArea                     | `TRIGGER._GD_GAMEAREA`                     | GarbPickDowntown.dat                                                                         |
| 2225 | gd_TrashArea                    | `TRIGGER._GD_TRASHAREA`                    | GarbPickDowntown.dat                                                                         |
| 2226 | gdorm_DoorR                     | `TRIGGER._GDORM_DOORR`                     | Gdorm.dat                                                                                    |
| 2227 | girlsDormCourtyard              | `TRIGGER._GIRLSDORMCOURTYARD`              | tschool_maindoors.dat                                                                        |
| 2228 | gnomeA                          | `TRIGGER._GNOMEA`                          | ttest.dat                                                                                    |
| 2229 | gs_GameArea                     | `TRIGGER._GS_GAMEAREA`                     | GarbPickSchool.dat                                                                           |
| 2230 | gs_TrashArea                    | `TRIGGER._GS_TRASHAREA`                    | GarbPickSchool.dat                                                                           |
| 2231 | gym_pool                        | `TRIGGER._GYM_POOL`                        | gym_pool.dat                                                                                 |
| 2232 | gyml_doorR                      | `TRIGGER._GYML_DOORR`                      | eventsGymAndPool.dat                                                                         |
| 2233 | hardwareback                    | `TRIGGER._HARDWAREBACK`                    | tbusines_doors.dat                                                                           |
| 2234 | iboxing_BoxRopes                | `TRIGGER._IBOXING_BOXROPES`                | iboxing.dat                                                                                  |
| 2235 | iboxing_BoxRopes01              | `TRIGGER._IBOXING_BOXROPES01`              | iboxing.dat                                                                                  |
| 2236 | iboxing_BoxRopes02              | `TRIGGER._IBOXING_BOXROPES02`              | iboxing.dat                                                                                  |
| 2237 | iboxing_BoxRopes03              | `TRIGGER._IBOXING_BOXROPES03`              | iboxing.dat                                                                                  |
| 2238 | iboxing_ESCDoorL                | `TRIGGER._IBOXING_ESCDOORL`                | iboxing.dat                                                                                  |
| 2239 | iboxing_ESCDoorL01              | `TRIGGER._IBOXING_ESCDOORL01`              | iboxing.dat                                                                                  |
| 2240 | iboxing_ESCDoorR                | `TRIGGER._IBOXING_ESCDOORR`                | iboxing.dat                                                                                  |
| 2241 | iboxing_ESCDoorR01              | `TRIGGER._IBOXING_ESCDOORR01`              | iboxing.dat                                                                                  |
| 2242 | iboxing_IntDoor02               | `TRIGGER._IBOXING_INTDOOR02`               | iboxing.dat                                                                                  |
| 2243 | iboxing_barvault01              | `TRIGGER._IBOXING_BARVAULT01`              | iboxing.dat                                                                                  |
| 2244 | iboxing_barvault02              | `TRIGGER._IBOXING_BARVAULT02`              | iboxing.dat                                                                                  |
| 2245 | iboxing_fakeCoronaTrigger       | `TRIGGER._IBOXING_FAKECORONATRIGGER`       | iboxing.dat                                                                                  |
| 2246 | icecream                        | `TRIGGER._ICECREAM`                        | trich_doors.dat                                                                              |
| 2247 | icloth_p_trigger                | `TRIGGER._ICLOTH_P_TRIGGER`                | icloth_p.dat                                                                                 |
| 2248 | icomshp_Basement                | `TRIGGER._ICOMSHP_BASEMENT`                | Store.dat                                                                                    |
| 2249 | ifunhous_CtrlRoom               | `TRIGGER._IFUNHOUS_CTRLROOM`               | ifunhous.dat                                                                                 |
| 2250 | ifunhous_CtrlRoomCtrl           | `TRIGGER._IFUNHOUS_CTRLROOMCTRL`           | ifunhous.dat                                                                                 |
| 2251 | ifunhous_EndMine                | `TRIGGER._IFUNHOUS_ENDMINE`                | ifunhous.dat                                                                                 |
| 2252 | ifunhous_FLbBook                | `TRIGGER._IFUNHOUS_FLBBOOK`                | ifunhous.dat                                                                                 |
| 2253 | ifunhous_FLbLader               | `TRIGGER._IFUNHOUS_FLBLADER`               | ifunhous.dat                                                                                 |
| 2254 | ifunhous_FMTrapDr00L            | `TRIGGER._IFUNHOUS_FMTRAPDR00L`            | ifunhous.dat                                                                                 |
| 2255 | ifunhous_FMTrapDr00O            | `TRIGGER._IFUNHOUS_FMTRAPDR00O`            | ifunhous.dat                                                                                 |
| 2256 | ifunhous_FMTrapDr01L            | `TRIGGER._IFUNHOUS_FMTRAPDR01L`            | ifunhous.dat                                                                                 |
| 2257 | ifunhous_FMTrapDr01O            | `TRIGGER._IFUNHOUS_FMTRAPDR01O`            | ifunhous.dat                                                                                 |
| 2258 | ifunhous_FMTrapDr02L            | `TRIGGER._IFUNHOUS_FMTRAPDR02L`            | ifunhous.dat                                                                                 |
| 2259 | ifunhous_FMTrapDr02O            | `TRIGGER._IFUNHOUS_FMTRAPDR02O`            | ifunhous.dat                                                                                 |
| 2260 | ifunhous_FMTrapDr03L            | `TRIGGER._IFUNHOUS_FMTRAPDR03L`            | ifunhous.dat                                                                                 |
| 2261 | ifunhous_FMTrapDr03O            | `TRIGGER._IFUNHOUS_FMTRAPDR03O`            | ifunhous.dat                                                                                 |
| 2262 | ifunhous_FMTrapSw               | `TRIGGER._IFUNHOUS_FMTRAPSW`               | ifunhous.dat                                                                                 |
| 2263 | ifunhous_FMTrapSw01             | `TRIGGER._IFUNHOUS_FMTRAPSW01`             | ifunhous.dat                                                                                 |
| 2264 | ifunhous_FMTrapSw01b            | `TRIGGER._IFUNHOUS_FMTRAPSW01B`            | ifunhous.dat                                                                                 |
| 2265 | ifunhous_FMTrapSw02             | `TRIGGER._IFUNHOUS_FMTRAPSW02`             | ifunhous.dat                                                                                 |
| 2266 | ifunhous_FMTrapSw02b            | `TRIGGER._IFUNHOUS_FMTRAPSW02B`            | ifunhous.dat                                                                                 |
| 2267 | ifunhous_FMTrapSw03             | `TRIGGER._IFUNHOUS_FMTRAPSW03`             | ifunhous.dat                                                                                 |
| 2268 | ifunhous_FMTrapSw03b            | `TRIGGER._IFUNHOUS_FMTRAPSW03B`            | ifunhous.dat                                                                                 |
| 2269 | ifunhous_FMTrapSw04             | `TRIGGER._IFUNHOUS_FMTRAPSW04`             | ifunhous.dat                                                                                 |
| 2270 | ifunhous_FMTrapSw04b            | `TRIGGER._IFUNHOUS_FMTRAPSW04B`            | ifunhous.dat                                                                                 |
| 2271 | ifunhous_FMTrapSw05             | `TRIGGER._IFUNHOUS_FMTRAPSW05`             | ifunhous.dat                                                                                 |
| 2272 | ifunhous_FMTrapSw05b            | `TRIGGER._IFUNHOUS_FMTRAPSW05B`            | ifunhous.dat                                                                                 |
| 2273 | ifunhous_FMTrapSw06             | `TRIGGER._IFUNHOUS_FMTRAPSW06`             | ifunhous.dat                                                                                 |
| 2274 | ifunhous_FMTrapSw06b            | `TRIGGER._IFUNHOUS_FMTRAPSW06B`            | ifunhous.dat                                                                                 |
| 2275 | ifunhous_FMTrapSw07             | `TRIGGER._IFUNHOUS_FMTRAPSW07`             | ifunhous.dat                                                                                 |
| 2276 | ifunhous_FMTrapSw07b            | `TRIGGER._IFUNHOUS_FMTRAPSW07B`            | ifunhous.dat                                                                                 |
| 2277 | ifunhous_FMTrapSwb              | `TRIGGER._IFUNHOUS_FMTRAPSWB`              | ifunhous.dat                                                                                 |
| 2278 | ifunhous_MineEnd                | `TRIGGER._IFUNHOUS_MINEEND`                | ifunhous.dat                                                                                 |
| 2279 | ifunhous_MineMze                | `TRIGGER._IFUNHOUS_MINEMZE`                | ifunhous.dat                                                                                 |
| 2280 | ifunhous_MzeMine                | `TRIGGER._IFUNHOUS_MZEMINE`                | ifunhous.dat                                                                                 |
| 2281 | ifunhous_Reeper00               | `TRIGGER._IFUNHOUS_REEPER00`               | ifunhous.dat                                                                                 |
| 2282 | ifunhous_Reeper00b              | `TRIGGER._IFUNHOUS_REEPER00B`              | ifunhous.dat                                                                                 |
| 2283 | ifunhous_Reeper01               | `TRIGGER._IFUNHOUS_REEPER01`               | ifunhous.dat                                                                                 |
| 2284 | ifunhous_Reeper01b              | `TRIGGER._IFUNHOUS_REEPER01B`              | ifunhous.dat                                                                                 |
| 2285 | ifunhous_Reeper02               | `TRIGGER._IFUNHOUS_REEPER02`               | ifunhous.dat                                                                                 |
| 2286 | ifunhous_Reeper02b              | `TRIGGER._IFUNHOUS_REEPER02B`              | ifunhous.dat                                                                                 |
| 2287 | ifunhous_funMinerB              | `TRIGGER._IFUNHOUS_FUNMINERB`              | ifunhous.dat                                                                                 |
| 2288 | ifunhous_funMinerD              | `TRIGGER._IFUNHOUS_FUNMINERD`              | ifunhous.dat                                                                                 |
| 2289 | ifunhous_funMinerG              | `TRIGGER._IFUNHOUS_FUNMINERG`              | ifunhous.dat                                                                                 |
| 2290 | ifunhous_funMinerH              | `TRIGGER._IFUNHOUS_FUNMINERH`              | ifunhous.dat                                                                                 |
| 2291 | ifunhous_funMinerI              | `TRIGGER._IFUNHOUS_FUNMINERI`              | ifunhous.dat                                                                                 |
| 2292 | ifunhous_funMinerX1             | `TRIGGER._IFUNHOUS_FUNMINERX1`             | ifunhous.dat                                                                                 |
| 2293 | ifunhous_funMinerX2             | `TRIGGER._IFUNHOUS_FUNMINERX2`             | ifunhous.dat                                                                                 |
| 2294 | ifunhous_funMinerX3             | `TRIGGER._IFUNHOUS_FUNMINERX3`             | ifunhous.dat                                                                                 |
| 2295 | ifunhous_funMinerX4             | `TRIGGER._IFUNHOUS_FUNMINERX4`             | ifunhous.dat                                                                                 |
| 2296 | ischool_CafDoor2R               | `TRIGGER._ISCHOOL_CAFDOOR2R`               | ischool_doors.dat                                                                            |
| 2297 | ischool_Door00                  | `TRIGGER._ISCHOOL_DOOR00`                  | ischool_doors.dat                                                                            |
| 2298 | ischool_Door02                  | `TRIGGER._ISCHOOL_DOOR02`                  | ischool_doors.dat                                                                            |
| 2299 | ischool_Door05                  | `TRIGGER._ISCHOOL_DOOR05`                  | ischool_doors.dat                                                                            |
| 2300 | ischool_Door06                  | `TRIGGER._ISCHOOL_DOOR06`                  | ischool_doors.dat                                                                            |
| 2301 | ischool_Door09                  | `TRIGGER._ISCHOOL_DOOR09`                  | ischool_doors.dat                                                                            |
| 2302 | ischool_Door19                  | `TRIGGER._ISCHOOL_DOOR19`                  | ischool_doors.dat                                                                            |
| 2303 | ischool_Door21                  | `TRIGGER._ISCHOOL_DOOR21`                  | ischool_doors.dat                                                                            |
| 2304 | ischool_Door23                  | `TRIGGER._ISCHOOL_DOOR23`                  | ischool_doors.dat                                                                            |
| 2305 | ischool_Door24                  | `TRIGGER._ISCHOOL_DOOR24`                  | ischool_doors.dat                                                                            |
| 2306 | ischool_Door25                  | `TRIGGER._ISCHOOL_DOOR25`                  | ischool_doors.dat                                                                            |
| 2307 | ischool_Door28                  | `TRIGGER._ISCHOOL_DOOR28`                  | ischool_doors.dat                                                                            |
| 2308 | ischool_Door30                  | `TRIGGER._ISCHOOL_DOOR30`                  | ischool_doors.dat                                                                            |
| 2309 | ischool_FrontDoorR              | `TRIGGER._ISCHOOL_FRONTDOORR`              | ischool_doors.dat                                                                            |
| 2310 | ischool_StoreArea               | `TRIGGER._ISCHOOL_STOREAREA`               | ischool_doors.dat                                                                            |
| 2311 | ischool_StoreDoor               | `TRIGGER._ISCHOOL_STOREDOOR`               | ischool_doors.dat                                                                            |
| 2312 | ischool_fountains_SCFount       | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT`       | ischool_fountains.dat                                                                        |
| 2313 | ischool_fountains_SCFount03     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT03`     | ischool_fountains.dat                                                                        |
| 2314 | ischool_fountains_SCFount04     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT04`     | ischool_fountains.dat                                                                        |
| 2315 | ischool_fountains_SCFount05     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT05`     | ischool_fountains.dat                                                                        |
| 2316 | ischool_fountains_SCFount06     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT06`     | ischool_fountains.dat                                                                        |
| 2317 | ischool_fountains_SCFount09     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT09`     | ischool_fountains.dat                                                                        |
| 2318 | ischool_fountains_SCFount12     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT12`     | ischool_fountains.dat                                                                        |
| 2319 | ischool_fountains_SCFount15     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT15`     | ischool_fountains.dat                                                                        |
| 2320 | ischool_fountains_SCFount16     | `TRIGGER._ISCHOOL_FOUNTAINS_SCFOUNT16`     | ischool_fountains.dat                                                                        |
| 2321 | isclib_Globe                    | `TRIGGER._ISCLIB_GLOBE`                    | isc_lib.dat                                                                                  |
| 2322 | lvl1GameArea                    | `TRIGGER._LVL1GAMEAREA`                    | P_Snow1.dat                                                                                  |
| 2323 | lvl2GameArea                    | `TRIGGER._LVL2GAMEAREA`                    | P_Snow2.dat                                                                                  |
| 2324 | lvl3GameArea                    | `TRIGGER._LVL3GAMEAREA`                    | P_Snow3.dat                                                                                  |
| 2325 | lvl4GameArea                    | `TRIGGER._LVL4GAMEAREA`                    | P_Snow4.dat                                                                                  |
| 2326 | lvl5GameArea                    | `TRIGGER._LVL5GAMEAREA`                    | P_Snow5.dat                                                                                  |
| 2327 | lvl5_gate                       | `TRIGGER._LVL5_GATE`                       | P_Snow5.dat                                                                                  |
| 2328 | lvl5_snowPile03                 | `TRIGGER._LVL5_SNOWPILE03`                 | P_Snow5.dat                                                                                  |
| 2329 | lvl5_snowPile06                 | `TRIGGER._LVL5_SNOWPILE06`                 | P_Snow5.dat                                                                                  |
| 2330 | lvl5_snowPile07                 | `TRIGGER._LVL5_SNOWPILE07`                 | P_Snow5.dat                                                                                  |
| 2331 | lvl5_snowPile08                 | `TRIGGER._LVL5_SNOWPILE08`                 | P_Snow5.dat                                                                                  |
| 2332 | lvl5_snowPile09                 | `TRIGGER._LVL5_SNOWPILE09`                 | P_Snow5.dat                                                                                  |
| 2333 | lvl5_snowPile10                 | `TRIGGER._LVL5_SNOWPILE10`                 | P_Snow5.dat                                                                                  |
| 2334 | lvl6GameArea                    | `TRIGGER._LVL6GAMEAREA`                    | P_Snow6.dat                                                                                  |
| 2335 | lvl6_snowPile_04                | `TRIGGER._LVL6_SNOWPILE_04`                | P_Snow6.dat                                                                                  |
| 2336 | lvl6_snowPile_05                | `TRIGGER._LVL6_SNOWPILE_05`                | P_Snow6.dat                                                                                  |
| 2337 | lvl6_snowPile_06                | `TRIGGER._LVL6_SNOWPILE_06`                | P_Snow6.dat                                                                                  |
| 2338 | lvl6_snowPile_07                | `TRIGGER._LVL6_SNOWPILE_07`                | P_Snow6.dat                                                                                  |
| 2339 | lvl6_snowPile_08                | `TRIGGER._LVL6_SNOWPILE_08`                | P_Snow6.dat                                                                                  |
| 2340 | lvl6_snowPile_09                | `TRIGGER._LVL6_SNOWPILE_09`                | P_Snow6.dat                                                                                  |
| 2341 | lvl6_snowPile_10                | `TRIGGER._LVL6_SNOWPILE_10`                | P_Snow6.dat                                                                                  |
| 2342 | lvl6_snowPile_12                | `TRIGGER._LVL6_SNOWPILE_12`                | P_Snow6.dat                                                                                  |
| 2343 | lvl6_snowPile_14                | `TRIGGER._LVL6_SNOWPILE_14`                | P_Snow6.dat                                                                                  |
| 2344 | observatory_doorR               | `TRIGGER._OBSERVATORY_DOORR`               | eventsObservatory.dat                                                                        |
| 2345 | pChair                          | `TRIGGER._PCHAIR`                          | ttest.dat                                                                                    |
| 2346 | pa_GameArea                     | `TRIGGER._PA_GAMEAREA`                     | GarbPickPoor.dat                                                                             |
| 2347 | pa_Hobo1Area                    | `TRIGGER._PA_HOBO1AREA`                    | GarbPickPoor.dat                                                                             |
| 2348 | pa_Hobo2Area                    | `TRIGGER._PA_HOBO2AREA`                    | GarbPickPoor.dat                                                                             |
| 2349 | pa_Hobo3Area                    | `TRIGGER._PA_HOBO3AREA`                    | GarbPickPoor.dat                                                                             |
| 2350 | pa_TrashArea                    | `TRIGGER._PA_TRASHAREA`                    | GarbPickPoor.dat                                                                             |
| 2351 | plat_North                      | `TRIGGER._PLAT_NORTH`                      | 4_B1.dat                                                                                     |
| 2352 | plat_South                      | `TRIGGER._PLAT_SOUTH`                      | 4_B1.dat                                                                                     |
| 2353 | plat_West                       | `TRIGGER._PLAT_WEST`                       | 4_B1.dat                                                                                     |
| 2354 | platform_South                  | `TRIGGER._PLATFORM_SOUTH`                  | 4_B1.dat                                                                                     |
| 2355 | platform_West                   | `TRIGGER._PLATFORM_WEST`                   | 4_B1.dat                                                                                     |
| 2356 | pool_boyslocker                 | `TRIGGER._POOL_BOYSLOCKER`                 | eventsGymAndPool.dat                                                                         |
| 2357 | pool_doorR                      | `TRIGGER._POOL_DOORR`                      | eventsGymAndPool.dat                                                                         |
| 2358 | pool_girlslocker                | `TRIGGER._POOL_GIRLSLOCKER`                | eventsGymAndPool.dat                                                                         |
| 2359 | smallTag                        | `TRIGGER._SMALLTAG`                        | GraffitiTest.dat                                                                             |
| 2360 | snowPile1_01                    | `TRIGGER._SNOWPILE1_01`                    | P_Snow1.dat                                                                                  |
| 2361 | snowPile1_02                    | `TRIGGER._SNOWPILE1_02`                    | P_Snow1.dat                                                                                  |
| 2362 | snowPile1_03                    | `TRIGGER._SNOWPILE1_03`                    | P_Snow1.dat                                                                                  |
| 2363 | snowPile1_04                    | `TRIGGER._SNOWPILE1_04`                    | P_Snow1.dat                                                                                  |
| 2364 | snowPile2_01                    | `TRIGGER._SNOWPILE2_01`                    | P_Snow2.dat                                                                                  |
| 2365 | snowPile2_02                    | `TRIGGER._SNOWPILE2_02`                    | P_Snow2.dat                                                                                  |
| 2366 | snowPile2_03                    | `TRIGGER._SNOWPILE2_03`                    | P_Snow2.dat                                                                                  |
| 2367 | snowPile2_04                    | `TRIGGER._SNOWPILE2_04`                    | P_Snow2.dat                                                                                  |
| 2368 | snowPile2_05                    | `TRIGGER._SNOWPILE2_05`                    | P_Snow2.dat                                                                                  |
| 2369 | snowPile2_06                    | `TRIGGER._SNOWPILE2_06`                    | P_Snow2.dat                                                                                  |
| 2370 | snowPile3_01                    | `TRIGGER._SNOWPILE3_01`                    | P_Snow3.dat                                                                                  |
| 2371 | snowPile3_02                    | `TRIGGER._SNOWPILE3_02`                    | P_Snow3.dat                                                                                  |
| 2372 | snowPile3_03                    | `TRIGGER._SNOWPILE3_03`                    | P_Snow3.dat                                                                                  |
| 2373 | snowPile3_04                    | `TRIGGER._SNOWPILE3_04`                    | P_Snow3.dat                                                                                  |
| 2374 | snowPile3_05                    | `TRIGGER._SNOWPILE3_05`                    | P_Snow3.dat                                                                                  |
| 2375 | snowPile3_06                    | `TRIGGER._SNOWPILE3_06`                    | P_Snow3.dat                                                                                  |
| 2376 | snowPile3_07                    | `TRIGGER._SNOWPILE3_07`                    | P_Snow3.dat                                                                                  |
| 2377 | snowPile3_08                    | `TRIGGER._SNOWPILE3_08`                    | P_Snow3.dat                                                                                  |
| 2378 | snowStage4_01                   | `TRIGGER._SNOWSTAGE4_01`                   | P_Snow4.dat                                                                                  |
| 2379 | snowStage4_02                   | `TRIGGER._SNOWSTAGE4_02`                   | P_Snow4.dat                                                                                  |
| 2380 | snowStage4_04                   | `TRIGGER._SNOWSTAGE4_04`                   | P_Snow4.dat                                                                                  |
| 2381 | snowStage4_05                   | `TRIGGER._SNOWSTAGE4_05`                   | P_Snow4.dat                                                                                  |
| 2382 | tag1                            | `TRIGGER._TAG1`                            | GraffitiTest.dat                                                                             |
| 2383 | tbarrels_Sbarels1               | `TRIGGER._TBARRELS_SBARELS1`               | tbarrels.dat                                                                                 |
| 2384 | tbusiness_BMXGate               | `TRIGGER._TBUSINESS_BMXGATE`               | tbusines_BMXGate.dat                                                                         |
| 2385 | tbusiness_GarbCanA08            | `TRIGGER._TBUSINESS_GARBCANA08`            | tbusines.dat                                                                                 |
| 2386 | tbusiness_MotelDor              | `TRIGGER._TBUSINESS_MOTELDOR`              | tbusines.dat                                                                                 |
| 2387 | testSafeCut_startCut            | `TRIGGER._TESTSAFECUT_STARTCUT`            | testSafeCut.dat                                                                              |
| 2388 | tmrf_ratBoundary                | `TRIGGER._TMRF_RATBOUNDARY`                | testMandyRatFlee.dat                                                                         |
| 2389 | trich_SprinklerSwitch           | `TRIGGER._TRICH_SPRINKLERSWITCH`           | PAn_Main.dat                                                                                 |
| 2390 | trich_TadGates                  | `TRIGGER._TRICH_TADGATES`                  | trich.dat                                                                                    |
| 2391 | trich_TadGates01                | `TRIGGER._TRICH_TADGATES01`                | trich.dat                                                                                    |
| 2392 | triggerBackAlley                | `TRIGGER._TRIGGERBACKALLEY`                | 3_03.dat                                                                                     |
| 2393 | triggerBalcony                  | `TRIGGER._TRIGGERBALCONY`                  | 3_03.dat                                                                                     |
| 2394 | triggerBalcony2                 | `TRIGGER._TRIGGERBALCONY2`                 | 3_03.dat                                                                                     |
| 2395 | triggerLola                     | `TRIGGER._TRIGGERLOLA`                     | 3_03.dat                                                                                     |
| 2396 | triggerTadTether                | `TRIGGER._TRIGGERTADTETHER`                | 3_03.dat                                                                                     |
| 2397 | tschool_AutoShopFGate           | `TRIGGER._TSCHOOL_AUTOSHOPFGATE`           | 1_03.dat                                                                                     |
| 2398 | tschool_BoysDormR               | `TRIGGER._TSCHOOL_BOYSDORMR`               | tschool_doors.dat                                                                            |
| 2399 | tschool_FieldR                  | `TRIGGER._TSCHOOL_FIELDR`                  | tschool_doors.dat                                                                            |
| 2400 | tschool_FrontGate               | `TRIGGER._TSCHOOL_FRONTGATE`               | 1_01.dat, 6_02.dat, Chapt1Trans.dat                                                          |
| 2401 | tschool_GirlsDormR              | `TRIGGER._TSCHOOL_GIRLSDORMR`              | tschool_doors.dat                                                                            |
| 2402 | tschool_GymR                    | `TRIGGER._TSCHOOL_GYMR`                    | tschool_doors.dat                                                                            |
| 2403 | tschool_LibraryR                | `TRIGGER._TSCHOOL_LIBRARYR`                | tschool_doors.dat                                                                            |
| 2404 | tschool_ParkingGate             | `TRIGGER._TSCHOOL_PARKINGGATE`             | 6_02.dat, Chapt1Trans.dat                                                                    |
| 2405 | tschool_PoolR                   | `TRIGGER._TSCHOOL_POOLR`                   | tschool_doors.dat                                                                            |
| 2406 | tschool_PreppyR                 | `TRIGGER._TSCHOOL_PREPPYR`                 | tschool_doors.dat                                                                            |
| 2407 | tschool_SchoolFrontDoorR        | `TRIGGER._TSCHOOL_SCHOOLFRONTDOORR`        | tschool_doors.dat                                                                            |
| 2408 | tschool_SchoolLeftFrontDoor     | `TRIGGER._TSCHOOL_SCHOOLLEFTFRONTDOOR`     | tschool_doors.dat                                                                            |
| 2409 | turret_top                      | `TRIGGER._TURRET_TOP`                      | 4_B1.dat                                                                                     |
| 2410 | tutorialTag                     | `TRIGGER._TUTORIALTAG`                     | GraffitiTest.dat                                                                             |
| 2411 | valeHotelDoor                   | `TRIGGER._VALEHOTELDOOR`                   | trich_doors.dat                                                                              |

---

## Trigger Types Overview

|    # | Trigger Key                     | Type                              |
| ---: | ------------------------------- | --------------------------------- |
|    1 | 1_01_BullyTrig                  | Box                               |
|    2 | 1_01_CHECKOBJS1                 | Box                               |
|    3 | 1_01_FightTrigger               | Box                               |
|    4 | 1_01_ParkDoor                   | Box                               |
|    5 | 1_01_PrincOffice                | Box                               |
|    6 | 1_01_SchoolTrig                 | Box                               |
|    7 | 1_02B_bathroom                  | Box                               |
|    8 | 1_02B_cafeMessage               | Box                               |
|    9 | 1_02B_constTether               | Box                               |
|   10 | 1_02B_disablePOI                | Box                               |
|   11 | 1_02B_euniceKiss                | Box                               |
|   12 | 1_02B_excluderLocker            | Box                               |
|   13 | 1_02B_lockerMessage             | Box                               |
|   14 | 1_02B_lockerMessage02           | Box                               |
|   15 | 1_02B_objCafe                   | Box                               |
|   16 | 1_02B_objLocker                 | Box                               |
|   17 | 1_02B_objSocial                 | Box                               |
|   18 | 1_02B_recruitGary               | Box                               |
|   19 | 1_02B_socialMessage             | Box                               |
|   20 | 1_02B_warn01                    | Box                               |
|   21 | 1_02B_warn02                    | Box                               |
|   22 | 1_02B_warn03                    | Box                               |
|   23 | 1_02B_warn04                    | Box                               |
|   24 | 1_02_FightArea                  | Box                               |
|   25 | 1_02_PopulationTrig             | PopulationPed                     |
|   26 | 1_02_RusselTease                | Box                               |
|   27 | 1_02_SchoolTrig                 | Box                               |
|   28 | 1_02_TrainArea                  | Box                               |
|   29 | 1_03_AutoShopArea               | PopulationPed                     |
|   30 | 1_03_DavisRegisterHit           | Box                               |
|   31 | 1_03_DavisRun                   | Box                               |
|   32 | 1_03_FailTrigger01              | Box                               |
|   33 | 1_03_FailTrigger02              | Box                               |
|   34 | 1_03_FalTrigger04               | Box                               |
|   35 | 1_03_Fight1                     | Box                               |
|   36 | 1_03_Fight3                     | Box                               |
|   37 | 1_03_Fight4                     | Box                               |
|   38 | 1_03_Fight5                     | Box                               |
|   39 | 1_03_FrontGate                  | Box                               |
|   40 | 1_03_GameArea                   | Box                               |
|   41 | 1_03_Garage02                   | Box                               |
|   42 | 1_03_Garage03                   | Box                               |
|   43 | 1_03_GarbageCan02               | Box                               |
|   44 | 1_03_GarbageCan05               | Box                               |
|   45 | 1_03_GarbageCan06               | Box                               |
|   46 | 1_03_GarbageCan07               | Box                               |
|   47 | 1_03_JumpTut01                  | Box                               |
|   48 | 1_03_KeepPedTrigger             | Box                               |
|   49 | 1_03_Ladder_Drop                | Box                               |
|   50 | 1_03_PeterTrigger               | Box                               |
|   51 | 1_03_SchoolYard                 | Box                               |
|   52 | 1_03_barelLad                   | Door                              |
|   53 | 1_04_BottleNIS                  | Box                               |
|   54 | 1_04_BottleShootArea            | Box                               |
|   55 | 1_04_BottleZone                 | Box                               |
|   56 | 1_04_FieldTrig                  | Box                               |
|   57 | 1_04_NemSitDown                 | Box                               |
|   58 | 1_04_Parking                    | Box                               |
|   59 | 1_04_Soda_Nerd                  | Box                               |
|   60 | 1_04_SuppressFieldPop           | PopulationPed                     |
|   61 | 1_04_SuppressParkingPop         | PopulationPed                     |
|   62 | 1_04_tree1_trig                 | Box                               |
|   63 | 1_04_tree2_trig                 | Box                               |
|   64 | 1_04_tree_sit                   | Box                               |
|   65 | 1_05B_algieLocker               | Box                               |
|   66 | 1_05B_algieStall                | Box                               |
|   67 | 1_05B_areaSecondFloorBR         | Box                               |
|   68 | 1_05B_bathroomFirstFloor        | Box                               |
|   69 | 1_05B_bathroomSecondFloor       | Box                               |
|   70 | 1_05B_firstFloorAmbientOff      | Box                               |
|   71 | 1_05B_firstFloorAmbientOn       | Box                               |
|   72 | 1_05B_firstFloorGirlsBR         | Box                               |
|   73 | 1_05B_loadSmoke                 | Box                               |
|   74 | 1_05B_secondFloorGirlsBR        | Box                               |
|   75 | 1_05_backDoorOff                | Box                               |
|   76 | 1_05_frontDoorOff               | Box                               |
|   77 | 1_05_triggerJockPack            | Box                               |
|   78 | 1_05_triggerJockPackWarning     | Box                               |
|   79 | 1_05_triggerJocksNearFront      | Box                               |
|   80 | 1_05_triggerJocksNearLibrary    | Box                               |
|   81 | 1_07_BUCKY_BOUND                | Box                               |
|   82 | 1_07_FightTrigger               | Box                               |
|   83 | 1_07_GateTrig                   | Box                               |
|   84 | 1_07_Gate_T                     | Door                              |
|   85 | 1_07_Library_Door               | Box                               |
|   86 | 1_07_NEAR_PARKING_LOT           | Box                               |
|   87 | 1_07_NoAmbientPeds              | Box                               |
|   88 | 1_07_SpawnZone                  | Box                               |
|   89 | 1_07_Spawner01                  | Box                               |
|   90 | 1_07_Spawner02                  | Box                               |
|   91 | 1_07_Spawner03                  | Box                               |
|   92 | 1_07_Spawner04                  | Box                               |
|   93 | 1_07_Spawner05                  | Box                               |
|   94 | 1_07_Spawner06                  | Box                               |
|   95 | 1_07_ToolBox01                  | Box                               |
|   96 | 1_08_BathroomLocker             | Box                               |
|   97 | 1_08_CafTrig                    | Box                               |
|   98 | 1_08_GYMGIRLWASH                | Box                               |
|   99 | 1_08_JimmyLeft                  | Box                               |
|  100 | 1_09_AisleLeft                  | Box                               |
|  101 | 1_09_AisleRight                 | Box                               |
|  102 | 1_09_BoxLeft1                   | Box                               |
|  103 | 1_09_BoxLeft2                   | Box                               |
|  104 | 1_09_BoxRight1                  | Box                               |
|  105 | 1_09_BoxRight2                  | Box                               |
|  106 | 1_09_Catwalk1                   | Box                               |
|  107 | 1_09_StageLeft                  | Box                               |
|  108 | 1_09_StageRight                 | Box                               |
|  109 | 1_10_BasementDoor               | Box                               |
|  110 | 1_10_BullyTrigger               | Box                               |
|  111 | 1_10_CrouchHint                 | Box                               |
|  112 | 1_10_GARY_TURN_OFF_ELEC         | Box                               |
|  113 | 1_10_InCage                     | Box                               |
|  114 | 1_10_NearHole                   | Box                               |
|  115 | 1_10_Near_BasementDoor          | Box                               |
|  116 | 1_10_TheHole                    | Box                               |
|  117 | 1_10_almost_complete            | Box                               |
|  118 | 1_10_atFurnace                  | Box                               |
|  119 | 1_10_aud_2                      | Box                               |
|  120 | 1_10_crawl_elec                 | Box                               |
|  121 | 1_10_exit_cage                  | Box                               |
|  122 | 1_10_ring_peds                  | Box                               |
|  123 | 1_10_room0                      | Box                               |
|  124 | 1_10_room1                      | Box                               |
|  125 | 1_10_room2                      | Box                               |
|  126 | 1_10_room3                      | Box                               |
|  127 | 1_10_room4                      | Box                               |
|  128 | 1_11X1_bullies                  | Box                               |
|  129 | 1_11X1_outside                  | Box                               |
|  130 | 1_11X1_pete                     | Box                               |
|  131 | 1_11x2_chadAttack               | Box                               |
|  132 | 1_11x2_garden                   | Box                               |
|  133 | 1_11x2_shitTarget               | Box                               |
|  134 | 1_11xp_DeadRat                  | Box                               |
|  135 | 1_11xp_F4000                    | Box                               |
|  136 | 1_11xp_Firecracker              | Box                               |
|  137 | 1_11xp_ItchPowder               | Box                               |
|  138 | 1_11xp_JokeCandy                | Box                               |
|  139 | 1_11xp_KickMe                   | Box                               |
|  140 | 1_11xp_Marbles                  | Box                               |
|  141 | 1_11xp_StinkBomb                | Box                               |
|  142 | 1_G1_BeatriceWarning            | Box                               |
|  143 | 1_G1_MathProxy                  | Box                               |
|  144 | 1_G1_StaffProxy                 | Box                               |
|  145 | 1_S01_Bathroom                  | Box                               |
|  146 | 1_S01_BathroomSetup             | Box                               |
|  147 | 1_S01_Bottle_Trig_Bath          | Box                               |
|  148 | 1_S01_Bottle_Trig_Cafe          | Box                               |
|  149 | 1_S01_Bottle_Trig_Case          | Box                               |
|  150 | 1_S01_Cafe                      | Box                               |
|  151 | 1_S01_Create_Edna               | Box                               |
|  152 | 1_S01_Glass                     | Box                               |
|  153 | 1_S01_HattrickDelete            | Box                               |
|  154 | 1_S01_Kitchen                   | Box                               |
|  155 | 1_S01_Phillips_Return           | Box                               |
|  156 | 1_S01_PlayerBlocking            | Box                               |
|  157 | 1_S01_Prefect1                  | Box                               |
|  158 | 1_S01_Prefect_8_1_Spawn         | Box                               |
|  159 | 1_S01_Prefect_Running1          | Box                               |
|  160 | 1_S01_Prefect_Running1_Delete   | Box                               |
|  161 | 1_S01_TrophySetup               | Box                               |
|  162 | 1_g1_Locker                     | Box                               |
|  163 | 2_01_EdnaFacePlayer             | Box                               |
|  164 | 2_01_GreaserTrig                | Box                               |
|  165 | 2_01_GreaserTrig2               | Box                               |
|  166 | 2_01_MOUNTBIKE                  | Box                               |
|  167 | 2_01_PreppyTrig                 | Box                               |
|  168 | 2_01_PreppyTrig2                | Box                               |
|  169 | 2_01_StartCopfight              | Box                               |
|  170 | 2_01_TutPlay1                   | Box                               |
|  171 | 2_01_tutOff                     | Box                               |
|  172 | 2_01_tutOff2                    | Box                               |
|  173 | 2_02_returnComic                | Box                               |
|  174 | 2_02_schoolParking              | Box                               |
|  175 | 2_03_BRTadTrigger               | Box                               |
|  176 | 2_03_Back_Gate                  | Box                               |
|  177 | 2_03_Back_Unlock                | Box                               |
|  178 | 2_03_Backyard                   | Box                               |
|  179 | 2_03_FrontDoorTrigger           | Box                               |
|  180 | 2_03_FrontGateArea              | Box                               |
|  181 | 2_03_FrontYard                  | Box                               |
|  182 | 2_03_Front_Unlock               | Box                               |
|  183 | 2_03_RearDoorTrigger            | Box                               |
|  184 | 2_03_RearGateArea               | Box                               |
|  185 | 2_03_TadHouse                   | Box                               |
|  186 | 2_03_TadNIS                     | Box                               |
|  187 | 2_03_TadsBlock                  | Box                               |
|  188 | 2_04_BarrelFire01               | Box                               |
|  189 | 2_04_BarrelFire02               | Box                               |
|  190 | 2_04_BarrelFire03               | Box                               |
|  191 | 2_04_BarrelFire04               | Box                               |
|  192 | 2_04_BarrelFire05               | Box                               |
|  193 | 2_04_BarrelFire06               | Box                               |
|  194 | 2_04_CHEATER_1_ZONE             | Box                               |
|  195 | 2_04_CHEATER_2_ZONE             | Box                               |
|  196 | 2_04_CHEATER_3_ZONE             | Box                               |
|  197 | 2_04_CHEATER_4_ZONE             | Box                               |
|  198 | 2_04_ChangeBeach                | Box                               |
|  199 | 2_04_DormDoor                   | Box                               |
|  200 | 2_04_TireFire01b                | Box                               |
|  201 | 2_04_TireFire02b                | Box                               |
|  202 | 2_04_TireFire03b                | Box                               |
|  203 | 2_05_BACKGATE                   | Box                               |
|  204 | 2_05_EggStashArea               | Box                               |
|  205 | 2_05_FRONTGATE                  | Box                               |
|  206 | 2_05_FrontExit                  | Box                               |
|  207 | 2_05_RecruitRussell             | Box                               |
|  208 | 2_05_RichArea                   | Box                               |
|  209 | 2_05_Room1                      | Box                               |
|  210 | 2_05_Room2                      | Box                               |
|  211 | 2_05_Room3                      | Box                               |
|  212 | 2_05_Room4                      | Box                               |
|  213 | 2_05_Room5                      | Box                               |
|  214 | 2_05_Room6                      | Box                               |
|  215 | 2_05_RussellOffBike             | Box                               |
|  216 | 2_05_TadsBlock                  | Box                               |
|  217 | 2_05_TadsYard                   | Box                               |
|  218 | 2_05_Tree01                     | Box                               |
|  219 | 2_05_Tree02                     | Box                               |
|  220 | 2_05_WallBreak01                | Box                               |
|  221 | 2_05_WallBreak02                | Box                               |
|  222 | 2_06_BikeZone                   | Box                               |
|  223 | 2_06_Theater                    | Box                               |
|  224 | 2_07_GORD_ON_DOCK               | Box                               |
|  225 | 2_07_OUTSIDEDOOR                | Box                               |
|  226 | 2_07_OUT_OF_AREA                | Box                               |
|  227 | 2_07_OUT_OF_AREA_WARN           | Box                               |
|  228 | 2_07_PREPPY_NINJA_TRIG          | Box                               |
|  229 | 2_07_REAR_PIER                  | Box                               |
|  230 | 2_07_behindDoor                 | Box                               |
|  231 | 2_08_BifAttackTrig              | Box                               |
|  232 | 2_08_DoorStairs                 | Box                               |
|  233 | 2_08_FirstFloorTrig             | Box                               |
|  234 | 2_08_FoyeurDoor                 | Box                               |
|  235 | 2_08_PlantTarget                | Box                               |
|  236 | 2_08_SecndFloorTrig             | Box                               |
|  237 | 2_08_SolariumEntrance           | Box                               |
|  238 | 2_08_StairPreppy                | Box                               |
|  239 | 2_08_ThrdFloorTrig              | Box                               |
|  240 | 2_08_ToSolarium                 | Box                               |
|  241 | 2_08_TriggerStairs              | Box                               |
|  242 | 2_B_BOSS_FIGHT                  | Box                               |
|  243 | 2_B_BOSS_FIGHT_INTRO            | Box                               |
|  244 | 2_B_DRBRACE_DOOR                | Box                               |
|  245 | 2_B_DRBRACE_DOOR01              | Box                               |
|  246 | 2_B_PLAYER_NEAR_BAR             | Box                               |
|  247 | 2_B_SECOND_ATTACK               | Box                               |
|  248 | 2_B_Tether                      | Box                               |
|  249 | 2_G2_ballToss                   | Box                               |
|  250 | 2_G2_ballTossExcluderInside     | Box                               |
|  251 | 2_G2_ballTossExcluderOutside    | Box                               |
|  252 | 2_G2_dunkExcluderOutside        | Box                               |
|  253 | 2_G2_dunkTank                   | Box                               |
|  254 | 2_G2_excluderCoaster            | Box                               |
|  255 | 2_G2_excluderFerris             | Box                               |
|  256 | 2_G2_excluderSquid              | Box                               |
|  257 | 2_G2_freakShow                  | Box                               |
|  258 | 2_G2_highStriker                | Box                               |
|  259 | 2_G2_pinkyAngryFail             | Box                               |
|  260 | 2_G2_pinkyArrived               | Box                               |
|  261 | 2_G2_shootingExcluderInside     | Box                               |
|  262 | 2_G2_shootingExcluderOutside    | Box                               |
|  263 | 2_G2_shootingGallery            | Box                               |
|  264 | 2_G2_ticketShop                 | Box                               |
|  265 | 2_S02CarSpeedup                 | Box                               |
|  266 | 2_S02_CarFailTrigger            | Box                               |
|  267 | 2_S02_CarInDriveway             | Box                               |
|  268 | 2_S02_CarInit                   | Box                               |
|  269 | 2_S02_CarTrigger                | Box                               |
|  270 | 2_S02_Cop1                      | Box                               |
|  271 | 2_S02_Cop_Car1_Stop             | Box                               |
|  272 | 2_S02_Cop_Car2_Stop             | Box                               |
|  273 | 2_S02_End_Trigger1              | Box                               |
|  274 | 2_S02_HATTRICKYARD              | Box                               |
|  275 | 2_S02_HattrickNIS               | Box                               |
|  276 | 2_S02_Intro_Failure             | Box                               |
|  277 | 2_S02_PathVolume                | Box                               |
|  278 | 2_S04Sheet3NIS                  | Box                               |
|  279 | 2_S04_AutoShopArea              | Box                               |
|  280 | 2_S04_LibraryJump               | Box                               |
|  281 | 2_S04_Nerd_Escape               | Box                               |
|  282 | 2_S04_SchoolPop                 | Box                               |
|  283 | 2_S04_Sheet1                    | Box                               |
|  284 | 2_S04_Sheet2                    | Box                               |
|  285 | 2_S04_Sheet3                    | Box                               |
|  286 | 2_S04_Sheet3Create              | Box                               |
|  287 | 2_S04_Sheet3Outer               | Box                               |
|  288 | 2_S04_Sheet4                    | Box                               |
|  289 | 2_S04_Sheet4Inner               | Box                               |
|  290 | 2_S04_Sheet5E1                  | Box                               |
|  291 | 2_S04_Sheet5E2                  | Box                               |
|  292 | 2_S04_Sheet5Start               | Box                               |
|  293 | 2_S04_StartSheet2               | Box                               |
|  294 | 2_S04_TetherBully               | Box                               |
|  295 | 2_S04_TrashCan                  | Box                               |
|  296 | 2_S05_AwfulHack                 | Box                               |
|  297 | 2_S05_DisturbRadius             | Box                               |
|  298 | 2_S05_DrugAlley                 | Box                               |
|  299 | 2_S05_Excluder                  | Box                               |
|  300 | 2_S05_Target                    | Box                               |
|  301 | 2_S05_TeacherArea               | Box                               |
|  302 | 2_S05_TeacherRadius             | Box                               |
|  303 | 2_S05_TrashCan1                 | Box                               |
|  304 | 2_S05_TrashCan2                 | Box                               |
|  305 | 2_S05_TrashCan3                 | Box                               |
|  306 | 2_S05_Tree                      | Box                               |
|  307 | 2_S05_Tree2                     | Box                               |
|  308 | 2_S06B_AngieChristyRoom         | Box                               |
|  309 | 2_S06B_EuniceFrontDoor          | Box                               |
|  310 | 2_S06B_MandyRoom                | Box                               |
|  311 | 2_S06B_atticEntry               | Box                               |
|  312 | 2_S06B_launchAsian              | Box                               |
|  313 | 2_S06B_makeGirlsStudy           | Box                               |
|  314 | 2_S06B_pinkyRoom                | Box                               |
|  315 | 2_S06B_showerWarn               | Box                               |
|  316 | 2_S06B_trigger01                | Box                               |
|  317 | 2_S06B_trigger02                | Box                               |
|  318 | 2_S06B_trigger03                | Box                               |
|  319 | 2_S06B_triggerShowerDialogue    | Box                               |
|  320 | 2_S06B_upstairsHallway          | Box                               |
|  321 | 2_S06_PrefectWander             | Box                               |
|  322 | 2_S06_latticeCam                | Box                               |
|  323 | 2_S06_mandySpeak                | Box                               |
|  324 | 2_S06_stg1Burton                | Box                               |
|  325 | 2_S06_stg1_Busted               | Box                               |
|  326 | 2_S06_stg3Burton                | Box                               |
|  327 | 2_S06_stg3LeftDorm              | Box                               |
|  328 | 2_S06_triggerLoadSchool         | Box                               |
|  329 | 2_S06_tutLattice                | Box                               |
|  330 | 306PoorArea                     | Box                               |
|  331 | 3B_CopsSpeedUp                  | Box                               |
|  332 | 3_01D_RUDY                      | Box                               |
|  333 | 3_01_KissFinal                  | Box                               |
|  334 | 3_01_MeetClimb                  | Box                               |
|  335 | 3_01_MissionArea                | Box                               |
|  336 | 3_01_MissionBlock               | Box                               |
|  337 | 3_01_OnRoof                     | Box                               |
|  338 | 3_02_BUSINESSAREA               | Box                               |
|  339 | 3_02_BUSINESSAREA               | Box                               |
|  340 | 3_02_PARKENTRANCE               | Box                               |
|  341 | 3_02_PARKENTRANCE               | Box                               |
|  342 | 3_02_SPAWNER01                  | Box                               |
|  343 | 3_02_SPAWNER01                  | Box                               |
|  344 | 3_02_SPAWNER02                  | Box                               |
|  345 | 3_02_SPAWNER02                  | Box                               |
|  346 | 3_02_SPAWNER03                  | Box                               |
|  347 | 3_02_SPAWNER03                  | Box                               |
|  348 | 3_02_SPAWNER04                  | Box                               |
|  349 | 3_02_SPAWNER04                  | Box                               |
|  350 | 3_02_SPAWNER05                  | Box                               |
|  351 | 3_02_SPAWNER05                  | Box                               |
|  352 | 3_04_algieFlee                  | Box                               |
|  353 | 3_04_cornScream2                | Box                               |
|  354 | 3_04_corneliusCut               | Box                               |
|  355 | 3_04_loadBikes                  | Box                               |
|  356 | 3_04_stg4_Return                | Box                               |
|  357 | 3_05_1StartUpstairs             | Box                               |
|  358 | 3_05_2CatwalkStart              | Box                               |
|  359 | 3_05_3NortonsDoor               | Door                              |
|  360 | 3_05_Ambush                     | Box                               |
|  361 | 3_05_BossFightTrigger           | Box                               |
|  362 | 3_05_Catwalk2                   | Box                               |
|  363 | 3_05_ExitGreasers1              | Box                               |
|  364 | 3_05_Hammerwall01               | Box                               |
|  365 | 3_05_Hammerwall02               | Box                               |
|  366 | 3_05_Hammerwall03               | Box                               |
|  367 | 3_05_Hammerwall04               | Box                               |
|  368 | 3_05_Hammerwall05               | Box                               |
|  369 | 3_05_SecondFloor                | Box                               |
|  370 | 3_05_StartCatwalk               | Box                               |
|  371 | 3_05_StartShooting              | Box                               |
|  372 | 3_05_StartShooting2             | Box                               |
|  373 | 3_06_FailTrig                   | Box                               |
|  374 | 3_06_FightTrig                  | Box                               |
|  375 | 3_06_InnerArea                  | Box                               |
|  376 | 3_06_OuterArea                  | Box                               |
|  377 | 3_07_StartConv                  | Box                               |
|  378 | 3_08_BackToRoomTrig             | Box                               |
|  379 | 3_08_Intercom_Trigger           | Box                               |
|  380 | 3_08_RunStart                   | Box                               |
|  381 | 3_08_SchoolPop                  | PopulationPed                     |
|  382 | 3_B_BIKE_REGION_NE              | Box                               |
|  383 | 3_B_BIKE_REGION_NW              | Box                               |
|  384 | 3_B_BIKE_REGION_SE              | Box                               |
|  385 | 3_B_BIKE_REGION_SW              | Box                               |
|  386 | 3_B_MAGNET                      | Box                               |
|  387 | 3_B_REGION_S                    | Box                               |
|  388 | 3_B_STAGE_2_TRIGGER             | Box                               |
|  389 | 3_G3_CheeringCrowd              | Box                               |
|  390 | 3_G3_MoveLola                   | Box                               |
|  391 | 3_G3_Tree1                      | Box                               |
|  392 | 3_G3_Tree2                      | Box                               |
|  393 | 3_G3_Tree3                      | Box                               |
|  394 | 3_G3_Tree4                      | Box                               |
|  395 | 3_R09_AreaT01                   | Box                               |
|  396 | 3_R09_AreaT01                   | Box                               |
|  397 | 3_R09_AreaT01                   | Box                               |
|  398 | 3_R09_AreaT01                   | Box                               |
|  399 | 3_R09_AreaT02                   | Box                               |
|  400 | 3_R09_AreaT02                   | Box                               |
|  401 | 3_R09_AreaT02                   | Box                               |
|  402 | 3_R09_AreaT02                   | Box                               |
|  403 | 3_R09_BasementTrigger           | Box                               |
|  404 | 3_R09_MainArea                  | Box                               |
|  405 | 3_R09_MainArea                  | Box                               |
|  406 | 3_R09_SpawnT01                  | Box                               |
|  407 | 3_R09_SpawnT01                  | Box                               |
|  408 | 3_R09_SpawnT01                  | Box                               |
|  409 | 3_R09_SpawnT01                  | Box                               |
|  410 | 3_R09_SpawnT01                  | Box                               |
|  411 | 3_R09_SpawnT02                  | Box                               |
|  412 | 3_R09_SpawnT02                  | Box                               |
|  413 | 3_R09_SpawnT02                  | Box                               |
|  414 | 3_R09_SpawnT02                  | Box                               |
|  415 | 3_R09_SpawnT02                  | Box                               |
|  416 | 3_R09_Upstairs                  | Box                               |
|  417 | 3_S03T_H_Car_Drop7_Stop         | Box                               |
|  418 | 3_S03T_OPEN_GATE_T              | Box                               |
|  419 | 3_S03T_Test_1                   | PopulationPed                     |
|  420 | 3_S03T_Test_1_Activate          | Box                               |
|  421 | 3_S03T_Test_2                   | Box                               |
|  422 | 3_S03T_Test_2_Activate          | Box                               |
|  423 | 3_S03T_Test_3                   | PopulationPed                     |
|  424 | 3_S03T_Test_3_Activate          | Box                               |
|  425 | 3_S03T_Test_4                   | PopulationPed                     |
|  426 | 3_S03T_Test_4_Activate          | Box                               |
|  427 | 3_S03T_Test_5                   | PopulationPed                     |
|  428 | 3_S03T_Test_5_Activate          | Box                               |
|  429 | 3_S03T_Test_6                   | PopulationPed                     |
|  430 | 3_S03T_Test_6_Activate          | Box                               |
|  431 | 3_S03_TEMP_DOORTELEPORT         | Box                               |
|  432 | 3_S03_failAlley                 | Box                               |
|  433 | 3_S03_failGreaser               | Box                               |
|  434 | 3_S03_failPool                  | Box                               |
|  435 | 3_S03_objectiveAlley            | Box                               |
|  436 | 3_S03_objectiveGreaser          | Box                               |
|  437 | 3_S03_objectivePool             | Box                               |
|  438 | 3_S03_parkingLot                | Box                               |
|  439 | 3_S03_poolArea                  | Box                               |
|  440 | 3_S09_AmbushTrigger01           | Box                               |
|  441 | 3_S09_AmbushTrigger02           | Box                               |
|  442 | 3_S09_AmbushTrigger03           | Box                               |
|  443 | 3_S09_Breakable01               | Box                               |
|  444 | 3_S09_Breakable02               | Box                               |
|  445 | 3_S09_Breakable03               | Box                               |
|  446 | 3_S09_Breakable04               | Box                               |
|  447 | 3_S09_Breakable05               | Box                               |
|  448 | 3_S09_Breakable06               | Box                               |
|  449 | 3_S09_Breakable07               | Box                               |
|  450 | 3_S09_Breakable08               | Box                               |
|  451 | 3_S09_Breakable09               | Box                               |
|  452 | 3_S09_Breakable10               | Box                               |
|  453 | 3_S09_Cover01                   | Box                               |
|  454 | 3_S09_Cover01                   | Box                               |
|  455 | 3_S09_Cover02                   | Box                               |
|  456 | 3_S09_Cover02                   | Box                               |
|  457 | 3_S09_Cover03                   | Box                               |
|  458 | 3_S09_Cover03                   | Box                               |
|  459 | 3_S09_Cover04                   | Box                               |
|  460 | 3_S09_Cover04                   | Box                               |
|  461 | 3_S09_Cover05                   | Box                               |
|  462 | 3_S09_CoverArea                 | Box                               |
|  463 | 3_S09_CoverArea                 | Box                               |
|  464 | 3_S09_CoverCrate01              | Box                               |
|  465 | 3_S09_CoverCrate02              | Box                               |
|  466 | 3_S09_Dumpster01                | Box                               |
|  467 | 3_S09_Dumpster01                | Box                               |
|  468 | 3_S09_LeavingTrigger            | Box                               |
|  469 | 3_S09_LeavingTrigger            | Box                               |
|  470 | 3_S10_ATagsLoad                 | Box                               |
|  471 | 3_S10_BTagsLoad                 | Box                               |
|  472 | 3_S10_CTagsLoad                 | Box                               |
|  473 | 3_S10_DTagsLoad                 | Box                               |
|  474 | 3_S10_PoorArea                  | Box                               |
|  475 | 3_S10_TUT_TAG                   | Box                               |
|  476 | 3_S10_TutTrigger                | Box                               |
|  477 | 3_S10_Tut_Tag02                 | Box                               |
|  478 | 3_S10_Tut_Tag03                 | Box                               |
|  479 | 3_S10_TutorialStart             | Box                               |
|  480 | 3_S10_underBridge               | Box                               |
|  481 | 3_S11_Asylum_Gate_Warning       | Box                               |
|  482 | 3_S11_Asylum_Gate_Warning2      | Box                               |
|  483 | 3_S11_Break_Out                 | Box                               |
|  484 | 3_S11_Fire01                    | Box                               |
|  485 | 3_S11_Fire02                    | Box                               |
|  486 | 3_S11_Fire03                    | Box                               |
|  487 | 3_S11_Fire04                    | Box                               |
|  488 | 3_S11_Fire05                    | Box                               |
|  489 | 3_S11_Fire06                    | Box                               |
|  490 | 3_S11_Fire07                    | Box                               |
|  491 | 3_S11_Galloway_Trigger          | Box                               |
|  492 | 3_S11_Inside_Asylum             | Box                               |
|  493 | 3_S11_PHILLIPS_REUNION          | Box                               |
|  494 | 3_S11_Phillips_Car_Stop         | Box                               |
|  495 | 3_S11_Player_On_A_Grounds       | Box                               |
|  496 | 3_S_10_FailTrigger              | Box                               |
|  497 | 3_XM_SpawnTrigger               | Box                               |
|  498 | 4_01_artNorth                   | Box                               |
|  499 | 4_01_artSouth                   | Box                               |
|  500 | 4_01_christySpeech              | Box                               |
|  501 | 4_01_girlsDormBathroom          | Box                               |
|  502 | 4_01_gymInsideDoor              | Box                               |
|  503 | 4_01_gymTunnel                  | Box                               |
|  504 | 4_01_launchEunice               | Box                               |
|  505 | 4_01_mandyRoom                  | Box                               |
|  506 | 4_01_mandyRoomBusted            | Box                               |
|  507 | 4_01_mandyRoomWarn              | Box                               |
|  508 | 4_01_showerRoom                 | Box                               |
|  509 | 4_01_showerWarn                 | Box                               |
|  510 | 4_01_tutLattice                 | Box                               |
|  511 | 4_02_Algie_Final_Stand          | Box                               |
|  512 | 4_02_Algie_Left_Lib             | Box                               |
|  513 | 4_02_Bar_01                     | Box                               |
|  514 | 4_02_Bar_01                     | Box                               |
|  515 | 4_02_Bar_02                     | Box                               |
|  516 | 4_02_Bar_02                     | Box                               |
|  517 | 4_02_Bar_03                     | Box                               |
|  518 | 4_02_Bar_03                     | Box                               |
|  519 | 4_02_Breaker_Box                | Box                               |
|  520 | 4_02_Breaker_Box                | Box                               |
|  521 | 4_02_Delete_Wave1               | Box                               |
|  522 | 4_02_Delete_Wave1               | Box                               |
|  523 | 4_02_Delete_Wave3               | Box                               |
|  524 | 4_02_Delete_Wave3               | Box                               |
|  525 | 4_02_Eavesdrop                  | Box                               |
|  526 | 4_02_Eavesdrop                  | Box                               |
|  527 | 4_02_Finale                     | Box                               |
|  528 | 4_02_Finale                     | Box                               |
|  529 | 4_02_GateKeeper                 | Box                               |
|  530 | 4_02_KeyPad                     | Box                               |
|  531 | 4_02_NERDS                      | PopulationPed                     |
|  532 | 4_02_NERDS                      | PopulationPed                     |
|  533 | 4_02_Nerd_Ambush1               | Box                               |
|  534 | 4_02_Nerd_Ambush2               | Box                               |
|  535 | 4_02_Nerd_Deleter               | Box                               |
|  536 | 4_02_O_R1_1T                    | Box                               |
|  537 | 4_02_O_R1_1T                    | Box                               |
|  538 | 4_02_O_R2_1T                    | Box                               |
|  539 | 4_02_O_R2_1T                    | Box                               |
|  540 | 4_02_O_WN1_1T                   | Box                               |
|  541 | 4_02_O_WN1_1T                   | Box                               |
|  542 | 4_02_O_WN2_1T                   | Box                               |
|  543 | 4_02_O_WN2_1T                   | Box                               |
|  544 | 4_02_O_WN3_1T                   | Box                               |
|  545 | 4_02_O_WN3_1T                   | Box                               |
|  546 | 4_02_O_WN4_1T                   | Box                               |
|  547 | 4_02_O_WN4_1T                   | Box                               |
|  548 | 4_02_O_W_F_1T                   | Box                               |
|  549 | 4_02_ObsDoor                    | Door                              |
|  550 | 4_02_ObsDoorCheck               | Box                               |
|  551 | 4_02_PREFECT1                   | PopulationPed                     |
|  552 | 4_02_PREFECT1                   | PopulationPed                     |
|  553 | 4_02_PREFECT2                   | PopulationPed                     |
|  554 | 4_02_PREFECT2                   | PopulationPed                     |
|  555 | 4_02_P_Wave2                    | Box                               |
|  556 | 4_02_P_Wave2                    | Box                               |
|  557 | 4_02_P_Wave3                    | Box                               |
|  558 | 4_02_P_Wave3                    | Box                               |
|  559 | 4_02_P_Wave4                    | Box                               |
|  560 | 4_02_P_Wave4                    | Box                               |
|  561 | 4_02_Player_On_CannonT          | Box                               |
|  562 | 4_02_Player_On_CannonT          | Box                               |
|  563 | 4_02_Player_Out_Of_Lib          | Box                               |
|  564 | 4_02_Player_Out_Of_Lib          | Box                               |
|  565 | 4_02_Spotted_Scout              | Box                               |
|  566 | 4_02_Spotted_Scout              | Box                               |
|  567 | 4_02_Spud_Cannon                | Box                               |
|  568 | 4_02_Spud_Cannon                | Box                               |
|  569 | 4_02_Spud_Tripod                | Box                               |
|  570 | 4_02_Spud_Tripod                | Box                               |
|  571 | 4_02_TEMP_Cannon_Line2          | Box                               |
|  572 | 4_02_TEMP_Cannon_Line2          | Box                               |
|  573 | 4_02_WATER                      | Box                               |
|  574 | 4_03_Bar_05_01                  | Door                              |
|  575 | 4_03_Bar_05_02                  | Door                              |
|  576 | 4_03_Bar_Blip_Trigger           | Box                               |
|  577 | 4_03_Cannon                     | Box                               |
|  578 | 4_03_Cannon_Tripod              | Box                               |
|  579 | 4_03_Jock_Past_Water            | Box                               |
|  580 | 4_03_Leave1                     | Box                               |
|  581 | 4_03_Leave2                     | Box                               |
|  582 | 4_03_Ob_Bar1                    | Box                               |
|  583 | 4_03_Ob_Bar2                    | Box                               |
|  584 | 4_03_Ob_Bar3                    | Box                               |
|  585 | 4_03_Ob_Bar4                    | Box                               |
|  586 | 4_03_Ob_Grounds                 | Box                               |
|  587 | 4_03_ObsDoor                    | Door                              |
|  588 | 4_03_Open_Door                  | Box                               |
|  589 | 4_03_Open_Door2                 | Box                               |
|  590 | 4_03_Player_To_Far              | Box                               |
|  591 | 4_03_SetUp_Nerds                | Box                               |
|  592 | 4_03_TETHER_BAR_04              | Box                               |
|  593 | 4_03_Trigger_Wave1              | Box                               |
|  594 | 4_04_CTRLROOM                   | Box                               |
|  595 | 4_04_ENDMINE                    | Box                               |
|  596 | 4_04_EXIT                       | Box                               |
|  597 | 4_04_JOCKNIS                    | Box                               |
|  598 | 4_04_MAZE_HALL_05               | Box                               |
|  599 | 4_04_MAZE_HALL_07               | Box                               |
|  600 | 4_04_MAZE_HALL_08               | Box                               |
|  601 | 4_04_MINE_ESCAPE                | Box                               |
|  602 | 4_04_MONITOR01                  | Box                               |
|  603 | 4_04_MONITOR02                  | Box                               |
|  604 | 4_04_MONITOR03                  | Box                               |
|  605 | 4_04_MineNerds1                 | Box                               |
|  606 | 4_04_MineNerds2                 | Box                               |
|  607 | 4_04_MineNerds3                 | Box                               |
|  608 | 4_04_NerdTrig                   | Box                               |
|  609 | 4_04_REACHED_FUNHOUSE           | Box                               |
|  610 | 4_04_Reaper01                   | Box                               |
|  611 | 4_04_Reaper02                   | Box                               |
|  612 | 4_04_Reaper03                   | Box                               |
|  613 | 4_04_Reaper04                   | Box                               |
|  614 | 4_04_Reaper05                   | Box                               |
|  615 | 4_04_Reaper06                   | Box                               |
|  616 | 4_04_ReaperRoom                 | Box                               |
|  617 | 4_05_FIELD                      | Box                               |
|  618 | 4_05_failAlley                  | Box                               |
|  619 | 4_05_failMain                   | Box                               |
|  620 | 4_05_failPath                   | Box                               |
|  621 | 4_05_mascotPOI1                 | Box                               |
|  622 | 4_05_mascotPOI2                 | Box                               |
|  623 | 4_05_mascotPOI3                 | Box                               |
|  624 | 4_05_mascotPOI4                 | Box                               |
|  625 | 4_05_mascotPOI5                 | Box                               |
|  626 | 4_05_nerdAmbush                 | Box                               |
|  627 | 4_05_warnAlley                  | Box                               |
|  628 | 4_05_warnMain                   | Box                               |
|  629 | 4_05_warnPath                   | Box                               |
|  630 | 4_05cut_fakeDoor                | Box                               |
|  631 | 4_06_BIB01                      | Box                               |
|  632 | 4_06_BIB02                      | Box                               |
|  633 | 4_06_BIB03                      | Box                               |
|  634 | 4_06_Bench_01                   | Box                               |
|  635 | 4_06_Bench_01A                  | Box                               |
|  636 | 4_06_Bench_02                   | Box                               |
|  637 | 4_06_Bench_02A                  | Box                               |
|  638 | 4_06_Bench_03                   | Box                               |
|  639 | 4_06_Bench_03A                  | Box                               |
|  640 | 4_06_Bench_04                   | Box                               |
|  641 | 4_06_Bench_04A                  | Box                               |
|  642 | 4_06_Cooler                     | Box                               |
|  643 | 4_06_Cooler_Location            | Box                               |
|  644 | 4_06_DockingTrigger             | Box                               |
|  645 | 4_06_Duffle_Bag                 | Box                               |
|  646 | 4_06_Field01                    | Box                               |
|  647 | 4_06_Field02                    | Box                               |
|  648 | 4_06_Field03                    | Box                               |
|  649 | 4_06_Field_Zone                 | Box                               |
|  650 | 4_06_GatObjective               | Box                               |
|  651 | 4_06_Hack_Switch                | Box                               |
|  652 | 4_06_InsideDockingTrigger       | Box                               |
|  653 | 4_06_Load_Field                 | Box                               |
|  654 | 4_06_OOB01                      | Box                               |
|  655 | 4_06_OOB02                      | Box                               |
|  656 | 4_06_OOB03                      | Box                               |
|  657 | 4_06_OPAENDTRIGG                | Box                               |
|  658 | 4_06_OPCENDTRIGG                | Box                               |
|  659 | 4_06_OutsideGate                | Box                               |
|  660 | 4_B1_EARNEST_PATTERN02          | Box                               |
|  661 | 4_B1_EARNEST_PATTERN03          | Box                               |
|  662 | 4_G4_BleacherPervert            | Box                               |
|  663 | 4_G4_BusPoster02                | Box                               |
|  664 | 4_G4_BusPoster08                | Box                               |
|  665 | 4_G4_BusTag2                    | Box                               |
|  666 | 4_G4_BusTag8                    | Box                               |
|  667 | 4_G4_LIBNERDS                   | Box                               |
|  668 | 4_G4_LeftTown                   | Box                               |
|  669 | 4_G4_NerdComics                 | Box                               |
|  670 | 4_G4_OutOfGrounds               | Box                               |
|  671 | 4_G4_SchoolPoster02             | Box                               |
|  672 | 4_G4_SchoolPoster03             | Box                               |
|  673 | 4_G4_SchoolPoster04             | Box                               |
|  674 | 4_G4_SchoolTag2                 | Box                               |
|  675 | 4_G4_SchoolTag3                 | Box                               |
|  676 | 4_G4_SchoolTag4                 | Box                               |
|  677 | 4_G4_TaggingTrig                | Box                               |
|  678 | 4_G4_TaggingTrig3               | Box                               |
|  679 | 4_G4_TiltPost1                  | Box                               |
|  680 | 4_G4_TiltTag1                   | Box                               |
|  681 | 4_S11_AtticPlank01              | Box                               |
|  682 | 4_S11_AtticPlank02              | Box                               |
|  683 | 4_S11_AtticPlank03              | Box                               |
|  684 | 4_S11_DockerDoor                | Box                               |
|  685 | 4_S11_EndTrigger                | Box                               |
|  686 | 4_S11_FieldTrigger              | Box                               |
|  687 | 4_S11_GymBag                    | Box                               |
|  688 | 4_S11_GymBagTrigger             | Box                               |
|  689 | 4_S11_JPhoto                    | Box                               |
|  690 | 4_S11_JockDiscoveryTrigger      | Box                               |
|  691 | 4_S11_LockedDoor                | Box                               |
|  692 | 4_S11_NerdTrigger               | Box                               |
|  693 | 4_S11_PaddleTrigger             | Box                               |
|  694 | 4_S11_RandomTeacherTrigger      | Box                               |
|  695 | 4_S11_SafeZone                  | Box                               |
|  696 | 4_S11_SafeZoneA                 | Box                               |
|  697 | 4_S11_SafeZoneB                 | Box                               |
|  698 | 4_S12_MSPHILLIPS                | Box                               |
|  699 | 4_S12_PEANUTBIKE                | Box                               |
|  700 | 4_S12_PEANUTBIKE2               | Box                               |
|  701 | 5_01_Meet_Librarian             | Box                               |
|  702 | 5_01_RatSpawnT01                | Box                               |
|  703 | 5_01_RatSpawnT02                | Box                               |
|  704 | 5_01_RatSpawnT03                | Box                               |
|  705 | 5_01_RatSpawnT04                | Box                               |
|  706 | 5_01_RatSpawnT05                | Box                               |
|  707 | 5_01_RatSpawnT06                | Box                               |
|  708 | 5_01_RatSpawnT07                | Box                               |
|  709 | 5_01_RatSpawnT08                | Box                               |
|  710 | 5_01_RatSpawnT09                | Box                               |
|  711 | 5_01_RatSpawnT10                | Box                               |
|  712 | 5_01_RatSpawnT11                | Box                               |
|  713 | 5_01_RatSpawnT12                | Box                               |
|  714 | 5_01_RatSpawnT13                | Box                               |
|  715 | 5_01_RatSpawnT14                | Box                               |
|  716 | 5_01_RatSpawnT15                | Box                               |
|  717 | 5_01_RatSpawnT16                | Box                               |
|  718 | 5_01_RatSpawnT17                | Box                               |
|  719 | 5_01_RatSpawnT18                | Box                               |
|  720 | 5_01_RatSpawnT19                | Box                               |
|  721 | 5_01_RatSpawnT20                | Box                               |
|  722 | 5_01_main_room_tr               | Box                               |
|  723 | 5_02_BigSmoke                   | Box                               |
|  724 | 5_02_BonfireTrigger01           | Box                               |
|  725 | 5_02_BonfireTrigger02           | Box                               |
|  726 | 5_02_DepopRichArea              | PopulationPed                     |
|  727 | 5_02_DepopulateDocks            | PopulationPed + PopulationVehicle |
|  728 | 5_02_DockPartyCreate            | Box                               |
|  729 | 5_02_FailTrigger                | Box                               |
|  730 | 5_02_FinalNIS                   | Box                               |
|  731 | 5_02_Flame01                    | Box                               |
|  732 | 5_02_Flame02                    | Box                               |
|  733 | 5_02_Flame03                    | Box                               |
|  734 | 5_02_GameArea                   | Box                               |
|  735 | 5_02_GreaserHangout             | Box                               |
|  736 | 5_02_InWarehouse                | Box                               |
|  737 | 5_02_NearNIS                    | Box                               |
|  738 | 5_02_OnBarge                    | Box                               |
|  739 | 5_02_PortExit                   | Box                               |
|  740 | 5_02_RatCrate                   | Box                               |
|  741 | 5_02_StartRatPhoto              | Box                               |
|  742 | 5_02_TrophyPile                 | Box                               |
|  743 | 5_02_WarehouseUpstairs          | Box                               |
|  744 | 5_02_WarehouseUpstairs02        | Box                               |
|  745 | 5_03_1st_Floor_1st_Hall         | Box                               |
|  746 | 5_03_Asylum_Grounds_SetUp       | Box                               |
|  747 | 5_03_BlockB                     | Box                               |
|  748 | 5_03_Control_Room_Door          | Box                               |
|  749 | 5_03_DOW_1                      | Box                               |
|  750 | 5_03_DOW_2                      | Box                               |
|  751 | 5_03_DOW_3                      | Box                               |
|  752 | 5_03_Exit                       | Box                               |
|  753 | 5_03_FIRE01                     | Box                               |
|  754 | 5_03_FIRE02                     | Box                               |
|  755 | 5_03_FIRE03                     | Box                               |
|  756 | 5_03_FIRE04                     | Box                               |
|  757 | 5_03_FIRE05                     | Box                               |
|  758 | 5_03_FRONT_GATE_LINE            | Box                               |
|  759 | 5_03_GameOver                   | Box                               |
|  760 | 5_03_Gen_Johnny                 | Box                               |
|  761 | 5_03_Inside_Asylum              | Box                               |
|  762 | 5_03_JOHNNY_END_TRIGGER         | Box                               |
|  763 | 5_03_Johnny_Goto1               | Box                               |
|  764 | 5_03_Johnny_Trig1               | Box                               |
|  765 | 5_03_Johnny_Yelling             | Box                               |
|  766 | 5_03_LEFT                       | Box                               |
|  767 | 5_03_Leaving                    | Box                               |
|  768 | 5_03_OnGrounds                  | Box                               |
|  769 | 5_03_Orderly_CS1_1              | Box                               |
|  770 | 5_03_Player_In_CR               | Box                               |
|  771 | 5_03_Rec_Room                   | Box                               |
|  772 | 5_04_AMBUSH_01                  | Box                               |
|  773 | 5_04_AMBUSH_02                  | Box                               |
|  774 | 5_04_AMBUSH_03                  | Box                               |
|  775 | 5_04_AMBUSH_04                  | Box                               |
|  776 | 5_04_AMBUSH_05                  | Box                               |
|  777 | 5_04_BANNERS_01                 | Box                               |
|  778 | 5_04_BANNERS_02                 | Box                               |
|  779 | 5_04_BANNERS_03                 | Box                               |
|  780 | 5_04_BANNERS_04                 | Box                               |
|  781 | 5_04_BANNERS_05                 | Box                               |
|  782 | 5_04_BANNERS_06                 | Box                               |
|  783 | 5_04_BANNERS_07                 | Box                               |
|  784 | 5_04_BANNERS_08                 | Box                               |
|  785 | 5_04_BANNERS_09                 | Box                               |
|  786 | 5_04_BANNERS_10                 | Box                               |
|  787 | 5_04_BANNERS_11                 | Box                               |
|  788 | 5_04_BANNERS_12                 | Box                               |
|  789 | 5_04_BANNERS_13                 | Box                               |
|  790 | 5_04_BIKE_STOP_01               | Box                               |
|  791 | 5_04_BIKE_STOP_02               | Box                               |
|  792 | 5_04_CHANGEROOM                 | Box                               |
|  793 | 5_04_COP_START_01               | Box                               |
|  794 | 5_04_COP_START_02               | Box                               |
|  795 | 5_04_CREATE_FOURTH_PEDS         | Box                               |
|  796 | 5_04_DOOR_HACK                  | Box                               |
|  797 | 5_04_DO_CHAT                    | Box                               |
|  798 | 5_04_DO_ESCAPE                  | Box                               |
|  799 | 5_04_DO_GOAL                    | Box                               |
|  800 | 5_04_DO_NEAR_BIKE               | Box                               |
|  801 | 5_04_DO_STOP_01                 | Box                               |
|  802 | 5_04_GYMHOOP                    | Door                              |
|  803 | 5_04_GYMWALL                    | Door                              |
|  804 | 5_04_LASTAMBUSH                 | Box                               |
|  805 | 5_04_LIGHT_01                   | Box                               |
|  806 | 5_04_LIGHT_02                   | Box                               |
|  807 | 5_04_LIGHT_03                   | Box                               |
|  808 | 5_04_LIGHT_04                   | Box                               |
|  809 | 5_04_OTHERROUTE                 | Box                               |
|  810 | 5_04_PREVENT01                  | Box                               |
|  811 | 5_04_PREVENT02                  | Box                               |
|  812 | 5_05_Alley                      | Box                               |
|  813 | 5_05_BoltCutters                | Box                               |
|  814 | 5_05_BurtonTether               | Box                               |
|  815 | 5_05_ClearMower                 | Box                               |
|  816 | 5_05_DogFood                    | Box                               |
|  817 | 5_05_ExcludedMeatFactory        | Box                               |
|  818 | 5_05_FactoryArea                | Box                               |
|  819 | 5_05_LastPotty                  | Box                               |
|  820 | 5_05_POTTY                      | Box                               |
|  821 | 5_05_Park                       | Box                               |
|  822 | 5_05_ParkOut                    | Box                               |
|  823 | 5_05_RunAwayZoe                 | Box                               |
|  824 | 5_05_TBoneTarget                | Box                               |
|  825 | 5_06_BarricadeCrash             | Box                               |
|  826 | 5_06_BarricadeDoor              | Box                               |
|  827 | 5_06_BikeTrigger                | Box                               |
|  828 | 5_06_Bridge                     | Box                               |
|  829 | 5_06_EndTrigger                 | Box                               |
|  830 | 5_06_RussellDoor                | Box                               |
|  831 | 5_06_RussellGarage              | Box                               |
|  832 | 5_06_RussellGate                | Box                               |
|  833 | 5_06_RussellTrigger             | Box                               |
|  834 | 5_07_BarricadeNIS               | Box                               |
|  835 | 5_07_ChemEntrance               | Box                               |
|  836 | 5_07_DoorLocked01               | Box                               |
|  837 | 5_07_DoorLocked02               | Box                               |
|  838 | 5_07_ElectricDoor               | Box                               |
|  839 | 5_07_Fire01                     | Box                               |
|  840 | 5_07_FirstZoe                   | Box                               |
|  841 | 5_07_MissionInit                | Box                               |
|  842 | 5_07_OmarFight                  | Box                               |
|  843 | 5_07_OutsideTheOffice           | Box                               |
|  844 | 5_07_PartThree                  | Box                               |
|  845 | 5_07_PedAttack01                | Box                               |
|  846 | 5_07_PedAttack02                | Box                               |
|  847 | 5_07_PedAttack03                | Box                               |
|  848 | 5_07_Ranged01                   | Box                               |
|  849 | 5_07_Ranged02                   | Box                               |
|  850 | 5_07_SecondZoe                  | Box                               |
|  851 | 5_07_SecuritySwitch             | Box                               |
|  852 | 5_07_SiloAttack01               | Box                               |
|  853 | 5_07_Slaughterhouse             | Box                               |
|  854 | 5_07_Spawner01                  | Box                               |
|  855 | 5_07_Spawner02                  | Box                               |
|  856 | 5_07_TrainSwitch                | Box                               |
|  857 | 5_07_TrainSwitch02              | Box                               |
|  858 | 5_09_Ambush                     | Box                               |
|  859 | 5_09_CityHallArea               | Box                               |
|  860 | 5_09_CityHallTag2               | Box                               |
|  861 | 5_09_CityHallTag3               | Box                               |
|  862 | 5_09_CityHall_Building          | Box                               |
|  863 | 5_09_CityHall_Grounds           | Box                               |
|  864 | 5_09_CityHall_Tag               | Box                               |
|  865 | 5_09_CityHall_Tower             | Box                               |
|  866 | 5_09_CityHall_Wall_Climbed      | Box                               |
|  867 | 5_09_DogYard                    | Box                               |
|  868 | 5_09_Earnest_Outdoors           | Box                               |
|  869 | 5_09_GreaserLoad                | Box                               |
|  870 | 5_09_Greaser_Safezone           | Box                               |
|  871 | 5_09_Paint_Yard                 | Box                               |
|  872 | 5_09_PhotoOp                    | Box                               |
|  873 | 5_09_Players_Room               | Box                               |
|  874 | 5_09_TowerTop                   | Box                               |
|  875 | 5_B_CHEM_DOOR                   | Box                               |
|  876 | 5_B_CHEM_DOOR_2                 | Box                               |
|  877 | 5_B_CRAWL                       | Box                               |
|  878 | 5_B_ChemCamShot                 | Box                               |
|  879 | 5_B_ChemCamShot02               | Box                               |
|  880 | 5_B_DEBUG_EDGAR                 | Box                               |
|  881 | 5_B_ENTRANCE                    | Box                               |
|  882 | 5_B_FALL_INTO_SLUDGE            | Box                               |
|  883 | 5_B_FINALSTAGE                  | Box                               |
|  884 | 5_B_GRAB_GOOD                   | Box                               |
|  885 | 5_B_LIFTDOWN                    | Box                               |
|  886 | 5_B_LIFTUP                      | Box                               |
|  887 | 5_B_LadderCamShot               | Box                               |
|  888 | 5_B_LadderCamShot02             | Box                               |
|  889 | 5_B_LadderCamShot03             | Box                               |
|  890 | 5_B_LowStaircase                | Box                               |
|  891 | 5_B_STAGE2_START                | Box                               |
|  892 | 5_B_STEAMAREA                   | Box                               |
|  893 | 5_B_SecDoor1                    | Box                               |
|  894 | 5_B_SecDoor2                    | Box                               |
|  895 | 5_G5_GroundDoorExit             | Box                               |
|  896 | 5_G5_Ladder04                   | Box                               |
|  897 | 5_G5_WHBackDoor                 | Box                               |
|  898 | 5_G5_WHFrontDoor                | Box                               |
|  899 | 5_G5_WareDoorZoe                | Box                               |
|  900 | 5_G5_Zone01                     | Box                               |
|  901 | 5_G5_Zone02                     | Box                               |
|  902 | 5_G5_Zone03                     | Box                               |
|  903 | 5_G5_Zone04                     | Box                               |
|  904 | 5_G5_finish                     | Box                               |
|  905 | 5_G5_meet_zoe                   | Box                               |
|  906 | 5_T1_BikeGarage                 | Box                               |
|  907 | 602_LibEntrance                 | Box                               |
|  908 | 6_01_PRINCIPALTRIG              | Box                               |
|  909 | 6_02A_BACKROUTE_STUDENTS        | Box                               |
|  910 | 6_02A_IA_COPS                   | Box                               |
|  911 | 6_02A_SCHOOLFRONT_COPS          | Box                               |
|  912 | 6_02A_SF_GIRLS                  | Box                               |
|  913 | 6_02_WonderMeats                | Box                               |
|  914 | 6_02g_bottomStairs              | Box                               |
|  915 | 6_02g_downstairs                | Box                               |
|  916 | 6_02g_entrance                  | Box                               |
|  917 | 6_02g_fireVase02                | Box                               |
|  918 | 6_02g_johnny                    | Box                               |
|  919 | 6_02g_livingroom                | Box                               |
|  920 | 6_02g_loadPeds                  | Box                               |
|  921 | 6_02g_norton                    | Box                               |
|  922 | 6_02g_vase01                    | Box                               |
|  923 | 6_02g_vase02                    | Box                               |
|  924 | 6_02g_vase03                    | Box                               |
|  925 | 6_03_Fail01                     | Box                               |
|  926 | 6_03_Fail02                     | Box                               |
|  927 | 6_03_Fail03                     | Box                               |
|  928 | 6_03_GetAway                    | Box                               |
|  929 | 6_03_GymPop                     | PopulationPed                     |
|  930 | 6_03_HallPopOverride            | Box                               |
|  931 | 6_03_NISJOCK01                  | Box                               |
|  932 | 6_03_NISJOCK02                  | Box                               |
|  933 | 6_03_NISJOCK03                  | Box                               |
|  934 | 6_03_NISJOCK04                  | Box                               |
|  935 | 6_03_NISNERD01                  | Box                               |
|  936 | 6_03_NISNERD02                  | Box                               |
|  937 | 6_03_NISNERD03                  | Box                               |
|  938 | 6_03_NISNERD04                  | Box                               |
|  939 | 6_03_NISNERD05                  | Box                               |
|  940 | 6_03_WarnFail01                 | Box                               |
|  941 | 6_03_WarnFail02                 | Box                               |
|  942 | 6_03_WarnFail03                 | Box                               |
|  943 | 6_B_BELLS_ONE                   | Box                               |
|  944 | 6_B_BELLS_THREE                 | Box                               |
|  945 | 6_B_BELLS_TWO                   | Box                               |
|  946 | 6_B_FIRSTPLANKRUN               | Box                               |
|  947 | 6_B_GARY_THROW_1                | Box                               |
|  948 | 6_B_GARY_THROW_2                | Box                               |
|  949 | 6_B_GARY_TRIGGER_1              | Box                               |
|  950 | 6_B_GARY_TRIGGER_2              | Box                               |
|  951 | 6_B_GARY_TRIGGER_3              | Box                               |
|  952 | 6_B_GARY_TRIGGER_4              | Box                               |
|  953 | 6_B_GARY_TRIGGER_5              | Box                               |
|  954 | 6_B_GARY_TRIGGER_6              | Box                               |
|  955 | 6_B_GLASS_TRIGGER               | Box                               |
|  956 | 6_B_LADDER1_BEGIN               | Box                               |
|  957 | 6_B_LADDER2_BEGIN               | Box                               |
|  958 | 6_B_OFFROOF                     | Box                               |
|  959 | 6_B_START                       | Box                               |
|  960 | 6_B_SchoolRoofTop               | Box                               |
|  961 | AMB_BUSINESS_AREA               | Box                               |
|  962 | AMB_Beach02_ISLAND              | Box                               |
|  963 | AMB_CARNIVAL_AREA               | Box                               |
|  964 | AMB_CHEMLAB                     | Box                               |
|  965 | AMB_ForestBeachTunnel           | Box                               |
|  966 | AMB_HOBOAREA                    | Box                               |
|  967 | AMB_INDUSTRIAL_AREA             | Box                               |
|  968 | AMB_JunkYard_AREA               | Box                               |
|  969 | AMB_Openwater                   | Box                               |
|  970 | AMB_POOR_AREA                   | Box                               |
|  971 | AMB_RICH_AREA                   | Box                               |
|  972 | AMB_RIVER                       | Box                               |
|  973 | AMB_RIVER03                     | Box                               |
|  974 | AMB_RIVER04                     | Box                               |
|  975 | AMB_RIVERDAM                    | Box                               |
|  976 | AMB_RIVER_DOCK                  | Box                               |
|  977 | AMB_SCHOOL_AREA                 | Box                               |
|  978 | AMB_SmallBeachForest            | Box                               |
|  979 | AREA_AROUND_BUTTON              | Box                               |
|  980 | ASYLUM_FRONT_DOOR_R             | Door                              |
|  981 | ASYLUM_FRONT_GATE_DOOR          | Door                              |
|  982 | AcrossGymBack                   | Box                               |
|  983 | AcrossGymBack                   | Box                               |
|  984 | AfterSteam                      | Box                               |
|  985 | AlleyPiss1                      | Box                               |
|  986 | AlleyPiss2                      | Box                               |
|  987 | AlleyPiss3                      | Box                               |
|  988 | Amb_Carnival_Tunnel             | Box                               |
|  989 | Amb_ClassRoom                   | Box                               |
|  990 | Amb_ForestTrainTunnels          | Box                               |
|  991 | Amb_ForestTunnels               | Box                               |
|  992 | Amb_RichAreaCliff               | Box                               |
|  993 | Amb_SchoolRoofTop               | Box                               |
|  994 | Amb_TownHallRoofTop             | Box                               |
|  995 | AmbientEvent1                   | Box                               |
|  996 | AmbientEvent2                   | Box                               |
|  997 | AngelStatue                     | Box                               |
|  998 | AngelStatue                     | Box                               |
|  999 | AniBroom                        | Door                              |
| 1000 | Armor                           | Box                               |
| 1001 | Art_Room                        | Box                               |
| 1002 | AssyInterTone01                 | Box                               |
| 1003 | AssyMain02                      | Box                               |
| 1004 | AssyMainDamaged                 | Box                               |
| 1005 | AssyRecRoom                     | Box                               |
| 1006 | AssyShowers                     | Box                               |
| 1007 | AssylumMain                     | Box                               |
| 1008 | AsyBars                         | Door                              |
| 1009 | AsyBars01                       | Door                              |
| 1010 | AsyBars02                       | Door                              |
| 1011 | AsyDoorB                        | Door                              |
| 1012 | AsyDoors                        | Door                              |
| 1013 | AsyDoors10                      | Door                              |
| 1014 | AsyDoors11                      | Door                              |
| 1015 | AsyDoors12                      | Door                              |
| 1016 | AsyDoors13                      | Door                              |
| 1017 | AsyDoors14                      | Door                              |
| 1018 | AsyDoors15                      | Door                              |
| 1019 | Asylum                          | Box                               |
| 1020 | AsylumPatrols                   | Box                               |
| 1021 | AudioStPinkBankTest             | Box                               |
| 1022 | AudioStereoBankTest             | Box                               |
| 1023 | AudioStereoStreamTest           | Box                               |
| 1024 | AudioSteroPinkStreamTest        | Box                               |
| 1025 | AudioSurrBankTest               | Box                               |
| 1026 | AudioSurrPinkBankTest           | Box                               |
| 1027 | AudioSurrPinkStreamTest         | Box                               |
| 1028 | AudioSurrndStreamTest           | Box                               |
| 1029 | Auditorium                      | Box                               |
| 1030 | AutoGarage                      | Box                               |
| 1031 | AutoGarage                      | Box                               |
| 1032 | AutoShop                        | Box                               |
| 1033 | AutoShop                        | Box                               |
| 1034 | AutoShopSide                    | Box                               |
| 1035 | AutoShopSide                    | Box                               |
| 1036 | BA_BMXGarage                    | Box                               |
| 1037 | BA_DoorStr01                    | Door                              |
| 1038 | BA_DoorStr02                    | Door                              |
| 1039 | BA_DoorStr03                    | Door                              |
| 1040 | BA_DoorStr04                    | Door                              |
| 1041 | BA_DoorStr05                    | Door                              |
| 1042 | BA_DoorStr07                    | Door                              |
| 1043 | BA_DoorStr08                    | Door                              |
| 1044 | BA_PrepDoor02                   | Door                              |
| 1045 | BA_PrepDoor03                   | Door                              |
| 1046 | BA_PrepDoor04                   | Door                              |
| 1047 | BA_PrepDoor05                   | Door                              |
| 1048 | BA_PrepDoor06                   | Door                              |
| 1049 | BA_PrepDoor09                   | Door                              |
| 1050 | BA_PrepDoor10                   | Door                              |
| 1051 | BA_PrepDoor11                   | Door                              |
| 1052 | BBChair                         | Door                              |
| 1053 | BBatter                         | Door                              |
| 1054 | BCatcher                        | Door                              |
| 1055 | BD_Medium1                      | Box                               |
| 1056 | BD_Medium2                      | Box                               |
| 1057 | BDormFlag1                      | Box                               |
| 1058 | BDormFlag1                      | Box                               |
| 1059 | BDormTarg                       | Box                               |
| 1060 | BEACH_AREA_P                    | Box                               |
| 1061 | BMXGate                         | Door                              |
| 1062 | BMXParkJump01                   | Box                               |
| 1063 | BMX_BigRoom                     | Box                               |
| 1064 | BMX_GarageDoor                  | Box                               |
| 1065 | BMX_Room                        | Box                               |
| 1066 | BMX_Warning_Trig                | Box                               |
| 1067 | BNews                           | Door                              |
| 1068 | BSign                           | Door                              |
| 1069 | BTable                          | Door                              |
| 1070 | BUS_SODA_01                     | Box                               |
| 1071 | BUmpire                         | Door                              |
| 1072 | BXPBag                          | Door                              |
| 1073 | BXPBag01                        | Door                              |
| 1074 | BXPBag02                        | Door                              |
| 1075 | BadPlaceTrigger                 | PopulationPed                     |
| 1076 | BalanceBeam                     | Box                               |
| 1077 | BarberShop                      | Box                               |
| 1078 | BarberShop                      | Box                               |
| 1079 | BathroomExit                    | Box                               |
| 1080 | BathroomLeftTrig                | Box                               |
| 1081 | BathroomRightTrig               | Box                               |
| 1082 | BatterEight                     | Box                               |
| 1083 | BatterEight                     | Box                               |
| 1084 | BatterFive                      | Box                               |
| 1085 | BatterFive                      | Box                               |
| 1086 | BatterFour                      | Box                               |
| 1087 | BatterFour                      | Box                               |
| 1088 | BatterNine                      | Box                               |
| 1089 | BatterNine                      | Box                               |
| 1090 | BatterOne                       | Box                               |
| 1091 | BatterOne                       | Box                               |
| 1092 | BatterSeven                     | Box                               |
| 1093 | BatterSeven                     | Box                               |
| 1094 | BatterSix                       | Box                               |
| 1095 | BatterSix                       | Box                               |
| 1096 | BatterThree                     | Box                               |
| 1097 | BatterThree                     | Box                               |
| 1098 | BatterTwo                       | Box                               |
| 1099 | BatterTwo                       | Box                               |
| 1100 | BdrDoorDownstairs1              | Door                              |
| 1101 | BdrDoorDownstairs2              | Door                              |
| 1102 | BdrDoorDownstairs4              | Door                              |
| 1103 | BdrDoorDownstairs5              | Door                              |
| 1104 | BdrDoorDownstairs6              | Door                              |
| 1105 | BdrDoorDownstairs7              | Door                              |
| 1106 | BdrDoorDownstairs8              | Door                              |
| 1107 | BdrDoorL                        | Door                              |
| 1108 | BdrDoorL                        | Door                              |
| 1109 | BdrDoorL01                      | Door                              |
| 1110 | BdrDoorL01                      | Door                              |
| 1111 | BdrDoorL02                      | Door                              |
| 1112 | BdrDoorL02                      | Door                              |
| 1113 | BeachNoGoArea                   | Box                               |
| 1114 | BeatriceCutsceneTrigger         | Box                               |
| 1115 | BeatriceTrigger                 | Box                               |
| 1116 | BellTowerCamera                 | Box                               |
| 1117 | BenchA                          | Door                              |
| 1118 | BenchB                          | Door                              |
| 1119 | BenchC                          | Door                              |
| 1120 | BigTag1                         | Box                               |
| 1121 | BigTag2                         | Box                               |
| 1122 | BigTag3                         | Box                               |
| 1123 | BikeBusiness                    | Box                               |
| 1124 | BikeFire01                      | Box                               |
| 1125 | BikeFire02                      | Box                               |
| 1126 | BikeFire03                      | Box                               |
| 1127 | BikeFire04                      | Box                               |
| 1128 | BikeFire05                      | Box                               |
| 1129 | BikeFire06                      | Box                               |
| 1130 | BikeShop                        | Box                               |
| 1131 | BitchDice                       | Box                               |
| 1132 | BitchFight1                     | Box                               |
| 1133 | BitchFight2                     | Box                               |
| 1134 | BleachersL                      | Box                               |
| 1135 | BleachersL                      | Box                               |
| 1136 | BleachersR                      | Box                               |
| 1137 | BleachersR                      | Box                               |
| 1138 | BonusTarget                     | Box                               |
| 1139 | BottleB                         | Box                               |
| 1140 | BottleC                         | Box                               |
| 1141 | BottleD                         | Box                               |
| 1142 | BottleE                         | Box                               |
| 1143 | Box2ndFloor                     | Box                               |
| 1144 | BoxHalfTheRing                  | Box                               |
| 1145 | BoxMain01                       | Box                               |
| 1146 | BoxMain02                       | Box                               |
| 1147 | BoxRopes                        | Door                              |
| 1148 | BoxStairs                       | Box                               |
| 1149 | BoxingTurfTrigger               | Box                               |
| 1150 | Boxing_Corner1                  | Box                               |
| 1151 | Boxing_Corner2                  | Box                               |
| 1152 | Boxing_Corner3                  | Box                               |
| 1153 | Boxing_Corner4                  | Box                               |
| 1154 | Boxing_Tether                   | Box                               |
| 1155 | Boxtest                         | Box                               |
| 1156 | BoysBathroom1                   | Box                               |
| 1157 | BoysBathroom2                   | Box                               |
| 1158 | BoysDormMain                    | Box                               |
| 1159 | BoysDorm_GameRm                 | Box                               |
| 1160 | BoysDorm_Halls                  | Box                               |
| 1161 | BoysDorm_JimmysRoom             | Box                               |
| 1162 | BuckyCutsceneTrigger            | Box                               |
| 1163 | BuckyTrigger                    | Box                               |
| 1164 | BullyTurf                       | PopulationPed                     |
| 1165 | Burger                          | Box                               |
| 1166 | BusDoors                        | Door                              |
| 1167 | Bus_BUS                         | Box                               |
| 1168 | Bus_Loc1                        | Box                               |
| 1169 | Bus_Loc3                        | Box                               |
| 1170 | Bus_Loc4                        | Box                               |
| 1171 | Bus_Loc5                        | Box                               |
| 1172 | Bus_Loc6                        | Box                               |
| 1173 | Bus_Loc7                        | Box                               |
| 1174 | Bus_Loc8                        | Box                               |
| 1175 | Bus_Loc9                        | Box                               |
| 1176 | Bus_LocX                        | Box                               |
| 1177 | BusinessBike                    | Box                               |
| 1178 | BusinessFirework                | Box                               |
| 1179 | BusinessGrocery                 | Box                               |
| 1180 | C3_MAT_BOUNDARY                 | Box                               |
| 1181 | C5T_POP                         | PopulationPed                     |
| 1182 | C5_PedEvent01                   | Box                               |
| 1183 | C5_PedEvent02                   | Box                               |
| 1184 | C5_PedEvent03                   | Box                               |
| 1185 | C5_WorkingOut1                  | Box                               |
| 1186 | C5_WorkingOut2                  | Box                               |
| 1187 | C5_WorkingOut3                  | Box                               |
| 1188 | C6_ShopBike                     | Box                               |
| 1189 | CARNY_ENTRANCE                  | Box                               |
| 1190 | CARNY_GAMESAREA                 | Box                               |
| 1191 | CARNY_GOKARTAREA                | Box                               |
| 1192 | CHTrespass                      | Box                               |
| 1193 | CafBackTrigger                  | Box                               |
| 1194 | CafTrigger                      | PopulationPed                     |
| 1195 | Carn_Tunnel_Reverb              | Box                               |
| 1196 | Carnival                        | PopulationPed                     |
| 1197 | CatcherFive                     | Box                               |
| 1198 | CatcherFive                     | Box                               |
| 1199 | CatcherFour                     | Box                               |
| 1200 | CatcherFour                     | Box                               |
| 1201 | CatcherOne                      | Box                               |
| 1202 | CatcherOne                      | Box                               |
| 1203 | CatcherSeven                    | Box                               |
| 1204 | CatcherSeven                    | Box                               |
| 1205 | CatcherSix                      | Box                               |
| 1206 | CatcherSix                      | Box                               |
| 1207 | CatcherThree                    | Box                               |
| 1208 | CatcherThree                    | Box                               |
| 1209 | CatcherTwo                      | Box                               |
| 1210 | CatcherTwo                      | Box                               |
| 1211 | CellDoor                        | Door                              |
| 1212 | CellDoor12                      | Door                              |
| 1213 | CellDoor13                      | Door                              |
| 1214 | CellDoor14                      | Door                              |
| 1215 | CellDoor15                      | Door                              |
| 1216 | CellDoor16                      | Door                              |
| 1217 | CellDoor17                      | Door                              |
| 1218 | CellDoor18                      | Door                              |
| 1219 | CellDoor19                      | Door                              |
| 1220 | CellDoor20                      | Door                              |
| 1221 | CellDoor21                      | Door                              |
| 1222 | Cemetary                        | Box                               |
| 1223 | Chair1                          | Box                               |
| 1224 | Chair2                          | Box                               |
| 1225 | ChangeRoom                      | Box                               |
| 1226 | CheerleadersTrigger             | Box                               |
| 1227 | ChemPlantAcid01                 | Box                               |
| 1228 | ChemPlantLower                  | Box                               |
| 1229 | ChemPlantMain                   | Box                               |
| 1230 | ChemPlantStairTunnel            | Box                               |
| 1231 | Chemical_Plant_Roof             | Box                               |
| 1232 | ChezLouis                       | Door                              |
| 1233 | ChristmasTreeExclude            | Box                               |
| 1234 | CityHall                        | Box                               |
| 1235 | CityHallTarg                    | Box                               |
| 1236 | Coaster                         | Door                              |
| 1237 | CoasterExitTrigger              | Box                               |
| 1238 | ComicBedExclude                 | Box                               |
| 1239 | ComicPopTrig                    | PopulationPed                     |
| 1240 | ComicShop                       | Box                               |
| 1241 | ComicShopExclude                | Box                               |
| 1242 | CopCar                          | Box                               |
| 1243 | Corner_Check1                   | Box                               |
| 1244 | Corner_Check3                   | Box                               |
| 1245 | CrateBrk                        | Door                              |
| 1246 | Cutscene02                      | Box                               |
| 1247 | DISABLED_SV_LibMain             | Box                               |
| 1248 | DRBrace                         | Door                              |
| 1249 | DRBrace01                       | Door                              |
| 1250 | DRPDoor                         | Door                              |
| 1251 | DRPDoor01                       | Door                              |
| 1252 | DT_ASYLUM_BACK_EXIT             | Box                               |
| 1253 | DT_ASYLUM_EXITL                 | Door                              |
| 1254 | DT_ASYLUM_FRONT_DOOR            | Box                               |
| 1255 | DT_ASYLUM_SIDE_EXIT             | Door                              |
| 1256 | DT_BMXGarage                    | Box                               |
| 1257 | DT_BMXGarageDoor                | Box                               |
| 1258 | DT_CarnCurt01                   | Box                               |
| 1259 | DT_CarnCurt02                   | Box                               |
| 1260 | DT_ChemPlant_DoorL              | Box                               |
| 1261 | DT_ComicShop                    | PopulationPed                     |
| 1262 | DT_DormExitDoorL                | Door                              |
| 1263 | DT_DropOutAlley                 | PopulationPed                     |
| 1264 | DT_FreakEntrance                | Door                              |
| 1265 | DT_FreakExit                    | Door                              |
| 1266 | DT_FreakShow_Entrance           | Box                               |
| 1267 | DT_FreakShow_Exit               | Box                               |
| 1268 | DT_FunhouseTheaterCarnival      | Door                              |
| 1269 | DT_GASSTATION                   | PopulationPed                     |
| 1270 | DT_GreaserAlley                 | PopulationPed                     |
| 1271 | DT_ISCHOOL_BIO                  | Door                              |
| 1272 | DT_ISCHOOL_CHEM                 | Door                              |
| 1273 | DT_Janitor_MainExit             | Box                               |
| 1274 | DT_Janitor_SchoolExit           | Box                               |
| 1275 | DT_LibraryExitR                 | Door                              |
| 1276 | DT_Medium_001                   | Box                               |
| 1277 | DT_Medium_002                   | Box                               |
| 1278 | DT_Medium_003                   | Box                               |
| 1279 | DT_Medium_004                   | Box                               |
| 1280 | DT_Medium_005                   | Box                               |
| 1281 | DT_Medium_006                   | Box                               |
| 1282 | DT_Medium_007                   | Box                               |
| 1283 | DT_Medium_008                   | Box                               |
| 1284 | DT_Medium_009                   | Box                               |
| 1285 | DT_Medium_010                   | Box                               |
| 1286 | DT_Medium_011                   | Box                               |
| 1287 | DT_Medium_012                   | Box                               |
| 1288 | DT_Medium_013                   | Box                               |
| 1289 | DT_Medium_014                   | Box                               |
| 1290 | DT_Medium_015                   | Box                               |
| 1291 | DT_Medium_016                   | Box                               |
| 1292 | DT_Medium_017                   | Box                               |
| 1293 | DT_Medium_019                   | Box                               |
| 1294 | DT_Medium_020                   | Box                               |
| 1295 | DT_Medium_021                   | Box                               |
| 1296 | DT_Medium_022                   | Box                               |
| 1297 | DT_Medium_023                   | Box                               |
| 1298 | DT_Medium_024                   | Box                               |
| 1299 | DT_Medium_025                   | Box                               |
| 1300 | DT_Observatory                  | Door                              |
| 1301 | DT_PrepToMain                   | Box                               |
| 1302 | DT_SpawnTest3                   | Box                               |
| 1303 | DT_TINDUST_CHEMEX_DOOR          | Door                              |
| 1304 | DT_Tenement_Window              | Box                               |
| 1305 | DT_auditorium_doorL             | Box                               |
| 1306 | DT_autoshop_doorL               | Box                               |
| 1307 | DT_barber_exit                  | Box                               |
| 1308 | DT_classr_doorL                 | Box                               |
| 1309 | DT_gdorm_DoorLExit              | Box                               |
| 1310 | DT_gdorm_doorL                  | Box                               |
| 1311 | DT_gym_doorL                    | Box                               |
| 1312 | DT_iSafeDrop_DoorL              | Door                              |
| 1313 | DT_iSafeGrsr_DoorL              | Door                              |
| 1314 | DT_iSafeJock_DoorL              | Door                              |
| 1315 | DT_iSafeNerd_DoorL              | Door                              |
| 1316 | DT_iSafePrep_DoorL              | Door                              |
| 1317 | DT_ibkshop_Door                 | Door                              |
| 1318 | DT_iboxing_DoorL                | Box                               |
| 1319 | DT_iclothp_doorL                | Door                              |
| 1320 | DT_iclothr_DoorL                | Door                              |
| 1321 | DT_icomshp_Basement             | Door                              |
| 1322 | DT_icomshp_Door                 | Door                              |
| 1323 | DT_ifunhous_FMDoor              | Door                              |
| 1324 | DT_ifunhous_FMDoorA             | Box                               |
| 1325 | DT_igrocery_Door                | Door                              |
| 1326 | DT_indoor_TattooShop            | Door                              |
| 1327 | DT_indoor_whouseFront           | Door                              |
| 1328 | DT_indoor_whouseRoof            | Door                              |
| 1329 | DT_ischool_Art                  | Door                              |
| 1330 | DT_ischool_AuditorBalc          | Door                              |
| 1331 | DT_ischool_AuditorDoorL         | Door                              |
| 1332 | DT_ischool_BackDoorLeft         | Door                              |
| 1333 | DT_ischool_BackDoorRight        | Door                              |
| 1334 | DT_ischool_Classroom            | Door                              |
| 1335 | DT_ischool_Door01               | Door                              |
| 1336 | DT_ischool_FrontDoorL           | Door                              |
| 1337 | DT_ischool_FrontDoorRight       | Door                              |
| 1338 | DT_ischool_HallWind             | Door                              |
| 1339 | DT_ischool_Janitor              | Door                              |
| 1340 | DT_ischool_RoofDoor             | Door                              |
| 1341 | DT_ischool_Staff                | Door                              |
| 1342 | DT_observatory_doorL            | Door                              |
| 1343 | DT_phair_doorL                  | Box                               |
| 1344 | DT_pool_doorL                   | Box                               |
| 1345 | DT_salon_exit                   | Box                               |
| 1346 | DT_staff_doorL                  | Box                               |
| 1347 | DT_tBMX_enter                   | Door                              |
| 1348 | DT_tBMX_leave                   | Door                              |
| 1349 | DT_tbusines_BikeShopDoor        | Door                              |
| 1350 | DT_tbusines_ClothDoor           | Door                              |
| 1351 | DT_tbusines_ComicShopDoor       | Door                              |
| 1352 | DT_tbusines_FirewShopDoor       | Door                              |
| 1353 | DT_tbusines_GenShop1Door        | Door                              |
| 1354 | DT_tbusines_GenShop2Door        | Door                              |
| 1355 | DT_tbusines_SafeNerd            | Door                              |
| 1356 | DT_tbusiness_FirewBusDoor       | Door                              |
| 1357 | DT_tbusiness_Recorddoor         | Door                              |
| 1358 | DT_tbusiness_barber             | Door                              |
| 1359 | DT_tind_SafeDrop                | Door                              |
| 1360 | DT_tpoor_BMX                    | Door                              |
| 1361 | DT_tpoor_Barber                 | Box                               |
| 1362 | DT_tpoor_SafeGreaser            | Door                              |
| 1363 | DT_tpoor_tenwindow              | Door                              |
| 1364 | DT_trich_BarberDoor             | Door                              |
| 1365 | DT_trich_BikeShopDoor           | Door                              |
| 1366 | DT_trich_BoxingDoor01           | Box                               |
| 1367 | DT_trich_BoxingDoor02           | Door                              |
| 1368 | DT_trich_ClothRichDoor          | Door                              |
| 1369 | DT_trich_FirewShopDoor          | Door                              |
| 1370 | DT_trich_GenShopDoor            | Door                              |
| 1371 | DT_trich_SafePrep               | Door                              |
| 1372 | DT_tschool_AutoShopL            | Door                              |
| 1373 | DT_tschool_BoysDormL            | Door                              |
| 1374 | DT_tschool_ExtWind              | Door                              |
| 1375 | DT_tschool_GirlsDormL           | Door                              |
| 1376 | DT_tschool_GirlsDormSideL       | Door                              |
| 1377 | DT_tschool_GymL                 | Door                              |
| 1378 | DT_tschool_LibraryL             | Door                              |
| 1379 | DT_tschool_PoolL                | Door                              |
| 1380 | DT_tschool_PreppyL              | Door                              |
| 1381 | DT_tschool_RoofDoor             | Door                              |
| 1382 | DT_tschool_SafeJock             | Door                              |
| 1383 | DT_tschool_SchoolFrontDoorL     | Door                              |
| 1384 | DT_tschool_SchoolLeftBackDoor   | Door                              |
| 1385 | DT_tschool_SchoolRightBackDoor  | Door                              |
| 1386 | DT_tschool_SchoolRightFrontDoor | Door                              |
| 1387 | DT_tschool_SchoolSideDoorL      | Door                              |
| 1388 | DT_whouse_front                 | Box                               |
| 1389 | DT_whouse_roof                  | Box                               |
| 1390 | DePopBeachAreaRace              | PopulationPed                     |
| 1391 | DePopIndustrialAreaRace         | PopulationPed                     |
| 1392 | DePopRichAreaRace               | PopulationPed                     |
| 1393 | Disabled_SV_AutoMain            | Box                               |
| 1394 | Disabled_SV_BoxingRich          | Box                               |
| 1395 | Disabled_SV_ClothMain           | Box                               |
| 1396 | Disabled_SV_EnglishSchool       | Box                               |
| 1397 | Disabled_SV_GymMain             | Box                               |
| 1398 | Disabled_SV_PrincipalSchool     | Box                               |
| 1399 | Disabled_SV_Staff               | Box                               |
| 1400 | Door_PrepHouse_Foyer            | Door                              |
| 1401 | Door_PrepHouse_FoyerOut         | Door                              |
| 1402 | Door_PrepHouse_Gamble           | Door                              |
| 1403 | Door_PrepHouse_Lounge           | Door                              |
| 1404 | Door_PrepHouse_Lounge_02        | Door                              |
| 1405 | Door_PrepHouse_Stairs           | Door                              |
| 1406 | Door_PrepHouse_Stairs_Lower     | Door                              |
| 1407 | Door_PrepHouse_Stairs_Upper     | Door                              |
| 1408 | DormChemistrySet                | Box                               |
| 1409 | DormDoorTrig1                   | Box                               |
| 1410 | DormDoorTrig2                   | Box                               |
| 1411 | DormDoorTrig3                   | Box                               |
| 1412 | DormDoorTrig4                   | Box                               |
| 1413 | DormExitDoorR                   | Door                              |
| 1414 | DormTVTrig                      | Box                               |
| 1415 | DownTown                        | PopulationPed + PopulationVehicle |
| 1416 | DowntownGameArea                | Box                               |
| 1417 | Dumpster                        | Box                               |
| 1418 | DunkBackBoard                   | Box                               |
| 1419 | DunkBttn                        | Door                              |
| 1420 | DunkSeat                        | Door                              |
| 1421 | DunkTank                        | Box                               |
| 1422 | DunkTankExcluder                | Box                               |
| 1423 | ESCDoorL                        | Door                              |
| 1424 | ESCDoorL                        | Door                              |
| 1425 | ESCDoorL04                      | Door                              |
| 1426 | ESCDoorL05                      | Door                              |
| 1427 | ESCDoorL05                      | Door                              |
| 1428 | ESCDoorL06                      | Door                              |
| 1429 | ESCDoorR                        | Door                              |
| 1430 | ESCDoorR                        | Door                              |
| 1431 | ESCDoorR05                      | Door                              |
| 1432 | EVENING_MUSIC_TRIGGER           | Box                               |
| 1433 | EasyDrugs_Trash01               | Box                               |
| 1434 | EasyDrugs_Trash02               | Box                               |
| 1435 | EasyDrugs_Trash03               | Box                               |
| 1436 | EasyDrugs_Trash04               | Box                               |
| 1437 | EasyDrugs_Trash05               | Box                               |
| 1438 | EasyDrugs_Trash06               | Box                               |
| 1439 | EggBDorm                        | Box                               |
| 1440 | EggGDorm                        | Box                               |
| 1441 | EntryToWondMeat                 | Box                               |
| 1442 | EquipmentRoom                   | Box                               |
| 1443 | EquipmentRoom                   | Box                               |
| 1444 | ExitFerrisTrigger               | Box                               |
| 1445 | ExitToWondMeat                  | Box                               |
| 1446 | FMDoor                          | Door                              |
| 1447 | FMDoor                          | Door                              |
| 1448 | FMDoor01                        | Door                              |
| 1449 | FMDoor01N                       | Door                              |
| 1450 | FMDoor02                        | Door                              |
| 1451 | FMDoor03                        | Door                              |
| 1452 | FMDoor04                        | Door                              |
| 1453 | FMDoor05                        | Door                              |
| 1454 | FMDoor06                        | Door                              |
| 1455 | FMDoor07                        | Door                              |
| 1456 | FMDoor08                        | Door                              |
| 1457 | FMDoorN                         | Door                              |
| 1458 | FMDoorN01                       | Door                              |
| 1459 | FRAFFY                          | Box                               |
| 1460 | FUNHOUSE_CURTAIN_OPEN           | Box                               |
| 1461 | FUNHOUSE_GRAVECONTROL           | Box                               |
| 1462 | FUNHOUSE_GRAVES                 | Box                               |
| 1463 | FUNHOUSE_GRAVEYARD              | Box                               |
| 1464 | FUNHOUSE_GRAVE_TO_MAZE_TRANS    | Box                               |
| 1465 | FUNHOUSE_MAZE                   | Box                               |
| 1466 | FUNHOUSE_MAZE_TO_GRAVE_TRANS    | Box                               |
| 1467 | FUNHOUSE_MINE                   | Box                               |
| 1468 | FUNHOUSE_MINE_ROCKS             | Box                               |
| 1469 | FUNHOUSE_MINE_STEAM_01          | Box                               |
| 1470 | FUNHOUSE_MINE_STEAM_02          | Box                               |
| 1471 | FUNHOUSE_MINE_STEAM_03          | Box                               |
| 1472 | FUNHOUSE_PILLOW_ROOM            | Box                               |
| 1473 | FUNHOUSE_P_TO_G_TRANS           | Box                               |
| 1474 | FUNHOUSE_SCAFFOLD               | Box                               |
| 1475 | FUNHOUSE_UPSIDEDOWN_ROOM        | Box                               |
| 1476 | FUNHOUSE_U_TO_G_TRANS           | Box                               |
| 1477 | FUNHOUSE_VORTEX_ENTRANCE        | Box                               |
| 1478 | FactoryEntrance                 | Box                               |
| 1479 | Ferris                          | Door                              |
| 1480 | FieldOverride                   | PopulationPed                     |
| 1481 | FightingArea                    | Box                               |
| 1482 | FinalFightTrig                  | Box                               |
| 1483 | FinalPosCheck                   | Box                               |
| 1484 | FireworkBusiness                | Box                               |
| 1485 | FlagLeftSchool                  | Box                               |
| 1486 | FlagLeftSchool                  | Box                               |
| 1487 | FlagRightSchool                 | Box                               |
| 1488 | FlagRightSchool                 | Box                               |
| 1489 | Flea                            | Box                               |
| 1490 | FootFieldTrig                   | Box                               |
| 1491 | FootballField                   | Box                               |
| 1492 | FootballFieldEntrance           | Box                               |
| 1493 | Forest                          | Box                               |
| 1494 | FortuneTeller                   | Box                               |
| 1495 | FountainCutscene                | Box                               |
| 1496 | FreakShow_AmbEnter              | Box                               |
| 1497 | FreakShow_AmbExit               | Box                               |
| 1498 | FreakShow_Errie01               | Box                               |
| 1499 | FreakShow_Errie02               | Box                               |
| 1500 | FreakShow_MidgetFight           | Box                               |
| 1501 | FreakShow_Midgets               | Box                               |
| 1502 | FunTeeth                        | Door                              |
| 1503 | Funhouse_Auditorium             | Box                               |
| 1504 | Funhouse_ControlRm_Graveyard    | Box                               |
| 1505 | Funhouse_HauntedMaze            | Box                               |
| 1506 | Funhouse_MineShaft              | Box                               |
| 1507 | Funhouse_Sound_Graveyard        | Box                               |
| 1508 | Funhouse_Tounge                 | Box                               |
| 1509 | Funhouse_UpsideDown             | Box                               |
| 1510 | Funhouse_Vortex                 | Box                               |
| 1511 | Funhouse_Whackamole             | Box                               |
| 1512 | GC1A_GameArea                   | PopulationPed                     |
| 1513 | GDormBackDr                     | Box                               |
| 1514 | GDormBackDr                     | Box                               |
| 1515 | GDormEntrance                   | Box                               |
| 1516 | GDormEntrance                   | Box                               |
| 1517 | GDormExitExclude                | Box                               |
| 1518 | GDormTarg                       | Box                               |
| 1519 | GDorm_GirlsOnly                 | PopulationPed                     |
| 1520 | GDorm_PopOverride               | PopulationPed                     |
| 1521 | GDorm_Stall01                   | Box                               |
| 1522 | GDorm_Stall02                   | Box                               |
| 1523 | GDorm_UpperDoor                 | Box                               |
| 1524 | GDorm_UpperDoorStorage          | Box                               |
| 1525 | GREASERS_JET01                  | Box                               |
| 1526 | GREASERS_JET02                  | Box                               |
| 1527 | GREASERS_JET03                  | Box                               |
| 1528 | GREASERS_JET04                  | Box                               |
| 1529 | GREASERS_JET05                  | Box                               |
| 1530 | GarageRoofTrig                  | Box                               |
| 1531 | GarageTrig                      | Box                               |
| 1532 | Garage_BusinessArea             | Box                               |
| 1533 | Garage_PoorArea                 | Box                               |
| 1534 | Garage_RichArea                 | Box                               |
| 1535 | Garage_SchoolGrounds            | Box                               |
| 1536 | GarbCanA                        | Door                              |
| 1537 | GaryTrigger                     | Box                               |
| 1538 | GasSign                         | Door                              |
| 1539 | GasStop1                        | Box                               |
| 1540 | GasStop2                        | Box                               |
| 1541 | GirlsBathroom1                  | Box                               |
| 1542 | GirlsBathroom2                  | Box                               |
| 1543 | GirlsDormTrig                   | Box                               |
| 1544 | GirlsDorm_Attic                 | Box                               |
| 1545 | GirlsTrig                       | Box                               |
| 1546 | GlassDome                       | Box                               |
| 1547 | GlassDome                       | Box                               |
| 1548 | GnomeB                          | Box                               |
| 1549 | GnomeD                          | Box                               |
| 1550 | GoKartTrack_Amb                 | Box                               |
| 1551 | GordYell                        | Box                               |
| 1552 | GraveYard                       | PopulationPed                     |
| 1553 | GreaserBathroom                 | Box                               |
| 1554 | GreaserMainRoom                 | Box                               |
| 1555 | GreaserTag                      | Box                               |
| 1556 | GreaserTagArea                  | Box                               |
| 1557 | Greasers                        | PopulationPed                     |
| 1558 | GroceryBusiness                 | Box                               |
| 1559 | GroceryStore                    | Box                               |
| 1560 | GymPoolHall                     | Box                               |
| 1561 | GymPool_PopOverride             | PopulationPed                     |
| 1562 | Gym_BoysChange                  | Box                               |
| 1563 | Gym_GirlsChange                 | Box                               |
| 1564 | Gym_Main                        | Box                               |
| 1565 | Gym_Pool01                      | Box                               |
| 1566 | Gym_Pool02                      | Box                               |
| 1567 | Gymnasium                       | Box                               |
| 1568 | Gymnasium                       | Box                               |
| 1569 | GymnasiumBack                   | Box                               |
| 1570 | GymnasiumBack                   | Box                               |
| 1571 | HSdinger                        | Door                              |
| 1572 | HairPoorRm01                    | Box                               |
| 1573 | HairPoorRm02                    | Box                               |
| 1574 | HallsPopTrigger                 | Box                               |
| 1575 | HarringtonTrig                  | Box                               |
| 1576 | HattrickDoor                    | Door                              |
| 1577 | Hattrick_gate                   | Door                              |
| 1578 | HighGround                      | Box                               |
| 1579 | HighStrikerExcluder             | Box                               |
| 1580 | HoboTrigger                     | Box                               |
| 1581 | HouseThirdFloor                 | Box                               |
| 1582 | IA_medium01                     | Box                               |
| 1583 | IA_medium02                     | Box                               |
| 1584 | IA_medium03                     | Box                               |
| 1585 | IA_medium04                     | Box                               |
| 1586 | IA_medium05                     | Box                               |
| 1587 | IA_medium06                     | Box                               |
| 1588 | IA_medium07                     | Box                               |
| 1589 | IBOXING_SWEATER_TRIG            | Box                               |
| 1590 | INPOOLAREA                      | Box                               |
| 1591 | Incin                           | Box                               |
| 1592 | Ind_DoorStr02                   | Door                              |
| 1593 | Ind_DoorStr1                    | Door                              |
| 1594 | Ind_MedicalDoor                 | Door                              |
| 1595 | Ind_PoliceDoor                  | Door                              |
| 1596 | Ind_SpazMeats                   | Box                               |
| 1597 | IndustrialArea_DropOutEnclave   | PopulationPed + PopulationVehicle |
| 1598 | IndustrialBarricade             | Box                               |
| 1599 | IndustrialGates                 | Box                               |
| 1600 | IndustrialNoGoArea              | Box                               |
| 1601 | Industrial_Docks                | PopulationPed                     |
| 1602 | Industrial_Sawmill              | PopulationPed                     |
| 1603 | InstBatter                      | Box                               |
| 1604 | InstCatcher                     | Box                               |
| 1605 | InstUmpire                      | Box                               |
| 1606 | JOHNNYONTHESPOT                 | Box                               |
| 1607 | JainitorsRoom                   | Box                               |
| 1608 | JanDoor02                       | Door                              |
| 1609 | JanDoors00                      | Door                              |
| 1610 | JanDoors01                      | Door                              |
| 1611 | JanDoors02                      | Door                              |
| 1612 | JanDoors03b                     | Door                              |
| 1613 | JanElectricProxy                | Box                               |
| 1614 | JanExtraFire                    | Box                               |
| 1615 | JanFire01                       | Box                               |
| 1616 | JanFire02                       | Box                               |
| 1617 | JanSteamProxy                   | Box                               |
| 1618 | JanSwtch00                      | Door                              |
| 1619 | JanSwtch01                      | Door                              |
| 1620 | JanSwtch02                      | Door                              |
| 1621 | JanSwtch03a                     | Door                              |
| 1622 | JockHideOut                     | Box                               |
| 1623 | Jocks                           | PopulationPed                     |
| 1624 | Jocks_FootballField             | PopulationPed                     |
| 1625 | JohnnyRamble02                  | Box                               |
| 1626 | LM1_GameArea                    | Box                               |
| 1627 | LM2_GameArea                    | Box                               |
| 1628 | LM3_Depop                       | PopulationPed                     |
| 1629 | LM3_GameArea                    | Box                               |
| 1630 | LM4_GameArea                    | Box                               |
| 1631 | LM5_GameArea                    | Box                               |
| 1632 | LackeySetA                      | Box                               |
| 1633 | LackeySetB                      | Box                               |
| 1634 | LackeySetC                      | Box                               |
| 1635 | LackeySetD                      | Box                               |
| 1636 | LackeySetE                      | Box                               |
| 1637 | LawnMowerTrigger                | Box                               |
| 1638 | LckrGymA01                      | Door                              |
| 1639 | LckrGymA02                      | Door                              |
| 1640 | LckrGymA03                      | Door                              |
| 1641 | LckrGymB                        | Door                              |
| 1642 | LckrGymB01                      | Door                              |
| 1643 | LckrGymB02                      | Door                              |
| 1644 | LckrGymB03                      | Door                              |
| 1645 | LckrGymM                        | Door                              |
| 1646 | LibTarg                         | Box                               |
| 1647 | LibTrig                         | Box                               |
| 1648 | LibraryArch                     | Box                               |
| 1649 | LibraryArch                     | Box                               |
| 1650 | LibraryL                        | Box                               |
| 1651 | LibraryL                        | Box                               |
| 1652 | LibraryR                        | Box                               |
| 1653 | LibraryR                        | Box                               |
| 1654 | Library_Inner                   | Box                               |
| 1655 | Library_Outer                   | Box                               |
| 1656 | Library_Tunnels                 | Box                               |
| 1657 | LifeGrd                         | Door                              |
| 1658 | LockerTest                      | Box                               |
| 1659 | LowCorona                       | Box                               |
| 1660 | LunchLadyTrigger                | Box                               |
| 1661 | MGL2_01_GameArea                | Box                               |
| 1662 | MGL2_02_GameArea                | Box                               |
| 1663 | MGL2_03_GameArea                | Box                               |
| 1664 | MGL2_04_GameArea                | Box                               |
| 1665 | MGL2_05_GameArea                | Box                               |
| 1666 | MGS2_Bonus01                    | Box                               |
| 1667 | MGS2_Bottle01                   | Box                               |
| 1668 | MGS2_Bottle02                   | Box                               |
| 1669 | MGS2_Bottle03                   | Box                               |
| 1670 | MGS2_Bottle04                   | Box                               |
| 1671 | MGS2_Bottle05                   | Box                               |
| 1672 | MGS2_Bottle06                   | Box                               |
| 1673 | MGS2_Bottle07                   | Box                               |
| 1674 | MGS2_Bottle08                   | Box                               |
| 1675 | MGS2_Cowboy01                   | Box                               |
| 1676 | MGS2_Cowboy02                   | Box                               |
| 1677 | MGS2_Cowboy03                   | Box                               |
| 1678 | MGS2_Cowboy04                   | Box                               |
| 1679 | MGS2_Robber01                   | Box                               |
| 1680 | MGS2_Robber02                   | Box                               |
| 1681 | MGS2_Robber03                   | Box                               |
| 1682 | MGS2_Robber04                   | Box                               |
| 1683 | MGS2_TutBottle                  | Box                               |
| 1684 | MGS2_TutCowboy                  | Box                               |
| 1685 | MGS2_TutRobber                  | Box                               |
| 1686 | MGS_Bonus01                     | Box                               |
| 1687 | MGS_Bottle01                    | Box                               |
| 1688 | MGS_Bottle02                    | Box                               |
| 1689 | MGS_Bottle03                    | Box                               |
| 1690 | MGS_Bottle04                    | Box                               |
| 1691 | MGS_Bottle05                    | Box                               |
| 1692 | MGS_Bottle06                    | Box                               |
| 1693 | MGS_Bottle07                    | Box                               |
| 1694 | MGS_Bottle08                    | Box                               |
| 1695 | MGS_Cowboy01                    | Box                               |
| 1696 | MGS_Cowboy02                    | Box                               |
| 1697 | MGS_Cowboy03                    | Box                               |
| 1698 | MGS_Cowboy04                    | Box                               |
| 1699 | MGS_Robber01                    | Box                               |
| 1700 | MGS_Robber02                    | Box                               |
| 1701 | MGS_Robber03                    | Box                               |
| 1702 | MGS_Robber04                    | Box                               |
| 1703 | MGS_TutBottle                   | Box                               |
| 1704 | MGS_TutCowboy                   | Box                               |
| 1705 | MGS_TutRobber                   | Box                               |
| 1706 | MailmanTrigger                  | Box                               |
| 1707 | MainAuto                        | Box                               |
| 1708 | MainBoysDorm                    | Box                               |
| 1709 | MainGym                         | Box                               |
| 1710 | MainPrep                        | Box                               |
| 1711 | MainSchool                      | Box                               |
| 1712 | ManicCopCar                     | Box                               |
| 1713 | MeatPlant_boltcutters_FDoorC01  | Door                              |
| 1714 | MeatPlant_hide_FDoorC02         | Door                              |
| 1715 | MeatPlant_hide_FDoorC03         | Door                              |
| 1716 | Midway_ShootGallery             | Box                               |
| 1717 | Mourge                          | Box                               |
| 1718 | NLock01A                        | Door                              |
| 1719 | NLock01A                        | Door                              |
| 1720 | NLock01A01                      | Door                              |
| 1721 | NLock01A02                      | Door                              |
| 1722 | NLock01B                        | Door                              |
| 1723 | NLock01B01                      | Door                              |
| 1724 | NLock01B02                      | Door                              |
| 1725 | NLock01B04                      | Box                               |
| 1726 | NLock01B05                      | Box                               |
| 1727 | NLock01B06                      | Box                               |
| 1728 | NLock01B07                      | Box                               |
| 1729 | NLock02A                        | Door                              |
| 1730 | NLock02A01                      | Door                              |
| 1731 | NLock02A02                      | Door                              |
| 1732 | NLock02A03                      | Door                              |
| 1733 | NLock02B                        | Door                              |
| 1734 | NLock02B01                      | Door                              |
| 1735 | NLock02B02                      | Door                              |
| 1736 | NLock02B03                      | Door                              |
| 1737 | NLock02B04                      | Door                              |
| 1738 | NLock02B05                      | Door                              |
| 1739 | NLock02B06                      | Door                              |
| 1740 | NLock02B07                      | Door                              |
| 1741 | NLock02B08                      | Box                               |
| 1742 | NLock02B09                      | Box                               |
| 1743 | NLock02B10                      | Box                               |
| 1744 | NLock03B                        | Door                              |
| 1745 | NerdComputerRoom                | Box                               |
| 1746 | NerdComputerRoom                | Box                               |
| 1747 | NerdEncounter                   | Box                               |
| 1748 | NerdMainRoom                    | Box                               |
| 1749 | NerdMainRoom                    | Box                               |
| 1750 | NerdPath_AsySwtch               | Door                              |
| 1751 | NerdPath_AsySwtch02             | Box                               |
| 1752 | NerdPath_BRDoor                 | Door                              |
| 1753 | NerdSmallRoom                   | Box                               |
| 1754 | NerdStairwell                   | Box                               |
| 1755 | NerdStairwell                   | Box                               |
| 1756 | Nerds                           | PopulationPed                     |
| 1757 | New_Gate                        | Box                               |
| 1758 | NursingPond                     | Box                               |
| 1759 | Observatory_Amb                 | Box                               |
| 1760 | OutsideSchool1                  | PopulationPed                     |
| 1761 | PAlleyPiss1                     | Box                               |
| 1762 | PAlleyPiss2                     | Box                               |
| 1763 | PAlleyPiss3                     | Box                               |
| 1764 | PAlleyPiss4                     | Box                               |
| 1765 | PAn_Prep_Armor01                | Box                               |
| 1766 | PAn_Prep_Armor02                | Box                               |
| 1767 | PAn_Prep_Armor03                | Box                               |
| 1768 | PAn_Prep_Armor04                | Box                               |
| 1769 | PAn_Prep_Armor05                | Box                               |
| 1770 | PAn_Prep_Armor06                | Box                               |
| 1771 | PAn_Prep_ESCDoorR               | Door                              |
| 1772 | PAn_Prep_Weed                   | Box                               |
| 1773 | PAnim_FlyTrap                   | Box                               |
| 1774 | PETEYPIER                       | Box                               |
| 1775 | PLAYER_ROOM                     | Box                               |
| 1776 | POORAREA_SODA_01                | Box                               |
| 1777 | POOR_TENEMENTS                  | PopulationPed                     |
| 1778 | PO_House                        | Box                               |
| 1779 | POfficeExclude                  | Box                               |
| 1780 | PREPHOUSE_PLANTAREA             | Box                               |
| 1781 | PR_CarStart01                   | Box                               |
| 1782 | PR_CarStart02                   | Box                               |
| 1783 | PR_CarStart03                   | Box                               |
| 1784 | PR_CarStart04                   | Box                               |
| 1785 | PR_CarStart05                   | Box                               |
| 1786 | PR_CheckEquip                   | Box                               |
| 1787 | PR_DogStart00                   | Box                               |
| 1788 | PR_DogStart01                   | Box                               |
| 1789 | PR_DogStart02                   | Box                               |
| 1790 | PR_DogStart03                   | Box                               |
| 1791 | PR_DogStart04                   | Box                               |
| 1792 | PR_HattrickYard                 | Box                               |
| 1793 | PR_HillTop                      | Box                               |
| 1794 | PR_JoggerTrigger                | Box                               |
| 1795 | PR_MailManStart01               | Box                               |
| 1796 | PR_MailManStart02               | Box                               |
| 1797 | PR_MailManStart03               | Box                               |
| 1798 | PR_OldLadyNorthStart            | Box                               |
| 1799 | PR_OldLadySouthStart            | Box                               |
| 1800 | PR_PaperPickupTrigger           | Box                               |
| 1801 | PSecretary                      | Box                               |
| 1802 | PTrig                           | Box                               |
| 1803 | PUN_BDORM                       | Box                               |
| 1804 | PUN_GDORM                       | Box                               |
| 1805 | PaperRoute_Excluder             | Box                               |
| 1806 | ParkingArchway                  | Box                               |
| 1807 | ParkingArchway                  | Box                               |
| 1808 | Picnic                          | Door                              |
| 1809 | PokerTbl                        | Door                              |
| 1810 | PoorArea                        | PopulationPed + PopulationVehicle |
| 1811 | PoorArea_Medium_001             | Box                               |
| 1812 | PoorArea_Medium_002             | Box                               |
| 1813 | PoorArea_Medium_004             | Box                               |
| 1814 | PoorArea_Medium_005             | Box                               |
| 1815 | PoorArea_Medium_006             | Box                               |
| 1816 | PoorArea_Medium_007             | Box                               |
| 1817 | PoorArea_Medium_008             | Box                               |
| 1818 | PoorArea_Medium_009             | Box                               |
| 1819 | PoorArea_Medium_010             | Box                               |
| 1820 | PoorArea_Medium_013             | Box                               |
| 1821 | PoorArea_Medium_014             | Box                               |
| 1822 | PoorArea_Medium_015             | Box                               |
| 1823 | PoorArea_Medium_016             | Box                               |
| 1824 | PoorArea_Medium_017             | Box                               |
| 1825 | PoorArea_Medium_018             | Box                               |
| 1826 | PoorArea_Medium_019             | Box                               |
| 1827 | PoorArea_Medium_020             | Box                               |
| 1828 | PoorArea_Medium_021             | Box                               |
| 1829 | PoorArea_Medium_022             | Box                               |
| 1830 | PoorArea_Medium_023             | Box                               |
| 1831 | PoorArea_Medium_024             | Box                               |
| 1832 | PoorArea_Medium_025             | Box                               |
| 1833 | PoorArea_Medium_026             | Box                               |
| 1834 | PoorArea_Medium_027             | Box                               |
| 1835 | PoorArea_Medium_028             | Box                               |
| 1836 | PoorArea_Medium_029             | Box                               |
| 1837 | PoorArea_Medium_030             | Box                               |
| 1838 | PoorBarricade                   | Box                               |
| 1839 | PoorClothing_Change             | Box                               |
| 1840 | PoorClothing_Main               | Box                               |
| 1841 | PoorDepop                       | PopulationPed                     |
| 1842 | PoorGameArea                    | Box                               |
| 1843 | PoorTarg1                       | Box                               |
| 1844 | PoorTarg2                       | Box                               |
| 1845 | PoorTrainTunnel                 | Box                               |
| 1846 | Poor_DropTurf1                  | PopulationPed                     |
| 1847 | PopRoads1                       | PopulationPed + PopulationVehicle |
| 1848 | PortaPoo                        | Box                               |
| 1849 | PowerStationTrig                | Box                               |
| 1850 | Powerplant_Sequrity             | Box                               |
| 1851 | Pr_HilltopExcluder              | Box                               |
| 1852 | PrepHouse_Atrium                | Box                               |
| 1853 | PrepHouse_Entrance              | Box                               |
| 1854 | PrepHouse_Main2nd               | Box                               |
| 1855 | PrepHouse_MainRoom              | Box                               |
| 1856 | PrephouseExterior               | Box                               |
| 1857 | PreppyL                         | Box                               |
| 1858 | PreppyL                         | Box                               |
| 1859 | PreppyR                         | Box                               |
| 1860 | PreppyR                         | Box                               |
| 1861 | Preps                           | PopulationPed                     |
| 1862 | Principle01                     | Box                               |
| 1863 | Principle02                     | Box                               |
| 1864 | Principle03                     | Box                               |
| 1865 | Principle04                     | Box                               |
| 1866 | Principle_AMB                   | Box                               |
| 1867 | Principle_AMB                   | Box                               |
| 1868 | RAIL_GDORM01                    | Box                               |
| 1869 | RAIL_GDORM02                    | Box                               |
| 1870 | RAIL_HALLWAY01                  | Box                               |
| 1871 | RAIL_HALLWAY02                  | Box                               |
| 1872 | RAIL_HALLWAY03                  | Box                               |
| 1873 | RAIL_HALLWAY04                  | Box                               |
| 1874 | RAIL_HHOUSE01                   | Box                               |
| 1875 | RAIL_RICH01                     | Box                               |
| 1876 | RAIL_RICH02                     | Box                               |
| 1877 | RAIL_RICH03                     | Box                               |
| 1878 | RAIL_RICH04                     | Box                               |
| 1879 | RAIL_RICH05                     | Box                               |
| 1880 | RAIL_RICH06                     | Box                               |
| 1881 | RAIL_SCHOOL01                   | Box                               |
| 1882 | RAIL_SCHOOL02                   | Box                               |
| 1883 | RA_DoorStr02                    | Door                              |
| 1884 | RA_DoorStr05                    | Door                              |
| 1885 | RA_DoorStr06                    | Door                              |
| 1886 | RA_DoorStr07                    | Door                              |
| 1887 | RA_DoorStr08                    | Door                              |
| 1888 | RA_DoorStr09                    | Door                              |
| 1889 | RA_Medium01                     | Box                               |
| 1890 | RA_Medium02                     | Box                               |
| 1891 | RA_Medium03                     | Box                               |
| 1892 | RA_Medium04                     | Box                               |
| 1893 | RA_Medium05                     | Box                               |
| 1894 | RA_Medium06                     | Box                               |
| 1895 | RA_Medium07                     | Box                               |
| 1896 | RA_Medium08                     | Box                               |
| 1897 | RA_Medium10                     | Box                               |
| 1898 | RA_Medium11                     | Box                               |
| 1899 | RA_Medium12                     | Box                               |
| 1900 | RA_Medium13                     | Box                               |
| 1901 | RA_Medium14                     | Box                               |
| 1902 | RA_Medium15                     | Box                               |
| 1903 | RA_Medium16                     | Box                               |
| 1904 | RA_Medium17                     | Box                               |
| 1905 | RA_Medium18                     | Box                               |
| 1906 | RA_Medium19                     | Box                               |
| 1907 | RA_Medium20                     | Box                               |
| 1908 | RA_Medium21                     | Box                               |
| 1909 | RA_Medium22                     | Box                               |
| 1910 | RA_Medium23                     | Box                               |
| 1911 | RA_Medium24                     | Box                               |
| 1912 | RA_PrepDoor02                   | Door                              |
| 1913 | RA_PrepDoor03                   | Door                              |
| 1914 | RA_PrepDoor04                   | Door                              |
| 1915 | RA_PrepDoor05                   | Door                              |
| 1916 | RA_PrepDoor06                   | Door                              |
| 1917 | RA_PrepDoor07                   | Door                              |
| 1918 | RA_PrepDoor08                   | Door                              |
| 1919 | RA_PrepDoor09                   | Door                              |
| 1920 | RA_PrepDoor10                   | Door                              |
| 1921 | RA_PrepDoor11                   | Door                              |
| 1922 | RA_PrepDoor12                   | Door                              |
| 1923 | RA_PrepDoor13                   | Door                              |
| 1924 | RA_PrepDoor14                   | Door                              |
| 1925 | RA_PrepDoor15                   | Door                              |
| 1926 | RA_medium09                     | Box                               |
| 1927 | RCLTH_Trigger                   | Box                               |
| 1928 | RG_FW_enter_m                   | Door                              |
| 1929 | RG_FW_enter_s                   | Door                              |
| 1930 | RG_FW_exit_m                    | Door                              |
| 1931 | RG_FW_exit_s                    | Door                              |
| 1932 | RG_RC_enter_m                   | Door                              |
| 1933 | RG_RC_enter_s                   | Door                              |
| 1934 | RG_RC_exit_m                    | Door                              |
| 1935 | RG_RC_exit_s                    | Door                              |
| 1936 | RG_SQ_enter_m                   | Door                              |
| 1937 | RG_SQ_exit_m                    | Door                              |
| 1938 | RICH_SODA_01                    | Box                               |
| 1939 | RMailbox                        | Door                              |
| 1940 | RT_Tether                       | Box                               |
| 1941 | Race3BrakeTutorial              | Box                               |
| 1942 | RetirementTrigger               | Box                               |
| 1943 | RichArea                        | PopulationPed + PopulationVehicle |
| 1944 | RichArea_DownTown               | PopulationPed + PopulationVehicle |
| 1945 | RichBoxing                      | Box                               |
| 1946 | RichClothing_Change             | Box                               |
| 1947 | RichClothing_Main               | Box                               |
| 1948 | RichFolkTrigger                 | Box                               |
| 1949 | RichNoGoArea                    | Box                               |
| 1950 | Rich_Area_Corner_Courtyard      | Box                               |
| 1951 | Rich_GreaserAlley               | PopulationPed                     |
| 1952 | Rich_GreaserAlley2              | Box                               |
| 1953 | Rich_MailBox01                  | Box                               |
| 1954 | Rich_MailBox23                  | Box                               |
| 1955 | Rich_MailBox24                  | Box                               |
| 1956 | Rich_MailBox25                  | Box                               |
| 1957 | Rich_Mailbox02                  | Box                               |
| 1958 | Rich_Mailbox03                  | Box                               |
| 1959 | Rich_Mailbox04                  | Box                               |
| 1960 | Rich_Mailbox05                  | Box                               |
| 1961 | Rich_Mailbox06                  | Box                               |
| 1962 | Rich_Mailbox07                  | Box                               |
| 1963 | Rich_Mailbox08                  | Box                               |
| 1964 | Rich_Mailbox09                  | Box                               |
| 1965 | Rich_Mailbox10                  | Box                               |
| 1966 | Rich_Mailbox11                  | Box                               |
| 1967 | Rich_Mailbox12                  | Box                               |
| 1968 | Rich_Mailbox13                  | Box                               |
| 1969 | Rich_Mailbox14                  | Box                               |
| 1970 | Rich_Mailbox15                  | Box                               |
| 1971 | Rich_Mailbox16                  | Box                               |
| 1972 | Rich_Mailbox17                  | Box                               |
| 1973 | Rich_Mailbox18                  | Box                               |
| 1974 | Rich_Mailbox19                  | Box                               |
| 1975 | Rich_Mailbox20                  | Box                               |
| 1976 | Rich_Mailbox21                  | Box                               |
| 1977 | Rich_Mailbox22                  | Box                               |
| 1978 | Rich_target1                    | Box                               |
| 1979 | Rich_target2                    | Box                               |
| 1980 | Rich_target3                    | Box                               |
| 1981 | RingArea                        | Box                               |
| 1982 | RunningThiefTrigger             | Box                               |
| 1983 | SAVEBOOKSCHOOL                  | Box                               |
| 1984 | SCFount                         | Door                              |
| 1985 | SCHOOLPROP_SODA_01              | Box                               |
| 1986 | SCHOOLPROP_SODA_02              | Box                               |
| 1987 | SCLock01                        | Door                              |
| 1988 | SCLock02                        | Box                               |
| 1989 | SCLock03                        | Box                               |
| 1990 | SC_Crest                        | Door                              |
| 1991 | SCgrdoor                        | Door                              |
| 1992 | SCgrdoor01                      | Door                              |
| 1993 | SCgrdoor02                      | Door                              |
| 1994 | SGTargBTrig                     | Box                               |
| 1995 | SG_Medium01                     | Box                               |
| 1996 | SG_Medium02                     | Box                               |
| 1997 | SG_Medium03                     | Box                               |
| 1998 | SG_Medium04                     | Box                               |
| 1999 | SG_Medium05                     | Box                               |
| 2000 | SG_Medium06                     | Box                               |
| 2001 | SG_Medium07                     | Box                               |
| 2002 | SG_Medium08                     | Box                               |
| 2003 | SG_Medium09                     | Box                               |
| 2004 | SG_Medium10                     | Box                               |
| 2005 | SG_Medium11                     | Box                               |
| 2006 | SG_Medium12                     | Box                               |
| 2007 | SG_Medium14                     | Box                               |
| 2008 | SG_Medium15                     | Box                               |
| 2009 | SG_Medium16                     | Box                               |
| 2010 | SG_Medium17                     | Box                               |
| 2011 | SG_Medium18                     | Box                               |
| 2012 | SG_Medium19                     | Box                               |
| 2013 | SG_Medium20                     | Box                               |
| 2014 | SH_Medium01                     | Box                               |
| 2015 | SH_Medium02                     | Box                               |
| 2016 | SH_Medium03                     | Box                               |
| 2017 | SH_Medium04                     | Box                               |
| 2018 | SH_Medium05                     | Box                               |
| 2019 | SH_Medium07                     | Box                               |
| 2020 | SH_Medium08                     | Box                               |
| 2021 | SH_Medium09                     | Box                               |
| 2022 | SND_BEACH                       | Box                               |
| 2023 | SND_BUSINESS_AREA               | Box                               |
| 2024 | SND_CARNIVAL_AREA               | Box                               |
| 2025 | SND_CarnTunnelBank              | Box                               |
| 2026 | SND_DAM                         | Box                               |
| 2027 | SND_DOCKYARD                    | Box                               |
| 2028 | SND_INDUSTRIAL_AREA             | Box                               |
| 2029 | SND_POOR_AREA                   | Box                               |
| 2030 | SND_RICHPARKSPRINKLERS          | Box                               |
| 2031 | SND_RICH_AREA                   | Box                               |
| 2032 | SND_Roundhouse                  | Box                               |
| 2033 | SND_SCHOOLPOND                  | Box                               |
| 2034 | SND_SCHOOLTUNNEL01              | Box                               |
| 2035 | SND_SCHOOLTUNNEL02              | Box                               |
| 2036 | SND_SCHOOLTUNNEL03              | Box                               |
| 2037 | SND_SCHOOL_AREA                 | Box                               |
| 2038 | SND_SCHOOL_ROOF                 | Box                               |
| 2039 | SND_WATER                       | Box                               |
| 2040 | SOCCER_SHOOT_OUT_01             | Box                               |
| 2041 | SOCCER_SHOOT_OUT_02             | Box                               |
| 2042 | SO_Medium01                     | Box                               |
| 2043 | SO_Medium02                     | Box                               |
| 2044 | SO_Medium03                     | Box                               |
| 2045 | SO_Medium04                     | Box                               |
| 2046 | SO_Medium05                     | Box                               |
| 2047 | ST1_dePopSnowArea               | PopulationPed                     |
| 2048 | ST2_dePopSnowArea               | PopulationPed                     |
| 2049 | ST3_dePopSnowArea               | PopulationPed                     |
| 2050 | ST4_dePopSnowArea               | PopulationPed                     |
| 2051 | ST5_dePopSnowArea               | PopulationPed                     |
| 2052 | ST6_dePopSnowArea               | PopulationPed                     |
| 2053 | STEALTH_PORTAPOTTY              | PopulationVehicle                 |
| 2054 | ST_CRATE_01                     | Box                               |
| 2055 | ST_CRATE_02                     | Box                               |
| 2056 | ST_CRATE_03                     | Box                               |
| 2057 | ST_DOOR                         | Box                               |
| 2058 | SV_BDormCrawl                   | Box                               |
| 2059 | SV_BioSchool                    | Box                               |
| 2060 | SV_CarnivalFunhouse             | Box                               |
| 2061 | SV_ChemSchool                   | Box                               |
| 2062 | SV_ExtBDormCrawl                | Box                               |
| 2063 | SV_GirlsDorm                    | Box                               |
| 2064 | SV_GirlsDormExit                | Box                               |
| 2065 | SandCasl                        | Door                              |
| 2066 | SaveBookBoysDorm                | Box                               |
| 2067 | SaveBookDropouts                | Box                               |
| 2068 | SaveBookGreasers                | Box                               |
| 2069 | SaveBookJocks                   | Box                               |
| 2070 | SaveBookNerds                   | Box                               |
| 2071 | SaveBookPreps                   | Box                               |
| 2072 | ScGate_Observatory              | Door                              |
| 2073 | SchoolArea                      | PopulationPed                     |
| 2074 | SchoolBackR                     | Box                               |
| 2075 | SchoolBackR                     | Box                               |
| 2076 | SchoolBikeTrig                  | PopulationVehicle                 |
| 2077 | SchoolBio                       | Box                               |
| 2078 | SchoolBoysWash                  | Box                               |
| 2079 | SchoolBoysWash2                 | Box                               |
| 2080 | SchoolCaf1                      | Box                               |
| 2081 | SchoolCaf2                      | Box                               |
| 2082 | SchoolCafeteria                 | Box                               |
| 2083 | SchoolChem                      | Box                               |
| 2084 | SchoolDepop                     | PopulationPed                     |
| 2085 | SchoolEnglish                   | Box                               |
| 2086 | SchoolEntrL1                    | Box                               |
| 2087 | SchoolEntrL1                    | Box                               |
| 2088 | SchoolEntrL2                    | Box                               |
| 2089 | SchoolEntrL2                    | Box                               |
| 2090 | SchoolEntrR1                    | Box                               |
| 2091 | SchoolEntrR1                    | Box                               |
| 2092 | SchoolEntrR2                    | Box                               |
| 2093 | SchoolEntrR2                    | Box                               |
| 2094 | SchoolEntranceTrig              | Box                               |
| 2095 | SchoolGameArea                  | Box                               |
| 2096 | SchoolGirlsWash                 | Box                               |
| 2097 | SchoolGirlsWash2                | Box                               |
| 2098 | SchoolHallRoofStairway          | Box                               |
| 2099 | SchoolHalls01                   | Box                               |
| 2100 | SchoolHalls02                   | Box                               |
| 2101 | SchoolMain                      | Box                               |
| 2102 | SchoolMainAtrium                | Box                               |
| 2103 | SchoolNurse                     | Box                               |
| 2104 | SchoolPrincipal                 | Box                               |
| 2105 | SchoolRoofTrig                  | Box                               |
| 2106 | SchoolSecondFloor               | Box                               |
| 2107 | SchoolSecondFloor               | Box                               |
| 2108 | SchoolSideTrig                  | Box                               |
| 2109 | SchoolStoreExc                  | Box                               |
| 2110 | SchoolTower                     | Box                               |
| 2111 | SchoolTower                     | Box                               |
| 2112 | SchoolTrig                      | PopulationPed                     |
| 2113 | School_Basketball_Court         | Box                               |
| 2114 | School_Turret                   | Box                               |
| 2115 | School_TurretTripod             | Box                               |
| 2116 | Silo                            | Box                               |
| 2117 | SmallCrate1                     | Box                               |
| 2118 | SmallCrate10                    | Box                               |
| 2119 | SmallCrate11                    | Box                               |
| 2120 | SmallCrate2                     | Box                               |
| 2121 | SmallCrate3                     | Box                               |
| 2122 | SmallCrate5                     | Box                               |
| 2123 | SmallCrate6                     | Box                               |
| 2124 | SmallCrate7                     | Box                               |
| 2125 | SmallCrate9                     | Box                               |
| 2126 | Snowman                         | Box                               |
| 2127 | SouvienrShop                    | Box                               |
| 2128 | SpawnKiss                       | Box                               |
| 2129 | SpawnTest_Door1                 | Box                               |
| 2130 | SpawnTest_Door2                 | Box                               |
| 2131 | SpawnTest_Trig1                 | Box                               |
| 2132 | Spud_Cannon_Bottom              | Box                               |
| 2133 | Spud_Cannon_Top                 | Box                               |
| 2134 | Squid                           | Door                              |
| 2135 | Stable                          | Door                              |
| 2136 | Stag1Trig                       | Box                               |
| 2137 | Stag2Trig                       | Box                               |
| 2138 | StalDoor01                      | Box                               |
| 2139 | StalDoor02                      | Box                               |
| 2140 | StalDoor11                      | Box                               |
| 2141 | StatueL                         | Box                               |
| 2142 | StatueL                         | Box                               |
| 2143 | StatueR                         | Box                               |
| 2144 | StatueR                         | Box                               |
| 2145 | StoreCarn_Area                  | Box                               |
| 2146 | Store_BarberPoor_Area           | Box                               |
| 2147 | Store_Barber_Area               | Box                               |
| 2148 | Store_DT_BikeArea               | Box                               |
| 2149 | Store_DT_ComicArea              | Box                               |
| 2150 | Store_DT_GeneralArea            | Box                               |
| 2151 | Store_HairSalon_Area            | Box                               |
| 2152 | TEMPCar1                        | Box                               |
| 2153 | TEMPCar1                        | Box                               |
| 2154 | TEMPCar1                        | Box                               |
| 2155 | TEMPCar2                        | Box                               |
| 2156 | TEMPCar2                        | Box                               |
| 2157 | TEMPCar2                        | Box                               |
| 2158 | TEMPCar3                        | Box                               |
| 2159 | TEMPCar3                        | Box                               |
| 2160 | TENEMENTS_FIRE_ESCAPE_CAMERA    | Box                               |
| 2161 | TEN_FIRE01                      | Box                               |
| 2162 | TEN_FIRE02                      | Box                               |
| 2163 | TEN_FIRE03                      | Box                               |
| 2164 | TEN_FIRE04                      | Box                               |
| 2165 | TEN_FIRE05                      | Box                               |
| 2166 | TEN_FIRE06                      | Box                               |
| 2167 | TEN_FIRE07                      | Box                               |
| 2168 | TEN_FIRE08                      | Box                               |
| 2169 | TEN_FIRE09                      | Box                               |
| 2170 | TEN_FIRE10                      | Box                               |
| 2171 | TF02_Fight1                     | Box                               |
| 2172 | TF02_Fight2                     | Box                               |
| 2173 | TFIGHT01_Barricade              | Box                               |
| 2174 | TFIGHT01_Cannon_Nerd            | Box                               |
| 2175 | TFIGHT01_Door1                  | Box                               |
| 2176 | TFIGHT01_Door2                  | Box                               |
| 2177 | TFIGHT01_Door3                  | Box                               |
| 2178 | TFIGHT01_Door4                  | Box                               |
| 2179 | TINDUST_ASYLUM                  | Box                               |
| 2180 | TINDUST_BAR_DOOR_01             | Door                              |
| 2181 | TINDUST_BAR_DOOR_02             | Door                              |
| 2182 | TINDUST_BAR_DOOR_03             | Door                              |
| 2183 | TINDUST_BAR_DOOR_PORT           | Box                               |
| 2184 | TINDUST_BAR_DOOR_SWITCH_01      | Box                               |
| 2185 | TINDUST_BAR_DOOR_SWITCH_02      | Box                               |
| 2186 | TINDUST_BAR_DOOR_SWITCH_03      | Box                               |
| 2187 | TINDUST_BAR_DOOR_SWITCH_PORT    | Box                               |
| 2188 | TINDUST_ELECTRIC_SHUTOFF        | Door                              |
| 2189 | TINDUST_FIRE_DOOR_01            | Door                              |
| 2190 | TINDUST_FIRE_DOOR_02            | Door                              |
| 2191 | TINDUST_GATE_SWITCH             | Box                               |
| 2192 | TINDUST_POWER_SWITCH_01         | Box                               |
| 2193 | TINDUST_POWER_SWITCH_02         | Box                               |
| 2194 | TINDUST_REDSTAR_GATE_01         | Door                              |
| 2195 | TINDUST_REDSTAR_SECURITY_DOOR   | Box                               |
| 2196 | TINDUST_SHDOOR_03               | Door                              |
| 2197 | TINDUST_SHDOOR_04               | Door                              |
| 2198 | TINDUST_SHDOOR_05               | Door                              |
| 2199 | TINDUST_SHDOOR_06               | Door                              |
| 2200 | TINDUST_SHDOOR_07               | Door                              |
| 2201 | TINDUST_TRAIN_SWITCH_01         | Box                               |
| 2202 | TINDUST_TRAIN_SWITCH_02         | Box                               |
| 2203 | TPHOTO_FIRE                     | Box                               |
| 2204 | TPHOTO_FIREG                    | Box                               |
| 2205 | TadBackDoorL                    | Door                              |
| 2206 | TadBackDoorR                    | Door                              |
| 2207 | TadFrontDoorL                   | Door                              |
| 2208 | TadFrontDoorR                   | Door                              |
| 2209 | TadGates02                      | Door                              |
| 2210 | TadShud                         | Door                              |
| 2211 | TadShud01                       | Door                              |
| 2212 | TadShud02                       | Door                              |
| 2213 | TadShud03                       | Door                              |
| 2214 | TadShud04                       | Door                              |
| 2215 | TadShud05                       | Door                              |
| 2216 | Tenements_Balcony               | Box                               |
| 2217 | Tenements_Bathroom              | Box                               |
| 2218 | Tenements_Hall01                | Box                               |
| 2219 | Tenements_Hall02                | Box                               |
| 2220 | Tenements_Hall03                | Box                               |
| 2221 | Tenements_Hole                  | Box                               |
| 2222 | Tenements_Hole02                | Box                               |
| 2223 | Tenements_Rm01                  | Box                               |
| 2224 | Tenements_Rm02                  | Box                               |
| 2225 | Tenements_Rm03                  | Box                               |
| 2226 | Tenements_Rm04                  | Box                               |
| 2227 | Tenements_Rm05                  | Box                               |
| 2228 | Tenements_Rm06                  | Box                               |
| 2229 | Tenements_Rm07                  | Box                               |
| 2230 | Tenements_Rm08                  | Box                               |
| 2231 | Tenements_Rm09                  | Box                               |
| 2232 | Tenements_Rm10                  | Box                               |
| 2233 | Tenements_Rm11                  | Box                               |
| 2234 | Tenements_Rm12                  | Box                               |
| 2235 | Tenements_Rm13                  | Box                               |
| 2236 | Tenements_base_stair            | Box                               |
| 2237 | Tenements_basement              | Box                               |
| 2238 | TennFrid                        | Box                               |
| 2239 | TennWash                        | Door                              |
| 2240 | TestBikeGraffiti                | Box                               |
| 2241 | TestMailboxTarget               | Box                               |
| 2242 | TestProjDetectionWall           | Box                               |
| 2243 | TestTriggerEvent                | Box                               |
| 2244 | TetherD101                      | Box                               |
| 2245 | TetherD102                      | Box                               |
| 2246 | TetherD103                      | Box                               |
| 2247 | TetherD104                      | Box                               |
| 2248 | TetherD105                      | Box                               |
| 2249 | TetherD201                      | Box                               |
| 2250 | TetherD202                      | Box                               |
| 2251 | TetherD203                      | Box                               |
| 2252 | TetherD204                      | Box                               |
| 2253 | TetherD205                      | Box                               |
| 2254 | TetherD301                      | Box                               |
| 2255 | TetherD302                      | Box                               |
| 2256 | TetherD303                      | Box                               |
| 2257 | TetherD304                      | Box                               |
| 2258 | TetherD305                      | Box                               |
| 2259 | Theatre                         | Box                               |
| 2260 | ThievesTrigger                  | Box                               |
| 2261 | ThirdFight                      | Box                               |
| 2262 | TicketPickup                    | Box                               |
| 2263 | Toys                            | Box                               |
| 2264 | TrainYard                       | Box                               |
| 2265 | Transmitter                     | Box                               |
| 2266 | TriggerArea                     | Box                               |
| 2267 | TrophyL                         | Box                               |
| 2268 | TrophyL                         | Box                               |
| 2269 | TrophyR                         | Box                               |
| 2270 | TrophyR                         | Box                               |
| 2271 | UmpireFive                      | Box                               |
| 2272 | UmpireFive                      | Box                               |
| 2273 | UmpireFour                      | Box                               |
| 2274 | UmpireFour                      | Box                               |
| 2275 | UmpireOne                       | Box                               |
| 2276 | UmpireOne                       | Box                               |
| 2277 | UmpireSeven                     | Box                               |
| 2278 | UmpireSeven                     | Box                               |
| 2279 | UmpireSix                       | Box                               |
| 2280 | UmpireSix                       | Box                               |
| 2281 | UmpireThree                     | Box                               |
| 2282 | UmpireThree                     | Box                               |
| 2283 | UmpireTwo                       | Box                               |
| 2284 | UmpireTwo                       | Box                               |
| 2285 | WM_GoKartCreate                 | Box                               |
| 2286 | WareHouse_Amb01                 | Box                               |
| 2287 | Water                           | Box                               |
| 2288 | Wires                           | Box                               |
| 2289 | ZoneBusiness                    | Box                               |
| 2290 | ZoneCarnival                    | Box                               |
| 2291 | ZoneIndustrial                  | Box                               |
| 2292 | ZonePoor                        | Box                               |
| 2293 | ZoneRich                        | Box                               |
| 2294 | ZoneSchool                      | Box                               |
| 2295 | \_SSI_00                        | Box                               |
| 2296 | \_SSI_01                        | Box                               |
| 2297 | \_SSI_02                        | Box                               |
| 2298 | \_SSI_03                        | Box                               |
| 2299 | \_SSI_04                        | Box                               |
| 2300 | \_SSI_05                        | Box                               |
| 2301 | \_SSI_06                        | Box                               |
| 2302 | \_SSI_07                        | Box                               |
| 2303 | \_SSI_08                        | Box                               |
| 2304 | \_SSI_09                        | Box                               |
| 2305 | \_SSI_10                        | Box                               |
| 2306 | \_SSI_11                        | Box                               |
| 2307 | \_SSI_12                        | Box                               |
| 2308 | \_SSI_13                        | Box                               |
| 2309 | \_SSI_14                        | Box                               |
| 2310 | \_SSI_15                        | Box                               |
| 2311 | \_SSI_16                        | Box                               |
| 2312 | \_SSI_17                        | Box                               |
| 2313 | \_SSI_18                        | Box                               |
| 2314 | \_SSI_19                        | Box                               |
| 2315 | \_SSI_20                        | Box                               |
| 2316 | \_SSI_21                        | Box                               |
| 2317 | \_SSI_22                        | Box                               |
| 2318 | \_SSI_23                        | Box                               |
| 2319 | \_SSI_24                        | Box                               |
| 2320 | \_SSI_25                        | Box                               |
| 2321 | \_SSI_26                        | Box                               |
| 2322 | \_SSI_27                        | Box                               |
| 2323 | \_SSI_28                        | Box                               |
| 2324 | \_SSI_29                        | Box                               |
| 2325 | \_SSI_30                        | Box                               |
| 2326 | \_SSI_31                        | Box                               |
| 2327 | auditorium_doorR                | Door                              |
| 2328 | barricade102                    | Box                               |
| 2329 | boysDormCourtyard               | Box                               |
| 2330 | bu_DoorStr10                    | Door                              |
| 2331 | bu_PrepDoor13                   | Door                              |
| 2332 | bu_PrepDoor14                   | Door                              |
| 2333 | bu_PrepDoor15                   | Door                              |
| 2334 | bu_PrepDoor16                   | Door                              |
| 2335 | bu_PrepDoor17                   | Door                              |
| 2336 | bu_PrepDoor18                   | Door                              |
| 2337 | bu_PrepDoor19                   | Door                              |
| 2338 | bu_PrepDoor20                   | Door                              |
| 2339 | bu_PrepDoor21                   | Door                              |
| 2340 | bu_PrepDoor22                   | Door                              |
| 2341 | bu_PrepDoor23                   | Door                              |
| 2342 | bu_PrepDoor24                   | Door                              |
| 2343 | bu_PrepDoor25                   | Door                              |
| 2344 | carnGate01                      | Box                               |
| 2345 | carnGate02                      | Box                               |
| 2346 | carnGate03                      | Box                               |
| 2347 | carnGate04                      | Box                               |
| 2348 | crate01                         | Box                               |
| 2349 | dowtownDepop                    | PopulationPed                     |
| 2350 | funCurtn                        | Door                              |
| 2351 | funCurtn01                      | Door                              |
| 2352 | fun_MazeEntryDoor               | Door                              |
| 2353 | gd_GameArea                     | PopulationPed                     |
| 2354 | gd_TrashArea                    | Box                               |
| 2355 | gdorm_DoorR                     | Door                              |
| 2356 | girlsDormCourtyard              | Box                               |
| 2357 | gnomeA                          | Box                               |
| 2358 | gs_GameArea                     | PopulationPed                     |
| 2359 | gs_TrashArea                    | Box                               |
| 2360 | gym_pool                        | Box                               |
| 2361 | gyml_doorR                      | Door                              |
| 2362 | hardwareback                    | Door                              |
| 2363 | iboxing_BoxRopes                | Door                              |
| 2364 | iboxing_BoxRopes01              | Door                              |
| 2365 | iboxing_BoxRopes02              | Door                              |
| 2366 | iboxing_BoxRopes03              | Door                              |
| 2367 | iboxing_ESCDoorL                | Door                              |
| 2368 | iboxing_ESCDoorL01              | Door                              |
| 2369 | iboxing_ESCDoorR                | Door                              |
| 2370 | iboxing_ESCDoorR01              | Door                              |
| 2371 | iboxing_IntDoor02               | Door                              |
| 2372 | iboxing_barvault01              | Box                               |
| 2373 | iboxing_barvault02              | Box                               |
| 2374 | iboxing_fakeCoronaTrigger       | Box                               |
| 2375 | icecream                        | Door                              |
| 2376 | icloth_p_trigger                | Box                               |
| 2377 | icomshp_Basement                | Door                              |
| 2378 | ifunhous_CtrlRoom               | Box                               |
| 2379 | ifunhous_CtrlRoomCtrl           | Box                               |
| 2380 | ifunhous_EndMine                | Box                               |
| 2381 | ifunhous_FLbBook                | Door                              |
| 2382 | ifunhous_FLbLader               | Door                              |
| 2383 | ifunhous_FMTrapDr00L            | Door                              |
| 2384 | ifunhous_FMTrapDr00O            | Door                              |
| 2385 | ifunhous_FMTrapDr01L            | Door                              |
| 2386 | ifunhous_FMTrapDr01O            | Door                              |
| 2387 | ifunhous_FMTrapDr02L            | Door                              |
| 2388 | ifunhous_FMTrapDr02O            | Door                              |
| 2389 | ifunhous_FMTrapDr03L            | Door                              |
| 2390 | ifunhous_FMTrapDr03O            | Door                              |
| 2391 | ifunhous_FMTrapSw               | Door                              |
| 2392 | ifunhous_FMTrapSw01             | Door                              |
| 2393 | ifunhous_FMTrapSw01b            | Door                              |
| 2394 | ifunhous_FMTrapSw02             | Door                              |
| 2395 | ifunhous_FMTrapSw02b            | Door                              |
| 2396 | ifunhous_FMTrapSw03             | Door                              |
| 2397 | ifunhous_FMTrapSw03b            | Door                              |
| 2398 | ifunhous_FMTrapSw04             | Door                              |
| 2399 | ifunhous_FMTrapSw04b            | Door                              |
| 2400 | ifunhous_FMTrapSw05             | Door                              |
| 2401 | ifunhous_FMTrapSw05b            | Door                              |
| 2402 | ifunhous_FMTrapSw06             | Door                              |
| 2403 | ifunhous_FMTrapSw06b            | Door                              |
| 2404 | ifunhous_FMTrapSw07             | Door                              |
| 2405 | ifunhous_FMTrapSw07b            | Door                              |
| 2406 | ifunhous_FMTrapSwb              | Door                              |
| 2407 | ifunhous_MineEnd                | Box                               |
| 2408 | ifunhous_MineMze                | Box                               |
| 2409 | ifunhous_MzeMine                | Box                               |
| 2410 | ifunhous_Reeper00               | Box                               |
| 2411 | ifunhous_Reeper00b              | Door                              |
| 2412 | ifunhous_Reeper01               | Door                              |
| 2413 | ifunhous_Reeper01b              | Box                               |
| 2414 | ifunhous_Reeper02               | Door                              |
| 2415 | ifunhous_Reeper02b              | Box                               |
| 2416 | ifunhous_funMinerB              | Door                              |
| 2417 | ifunhous_funMinerD              | Door                              |
| 2418 | ifunhous_funMinerG              | Door                              |
| 2419 | ifunhous_funMinerH              | Door                              |
| 2420 | ifunhous_funMinerI              | Door                              |
| 2421 | ifunhous_funMinerX1             | Box                               |
| 2422 | ifunhous_funMinerX2             | Box                               |
| 2423 | ifunhous_funMinerX3             | Box                               |
| 2424 | ifunhous_funMinerX4             | Box                               |
| 2425 | ischool_CafDoor2R               | Door                              |
| 2426 | ischool_Door00                  | Door                              |
| 2427 | ischool_Door02                  | Door                              |
| 2428 | ischool_Door05                  | Door                              |
| 2429 | ischool_Door06                  | Door                              |
| 2430 | ischool_Door09                  | Door                              |
| 2431 | ischool_Door19                  | Door                              |
| 2432 | ischool_Door21                  | Door                              |
| 2433 | ischool_Door23                  | Door                              |
| 2434 | ischool_Door24                  | Door                              |
| 2435 | ischool_Door25                  | Door                              |
| 2436 | ischool_Door28                  | Door                              |
| 2437 | ischool_Door30                  | Door                              |
| 2438 | ischool_FrontDoorR              | Door                              |
| 2439 | ischool_StoreArea               | Box                               |
| 2440 | ischool_StoreDoor               | Door                              |
| 2441 | ischool_fountains_SCFount       | Door                              |
| 2442 | ischool_fountains_SCFount03     | Door                              |
| 2443 | ischool_fountains_SCFount04     | Door                              |
| 2444 | ischool_fountains_SCFount05     | Door                              |
| 2445 | ischool_fountains_SCFount06     | Door                              |
| 2446 | ischool_fountains_SCFount09     | Door                              |
| 2447 | ischool_fountains_SCFount12     | Door                              |
| 2448 | ischool_fountains_SCFount15     | Door                              |
| 2449 | ischool_fountains_SCFount16     | Door                              |
| 2450 | isclib_Globe                    | Box                               |
| 2451 | lvl1GameArea                    | Box                               |
| 2452 | lvl2GameArea                    | Box                               |
| 2453 | lvl3GameArea                    | Box                               |
| 2454 | lvl4GameArea                    | Box                               |
| 2455 | lvl5GameArea                    | Box                               |
| 2456 | lvl5_gate                       | Box                               |
| 2457 | lvl5_snowPile03                 | Box                               |
| 2458 | lvl5_snowPile06                 | Box                               |
| 2459 | lvl5_snowPile07                 | Box                               |
| 2460 | lvl5_snowPile08                 | Box                               |
| 2461 | lvl5_snowPile09                 | Box                               |
| 2462 | lvl5_snowPile10                 | Box                               |
| 2463 | lvl6GameArea                    | Box                               |
| 2464 | lvl6_snowPile_04                | Box                               |
| 2465 | lvl6_snowPile_05                | Box                               |
| 2466 | lvl6_snowPile_06                | Box                               |
| 2467 | lvl6_snowPile_07                | Box                               |
| 2468 | lvl6_snowPile_08                | Box                               |
| 2469 | lvl6_snowPile_09                | Box                               |
| 2470 | lvl6_snowPile_10                | Box                               |
| 2471 | lvl6_snowPile_12                | Box                               |
| 2472 | lvl6_snowPile_14                | Box                               |
| 2473 | observatory_doorR               | Door                              |
| 2474 | pChair                          | Door                              |
| 2475 | pa_GameArea                     | PopulationPed                     |
| 2476 | pa_Hobo1Area                    | Box                               |
| 2477 | pa_Hobo2Area                    | Box                               |
| 2478 | pa_Hobo3Area                    | Box                               |
| 2479 | pa_TrashArea                    | Box                               |
| 2480 | plat_North                      | Box                               |
| 2481 | plat_South                      | Box                               |
| 2482 | plat_West                       | Box                               |
| 2483 | platform_South                  | Box                               |
| 2484 | platform_West                   | Box                               |
| 2485 | pool_boyslocker                 | Box                               |
| 2486 | pool_doorR                      | Door                              |
| 2487 | pool_girlslocker                | Box                               |
| 2488 | smallTag                        | Box                               |
| 2489 | snowPile1_01                    | Box                               |
| 2490 | snowPile1_02                    | Box                               |
| 2491 | snowPile1_03                    | Box                               |
| 2492 | snowPile1_04                    | Box                               |
| 2493 | snowPile2_01                    | Box                               |
| 2494 | snowPile2_02                    | Box                               |
| 2495 | snowPile2_03                    | Box                               |
| 2496 | snowPile2_04                    | Box                               |
| 2497 | snowPile2_05                    | Box                               |
| 2498 | snowPile2_06                    | Box                               |
| 2499 | snowPile3_01                    | Box                               |
| 2500 | snowPile3_02                    | Box                               |
| 2501 | snowPile3_03                    | Box                               |
| 2502 | snowPile3_04                    | Box                               |
| 2503 | snowPile3_05                    | Box                               |
| 2504 | snowPile3_06                    | Box                               |
| 2505 | snowPile3_07                    | Box                               |
| 2506 | snowPile3_08                    | Box                               |
| 2507 | snowStage4_01                   | Box                               |
| 2508 | snowStage4_02                   | Box                               |
| 2509 | snowStage4_04                   | Box                               |
| 2510 | snowStage4_05                   | Box                               |
| 2511 | tag1                            | Box                               |
| 2512 | tbarrels_Sbarels1               | Door                              |
| 2513 | tbusiness_BMXGate               | Door                              |
| 2514 | tbusiness_GarbCanA08            | Door                              |
| 2515 | tbusiness_MotelDor              | Door                              |
| 2516 | testSafeCut_startCut            | Box                               |
| 2517 | tmrf_ratBoundary                | Box                               |
| 2518 | trich_SprinklerSwitch           | Box                               |
| 2519 | trich_TadGates                  | Door                              |
| 2520 | trich_TadGates01                | Door                              |
| 2521 | triggerBackAlley                | Box                               |
| 2522 | triggerBalcony                  | Box                               |
| 2523 | triggerBalcony2                 | Box                               |
| 2524 | triggerLola                     | Box                               |
| 2525 | triggerTadTether                | Box                               |
| 2526 | tschool_AutoShopFGate           | Door                              |
| 2527 | tschool_BoysDormR               | Door                              |
| 2528 | tschool_FieldR                  | Door                              |
| 2529 | tschool_FrontGate               | Door                              |
| 2530 | tschool_FrontGate               | Door                              |
| 2531 | tschool_FrontGate               | Door                              |
| 2532 | tschool_GirlsDormR              | Door                              |
| 2533 | tschool_GymR                    | Door                              |
| 2534 | tschool_LibraryR                | Door                              |
| 2535 | tschool_ParkingGate             | Door                              |
| 2536 | tschool_ParkingGate             | Door                              |
| 2537 | tschool_PoolR                   | Door                              |
| 2538 | tschool_PreppyR                 | Door                              |
| 2539 | tschool_SchoolFrontDoorR        | Door                              |
| 2540 | tschool_SchoolLeftFrontDoor     | Door                              |
| 2541 | turret_top                      | Box                               |
| 2542 | tutorialTag                     | Box                               |
| 2543 | valeHotelDoor                   | Door                              |

---

## Duplicate Triggers

|   # | Trigger Key            | Appears | Files                                                                                        |
| --: | ---------------------- | ------- | -------------------------------------------------------------------------------------------- |
|   1 | 3_02_BUSINESSAREA      | 2       | 3_02.dat, 3_02_new.dat                                                                       |
|   2 | 3_02_PARKENTRANCE      | 2       | 3_02.dat, 3_02_new.dat                                                                       |
|   3 | 3_02_SPAWNER01         | 2       | 3_02.dat, 3_02_new.dat                                                                       |
|   4 | 3_02_SPAWNER02         | 2       | 3_02.dat, 3_02_new.dat                                                                       |
|   5 | 3_02_SPAWNER03         | 2       | 3_02.dat, 3_02_new.dat                                                                       |
|   6 | 3_02_SPAWNER04         | 2       | 3_02.dat, 3_02_new.dat                                                                       |
|   7 | 3_02_SPAWNER05         | 2       | 3_02.dat, 3_02_new.dat                                                                       |
|   8 | 3_R09_AreaT01          | 4       | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Preppies.dat                  |
|   9 | 3_R09_AreaT02          | 4       | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Preppies.dat                  |
|  10 | 3_R09_MainArea         | 2       | 3_R09_Dropouts.dat, 3_R09_Greasers.dat                                                       |
|  11 | 3_R09_SpawnT01         | 5       | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Nerds.dat, 3_R09_Preppies.dat |
|  12 | 3_R09_SpawnT02         | 5       | 3_R09_Dropouts.dat, 3_R09_Greasers.dat, 3_R09_Jocks.dat, 3_R09_Nerds.dat, 3_R09_Preppies.dat |
|  13 | 3_S09_Cover01          | 2       | 3_S09.dat, RaulTest.dat                                                                      |
|  14 | 3_S09_Cover02          | 2       | 3_S09.dat, RaulTest.dat                                                                      |
|  15 | 3_S09_Cover03          | 2       | 3_S09.dat, RaulTest.dat                                                                      |
|  16 | 3_S09_Cover04          | 2       | 3_S09.dat, RaulTest.dat                                                                      |
|  17 | 3_S09_CoverArea        | 2       | 3_S09.dat, RaulTest.dat                                                                      |
|  18 | 3_S09_Dumpster01       | 2       | 3_S09.dat, RaulTest.dat                                                                      |
|  19 | 3_S09_LeavingTrigger   | 2       | 3_S09.dat, RaulTest.dat                                                                      |
|  20 | 4_02_Bar_01            | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  21 | 4_02_Bar_02            | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  22 | 4_02_Bar_03            | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  23 | 4_02_Breaker_Box       | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  24 | 4_02_Delete_Wave1      | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  25 | 4_02_Delete_Wave3      | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  26 | 4_02_Eavesdrop         | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  27 | 4_02_Finale            | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  28 | 4_02_NERDS             | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  29 | 4_02_O_R1_1T           | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  30 | 4_02_O_R2_1T           | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  31 | 4_02_O_WN1_1T          | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  32 | 4_02_O_WN2_1T          | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  33 | 4_02_O_WN3_1T          | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  34 | 4_02_O_WN4_1T          | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  35 | 4_02_PREFECT1          | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  36 | 4_02_PREFECT2          | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  37 | 4_02_P_Wave2           | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  38 | 4_02_P_Wave3           | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  39 | 4_02_P_Wave4           | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  40 | 4_02_Player_On_CannonT | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  41 | 4_02_Player_Out_Of_Lib | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  42 | 4_02_Spotted_Scout     | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  43 | 4_02_Spud_Cannon       | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  44 | 4_02_Spud_Tripod       | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  45 | 4_02_TEMP_Cannon_Line2 | 2       | 4_02.dat, Test_4_02.dat                                                                      |
|  46 | AcrossGymBack          | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  47 | AngelStatue            | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  48 | AutoGarage             | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  49 | AutoShop               | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  50 | AutoShopSide           | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  51 | BDormFlag1             | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  52 | BarberShop             | 2       | SP_Barber.dat, SP_Pool.dat                                                                   |
|  53 | BatterEight            | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  54 | BatterFive             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  55 | BatterFour             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  56 | BatterNine             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  57 | BatterOne              | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  58 | BatterSeven            | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  59 | BatterSix              | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  60 | BatterThree            | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  61 | BatterTwo              | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  62 | BdrDoorL               | 2       | iSaveZones.dat, isc_offi.dat                                                                 |
|  63 | BdrDoorL01             | 2       | iSaveZones.dat                                                                               |
|  64 | BdrDoorL02             | 2       | iSaveZones.dat                                                                               |
|  65 | BleachersL             | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  66 | BleachersR             | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  67 | CatcherFive            | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  68 | CatcherFour            | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  69 | CatcherOne             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  70 | CatcherSeven           | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  71 | CatcherSix             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  72 | CatcherThree           | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  73 | CatcherTwo             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
|  74 | ESCDoorL               | 2       | iSaveZones.dat, isc_lib.dat                                                                  |
|  75 | ESCDoorL05             | 2       | iSaveZones.dat, trich.dat                                                                    |
|  76 | ESCDoorR               | 2       | iSaveZones.dat, iasylum.dat                                                                  |
|  77 | EquipmentRoom          | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  78 | FMDoor                 | 2       | iSaveZones.dat, iasylum.dat                                                                  |
|  79 | FlagLeftSchool         | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  80 | FlagRightSchool        | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  81 | GDormBackDr            | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  82 | GDormEntrance          | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  83 | GlassDome              | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  84 | Gymnasium              | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  85 | GymnasiumBack          | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  86 | LibraryArch            | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  87 | LibraryL               | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  88 | LibraryR               | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  89 | NLock01A               | 2       | ischool_lockers.dat, ttest.dat                                                               |
|  90 | NerdComputerRoom       | 2       | SP_Comic_Shop_Rich.dat, SP_iNerdS.dat                                                        |
|  91 | NerdMainRoom           | 2       | SP_Comic_Shop_Rich.dat, SP_iNerdS.dat                                                        |
|  92 | NerdStairwell          | 2       | SP_Comic_Shop_Rich.dat, SP_iNerdS.dat                                                        |
|  93 | ParkingArchway         | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  94 | PreppyL                | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  95 | PreppyR                | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  96 | Principle_AMB          | 2       | SP_Principal.dat, SP_School_Hallways.dat                                                     |
|  97 | SchoolBackR            | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  98 | SchoolEntrL1           | 2       | C5.dat, PhotoZoom.dat                                                                        |
|  99 | SchoolEntrL2           | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 100 | SchoolEntrR1           | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 101 | SchoolEntrR2           | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 102 | SchoolSecondFloor      | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 103 | SchoolTower            | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 104 | StatueL                | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 105 | StatueR                | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 106 | TEMPCar1               | 3       | P_Snow4.dat, P_Snow5.dat, P_Snow6.dat                                                        |
| 107 | TEMPCar2               | 3       | P_Snow4.dat, P_Snow5.dat, P_Snow6.dat                                                        |
| 108 | TEMPCar3               | 2       | P_Snow4.dat, P_Snow6.dat                                                                     |
| 109 | TrophyL                | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 110 | TrophyR                | 2       | C5.dat, PhotoZoom.dat                                                                        |
| 111 | UmpireFive             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 112 | UmpireFour             | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 113 | UmpireOne              | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 114 | UmpireSeven            | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 115 | UmpireSix              | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 116 | UmpireThree            | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 117 | UmpireTwo              | 2       | MGBaseballToss.dat, TestBaseballToss.dat                                                     |
| 118 | tschool_FrontGate      | 3       | 1_01.dat, 6_02.dat, Chapt1Trans.dat                                                          |
| 119 | tschool_ParkingGate    | 2       | 6_02.dat, Chapt1Trans.dat                                                                    |

---

## Triggers by File

### 1_01.dat

Count: 7

- 1_01_BullyTrig
- 1_01_CHECKOBJS1
- 1_01_FightTrigger
- 1_01_ParkDoor
- 1_01_PrincOffice
- 1_01_SchoolTrig
- tschool_FrontGate

### 1_02.dat

Count: 6

- 1_02_FightArea
- 1_02_PopulationTrig
- 1_02_RusselTease
- 1_02_SchoolTrig
- 1_02_TrainArea
- GaryTrigger

### 1_02B.dat

Count: 17

- 1_02B_bathroom
- 1_02B_cafeMessage
- 1_02B_constTether
- 1_02B_disablePOI
- 1_02B_euniceKiss
- 1_02B_excluderLocker
- 1_02B_lockerMessage
- 1_02B_lockerMessage02
- 1_02B_objCafe
- 1_02B_objLocker
- 1_02B_objSocial
- 1_02B_recruitGary
- 1_02B_socialMessage
- 1_02B_warn01
- 1_02B_warn02
- 1_02B_warn03
- 1_02B_warn04

### 1_03.dat

Count: 25

- 1_03_AutoShopArea
- 1_03_DavisRegisterHit
- 1_03_DavisRun
- 1_03_FailTrigger01
- 1_03_FailTrigger02
- 1_03_FalTrigger04
- 1_03_Fight1
- 1_03_Fight3
- 1_03_Fight4
- 1_03_Fight5
- 1_03_FrontGate
- 1_03_GameArea
- 1_03_Garage02
- 1_03_Garage03
- 1_03_GarbageCan02
- 1_03_GarbageCan05
- 1_03_GarbageCan06
- 1_03_GarbageCan07
- 1_03_JumpTut01
- 1_03_KeepPedTrigger
- 1_03_Ladder_Drop
- 1_03_PeterTrigger
- 1_03_SchoolYard
- 1_03_barelLad
- tschool_AutoShopFGate

### 1_04.dat

Count: 11

- 1_04_BottleNIS
- 1_04_BottleShootArea
- 1_04_BottleZone
- 1_04_FieldTrig
- 1_04_NemSitDown
- 1_04_Parking
- 1_04_SuppressFieldPop
- 1_04_SuppressParkingPop
- 1_04_tree1_trig
- 1_04_tree2_trig
- 1_04_tree_sit

### 1_05.dat

Count: 9

- 1_05_backDoorOff
- 1_05_frontDoorOff
- 1_05_triggerJockPack
- 1_05_triggerJockPackWarning
- 1_05_triggerJocksNearFront
- 1_05_triggerJocksNearLibrary
- StalDoor01
- StalDoor02
- StalDoor11

### 1_05b.dat

Count: 10

- 1_05B_algieLocker
- 1_05B_algieStall
- 1_05B_areaSecondFloorBR
- 1_05B_bathroomFirstFloor
- 1_05B_bathroomSecondFloor
- 1_05B_firstFloorAmbientOff
- 1_05B_firstFloorAmbientOn
- 1_05B_firstFloorGirlsBR
- 1_05B_loadSmoke
- 1_05B_secondFloorGirlsBR

### 1_06.dat

Count: 8

- FightingArea
- FinalPosCheck
- HighGround
- HoboTrigger
- LowCorona
- RingArea
- Transmitter
- TriggerArea

### 1_07.dat

Count: 15

- 1_07_BUCKY_BOUND
- 1_07_FightTrigger
- 1_07_GateTrig
- 1_07_Gate_T
- 1_07_Library_Door
- 1_07_NEAR_PARKING_LOT
- 1_07_NoAmbientPeds
- 1_07_SpawnZone
- 1_07_Spawner01
- 1_07_Spawner02
- 1_07_Spawner03
- 1_07_Spawner04
- 1_07_Spawner05
- 1_07_Spawner06
- 1_07_ToolBox01

### 1_08.dat

Count: 23

- 1_08_BathroomLocker
- 1_08_CafTrig
- 1_08_GYMGIRLWASH
- 1_08_JimmyLeft
- BathroomExit
- BathroomLeftTrig
- BathroomRightTrig
- BeatriceCutsceneTrigger
- BeatriceTrigger
- BitchDice
- BuckyCutsceneTrigger
- BuckyTrigger
- CafBackTrigger
- ChangeRoom
- CheerleadersTrigger
- FountainCutscene
- LackeySetA
- LackeySetB
- LackeySetC
- LackeySetD
- LackeySetE
- RunningThiefTrigger
- ThievesTrigger

### 1_09.dat

Count: 9

- 1_09_AisleLeft
- 1_09_AisleRight
- 1_09_BoxLeft1
- 1_09_BoxLeft2
- 1_09_BoxRight1
- 1_09_BoxRight2
- 1_09_Catwalk1
- 1_09_StageLeft
- 1_09_StageRight

### 1_10.dat

Count: 19

- 1_10_BasementDoor
- 1_10_BullyTrigger
- 1_10_CrouchHint
- 1_10_GARY_TURN_OFF_ELEC
- 1_10_InCage
- 1_10_NearHole
- 1_10_Near_BasementDoor
- 1_10_TheHole
- 1_10_almost_complete
- 1_10_atFurnace
- 1_10_aud_2
- 1_10_crawl_elec
- 1_10_exit_cage
- 1_10_ring_peds
- 1_10_room0
- 1_10_room1
- 1_10_room2
- 1_10_room3
- 1_10_room4

### 1_11x1.dat

Count: 3

- 1_11X1_bullies
- 1_11X1_outside
- 1_11X1_pete

### 1_11x2.dat

Count: 3

- 1_11x2_chadAttack
- 1_11x2_garden
- 1_11x2_shitTarget

### 1_11xp.dat

Count: 8

- 1_11xp_DeadRat
- 1_11xp_F4000
- 1_11xp_Firecracker
- 1_11xp_ItchPowder
- 1_11xp_JokeCandy
- 1_11xp_KickMe
- 1_11xp_Marbles
- 1_11xp_StinkBomb

### 1_G1_new.dat

Count: 4

- 1_G1_BeatriceWarning
- 1_G1_MathProxy
- 1_G1_StaffProxy
- 1_g1_Locker

### 1_S01.dat

Count: 17

- 1_S01_Bathroom
- 1_S01_BathroomSetup
- 1_S01_Bottle_Trig_Bath
- 1_S01_Bottle_Trig_Cafe
- 1_S01_Bottle_Trig_Case
- 1_S01_Cafe
- 1_S01_Create_Edna
- 1_S01_Glass
- 1_S01_HattrickDelete
- 1_S01_Kitchen
- 1_S01_Phillips_Return
- 1_S01_PlayerBlocking
- 1_S01_Prefect1
- 1_S01_Prefect_8_1_Spawn
- 1_S01_Prefect_Running1
- 1_S01_Prefect_Running1_Delete
- 1_S01_TrophySetup

### 2_01.dat

Count: 10

- 2_01_EdnaFacePlayer
- 2_01_GreaserTrig
- 2_01_GreaserTrig2
- 2_01_MOUNTBIKE
- 2_01_PreppyTrig
- 2_01_PreppyTrig2
- 2_01_StartCopfight
- 2_01_TutPlay1
- 2_01_tutOff
- 2_01_tutOff2

### 2_02.dat

Count: 2

- 2_02_returnComic
- 2_02_schoolParking

### 2_03.dat

Count: 13

- 2_03_BRTadTrigger
- 2_03_Back_Gate
- 2_03_Back_Unlock
- 2_03_Backyard
- 2_03_FrontDoorTrigger
- 2_03_FrontGateArea
- 2_03_FrontYard
- 2_03_Front_Unlock
- 2_03_RearDoorTrigger
- 2_03_RearGateArea
- 2_03_TadHouse
- 2_03_TadNIS
- 2_03_TadsBlock

### 2_04.dat

Count: 11

- 2_04_BarrelFire01
- 2_04_BarrelFire02
- 2_04_BarrelFire03
- 2_04_BarrelFire04
- 2_04_BarrelFire05
- 2_04_BarrelFire06
- 2_04_ChangeBeach
- 2_04_DormDoor
- 2_04_TireFire01b
- 2_04_TireFire02b
- 2_04_TireFire03b

### 2_04_Bus.dat

Count: 4

- 2_04_CHEATER_1_ZONE
- 2_04_CHEATER_2_ZONE
- 2_04_CHEATER_3_ZONE
- 2_04_CHEATER_4_ZONE

### 2_05_new.dat

Count: 19

- 2_05_BACKGATE
- 2_05_EggStashArea
- 2_05_FRONTGATE
- 2_05_FrontExit
- 2_05_RecruitRussell
- 2_05_RichArea
- 2_05_Room1
- 2_05_Room2
- 2_05_Room3
- 2_05_Room4
- 2_05_Room5
- 2_05_Room6
- 2_05_RussellOffBike
- 2_05_TadsBlock
- 2_05_TadsYard
- 2_05_Tree01
- 2_05_Tree02
- 2_05_WallBreak01
- 2_05_WallBreak02

### 2_06.dat

Count: 2

- 2_06_BikeZone
- 2_06_Theater

### 2_07_BeachA.dat

Count: 7

- 2_07_GORD_ON_DOCK
- 2_07_OUTSIDEDOOR
- 2_07_OUT_OF_AREA
- 2_07_OUT_OF_AREA_WARN
- 2_07_PREPPY_NINJA_TRIG
- 2_07_REAR_PIER
- 2_07_behindDoor

### 2_08.dat

Count: 11

- 2_08_BifAttackTrig
- 2_08_DoorStairs
- 2_08_FirstFloorTrig
- 2_08_FoyeurDoor
- 2_08_PlantTarget
- 2_08_SecndFloorTrig
- 2_08_SolariumEntrance
- 2_08_StairPreppy
- 2_08_ThrdFloorTrig
- 2_08_ToSolarium
- 2_08_TriggerStairs

### 2_09.dat

Count: 1

- Cutscene02

### 2_B.dat

Count: 9

- 2_B_BOSS_FIGHT
- 2_B_BOSS_FIGHT_INTRO
- 2_B_DRBRACE_DOOR
- 2_B_DRBRACE_DOOR01
- 2_B_PLAYER_NEAR_BAR
- 2_B_SECOND_ATTACK
- 2_B_Tether
- DRBrace
- DRBrace01

### 2_G2.dat

Count: 11

- 2_G2_ballToss
- 2_G2_dunkTank
- 2_G2_excluderCoaster
- 2_G2_excluderFerris
- 2_G2_excluderSquid
- 2_G2_freakShow
- 2_G2_highStriker
- 2_G2_pinkyAngryFail
- 2_G2_pinkyArrived
- 2_G2_shootingGallery
- 2_G2_ticketShop

### 2_S02.dat

Count: 13

- 2_S02CarSpeedup
- 2_S02_CarFailTrigger
- 2_S02_CarInDriveway
- 2_S02_CarInit
- 2_S02_CarTrigger
- 2_S02_Cop1
- 2_S02_Cop_Car1_Stop
- 2_S02_Cop_Car2_Stop
- 2_S02_End_Trigger1
- 2_S02_HATTRICKYARD
- 2_S02_HattrickNIS
- 2_S02_Intro_Failure
- 2_S02_PathVolume

### 2_S04.dat

Count: 18

- 2_S04Sheet3NIS
- 2_S04_AutoShopArea
- 2_S04_LibraryJump
- 2_S04_Nerd_Escape
- 2_S04_SchoolPop
- 2_S04_Sheet1
- 2_S04_Sheet2
- 2_S04_Sheet3
- 2_S04_Sheet3Create
- 2_S04_Sheet3Outer
- 2_S04_Sheet4
- 2_S04_Sheet4Inner
- 2_S04_Sheet5E1
- 2_S04_Sheet5E2
- 2_S04_Sheet5Start
- 2_S04_StartSheet2
- 2_S04_TetherBully
- 2_S04_TrashCan

### 2_S05.dat

Count: 12

- 2_S05_AwfulHack
- 2_S05_DisturbRadius
- 2_S05_DrugAlley
- 2_S05_Excluder
- 2_S05_Target
- 2_S05_TeacherArea
- 2_S05_TeacherRadius
- 2_S05_TrashCan1
- 2_S05_TrashCan2
- 2_S05_TrashCan3
- 2_S05_Tree
- 2_S05_Tree2

### 2_S06.dat

Count: 9

- 2_S06_PrefectWander
- 2_S06_latticeCam
- 2_S06_mandySpeak
- 2_S06_stg1Burton
- 2_S06_stg1_Busted
- 2_S06_stg3Burton
- 2_S06_stg3LeftDorm
- 2_S06_triggerLoadSchool
- 2_S06_tutLattice

### 2_S06b.dat

Count: 13

- 2_S06B_AngieChristyRoom
- 2_S06B_EuniceFrontDoor
- 2_S06B_MandyRoom
- 2_S06B_atticEntry
- 2_S06B_launchAsian
- 2_S06B_makeGirlsStudy
- 2_S06B_pinkyRoom
- 2_S06B_showerWarn
- 2_S06B_trigger01
- 2_S06B_trigger02
- 2_S06B_trigger03
- 2_S06B_triggerShowerDialogue
- 2_S06B_upstairsHallway

### 3_01.dat

Count: 5

- 3_01_KissFinal
- 3_01_MeetClimb
- 3_01_MissionArea
- 3_01_MissionBlock
- 3_01_OnRoof

### 3_01A.dat

Count: 1

- barricade102

### 3_01D.dat

Count: 1

- 3_01D_RUDY

### 3_02.dat

Count: 7

- 3_02_BUSINESSAREA
- 3_02_PARKENTRANCE
- 3_02_SPAWNER01
- 3_02_SPAWNER02
- 3_02_SPAWNER03
- 3_02_SPAWNER04
- 3_02_SPAWNER05

### 3_02_BMX.dat

Count: 1

- BMXParkJump01

### 3_02_new.dat

Count: 7

- 3_02_BUSINESSAREA
- 3_02_PARKENTRANCE
- 3_02_SPAWNER01
- 3_02_SPAWNER02
- 3_02_SPAWNER03
- 3_02_SPAWNER04
- 3_02_SPAWNER05

### 3_03.dat

Count: 5

- triggerBackAlley
- triggerBalcony
- triggerBalcony2
- triggerLola
- triggerTadTether

### 3_04.dat

Count: 5

- 3_04_algieFlee
- 3_04_cornScream2
- 3_04_corneliusCut
- 3_04_loadBikes
- 3_04_stg4_Return

### 3_05.dat

Count: 16

- 3_05_1StartUpstairs
- 3_05_2CatwalkStart
- 3_05_3NortonsDoor
- 3_05_Ambush
- 3_05_BossFightTrigger
- 3_05_Catwalk2
- 3_05_ExitGreasers1
- 3_05_Hammerwall01
- 3_05_Hammerwall02
- 3_05_Hammerwall03
- 3_05_Hammerwall04
- 3_05_Hammerwall05
- 3_05_SecondFloor
- 3_05_StartCatwalk
- 3_05_StartShooting
- 3_05_StartShooting2

### 3_06New.dat

Count: 13

- 306PoorArea
- 3_06_FailTrig
- 3_06_FightTrig
- 3_06_InnerArea
- 3_06_OuterArea
- AmbientEvent1
- AmbientEvent2
- FinalFightTrig
- GordYell
- ManicCopCar
- Stag1Trig
- Stag2Trig
- ThirdFight

### 3_07.dat

Count: 1

- 3_07_StartConv

### 3_08.dat

Count: 4

- 3_08_BackToRoomTrig
- 3_08_Intercom_Trigger
- 3_08_RunStart
- 3_08_SchoolPop

### 3_B.dat

Count: 10

- 3B_CopsSpeedUp
- 3_B_MAGNET
- 3_B_STAGE_2_TRIGGER
- AREA_AROUND_BUTTON
- GREASERS_JET01
- GREASERS_JET02
- GREASERS_JET03
- GREASERS_JET04
- GREASERS_JET05
- JohnnyRamble02

### 3_B_BIKE_STUFF.dat

Count: 5

- 3_B_BIKE_REGION_NE
- 3_B_BIKE_REGION_NW
- 3_B_BIKE_REGION_SE
- 3_B_BIKE_REGION_SW
- 3_B_REGION_S

### 3_G3.dat

Count: 6

- 3_G3_CheeringCrowd
- 3_G3_MoveLola
- 3_G3_Tree1
- 3_G3_Tree2
- 3_G3_Tree3
- 3_G3_Tree4

### 3_R07.dat

Count: 1

- 5_T1_BikeGarage

### 3_R09_Dropouts.dat

Count: 5

- 3_R09_AreaT01
- 3_R09_AreaT02
- 3_R09_MainArea
- 3_R09_SpawnT01
- 3_R09_SpawnT02

### 3_R09_Greasers.dat

Count: 5

- 3_R09_AreaT01
- 3_R09_AreaT02
- 3_R09_MainArea
- 3_R09_SpawnT01
- 3_R09_SpawnT02

### 3_R09_Jocks.dat

Count: 4

- 3_R09_AreaT01
- 3_R09_AreaT02
- 3_R09_SpawnT01
- 3_R09_SpawnT02

### 3_R09_Nerds.dat

Count: 4

- 3_R09_BasementTrigger
- 3_R09_SpawnT01
- 3_R09_SpawnT02
- 3_R09_Upstairs

### 3_R09_Preppies.dat

Count: 4

- 3_R09_AreaT01
- 3_R09_AreaT02
- 3_R09_SpawnT01
- 3_R09_SpawnT02

### 3_S03.dat

Count: 8

- 3_S03_failAlley
- 3_S03_failGreaser
- 3_S03_failPool
- 3_S03_objectiveAlley
- 3_S03_objectiveGreaser
- 3_S03_objectivePool
- 3_S03_parkingLot
- 3_S03_poolArea

### 3_S03T.dat

Count: 15

- 3_S03T_H_Car_Drop7_Stop
- 3_S03T_OPEN_GATE_T
- 3_S03T_Test_1
- 3_S03T_Test_1_Activate
- 3_S03T_Test_2
- 3_S03T_Test_2_Activate
- 3_S03T_Test_3
- 3_S03T_Test_3_Activate
- 3_S03T_Test_4
- 3_S03T_Test_4_Activate
- 3_S03T_Test_5
- 3_S03T_Test_5_Activate
- 3_S03T_Test_6
- 3_S03T_Test_6_Activate
- 3_S03_TEMP_DOORTELEPORT

### 3_S09.dat

Count: 23

- 3_S09_AmbushTrigger01
- 3_S09_AmbushTrigger02
- 3_S09_AmbushTrigger03
- 3_S09_Breakable01
- 3_S09_Breakable02
- 3_S09_Breakable03
- 3_S09_Breakable04
- 3_S09_Breakable05
- 3_S09_Breakable06
- 3_S09_Breakable07
- 3_S09_Breakable08
- 3_S09_Breakable09
- 3_S09_Breakable10
- 3_S09_Cover01
- 3_S09_Cover02
- 3_S09_Cover03
- 3_S09_Cover04
- 3_S09_Cover05
- 3_S09_CoverArea
- 3_S09_CoverCrate01
- 3_S09_CoverCrate02
- 3_S09_Dumpster01
- 3_S09_LeavingTrigger

### 3_S10.dat

Count: 12

- 3_S10_ATagsLoad
- 3_S10_BTagsLoad
- 3_S10_CTagsLoad
- 3_S10_DTagsLoad
- 3_S10_PoorArea
- 3_S10_TUT_TAG
- 3_S10_TutTrigger
- 3_S10_Tut_Tag02
- 3_S10_Tut_Tag03
- 3_S10_TutorialStart
- 3_S10_underBridge
- 3_S_10_FailTrigger

### 3_S11.dat

Count: 15

- 3_S11_Asylum_Gate_Warning
- 3_S11_Asylum_Gate_Warning2
- 3_S11_Break_Out
- 3_S11_Fire01
- 3_S11_Fire02
- 3_S11_Fire03
- 3_S11_Fire04
- 3_S11_Fire05
- 3_S11_Fire06
- 3_S11_Fire07
- 3_S11_Galloway_Trigger
- 3_S11_Inside_Asylum
- 3_S11_PHILLIPS_REUNION
- 3_S11_Phillips_Car_Stop
- 3_S11_Player_On_A_Grounds

### 3_XM.dat

Count: 1

- 3_XM_SpawnTrigger

### 4_01.dat

Count: 13

- 4_01_artNorth
- 4_01_artSouth
- 4_01_christySpeech
- 4_01_girlsDormBathroom
- 4_01_gymInsideDoor
- 4_01_gymTunnel
- 4_01_launchEunice
- 4_01_mandyRoom
- 4_01_mandyRoomBusted
- 4_01_mandyRoomWarn
- 4_01_showerRoom
- 4_01_showerWarn
- 4_01_tutLattice

### 4_02.dat

Count: 30

- 4_02_Bar_01
- 4_02_Bar_02
- 4_02_Bar_03
- 4_02_Breaker_Box
- 4_02_Delete_Wave1
- 4_02_Delete_Wave3
- 4_02_Eavesdrop
- 4_02_Finale
- 4_02_GateKeeper
- 4_02_KeyPad
- 4_02_NERDS
- 4_02_O_R1_1T
- 4_02_O_R2_1T
- 4_02_O_WN1_1T
- 4_02_O_WN2_1T
- 4_02_O_WN3_1T
- 4_02_O_WN4_1T
- 4_02_ObsDoor
- 4_02_ObsDoorCheck
- 4_02_PREFECT1
- 4_02_PREFECT2
- 4_02_P_Wave2
- 4_02_P_Wave3
- 4_02_P_Wave4
- 4_02_Player_On_CannonT
- 4_02_Player_Out_Of_Lib
- 4_02_Spotted_Scout
- 4_02_Spud_Cannon
- 4_02_Spud_Tripod
- 4_02_TEMP_Cannon_Line2

### 4_03.dat

Count: 20

- 4_03_Bar_05_01
- 4_03_Bar_05_02
- 4_03_Bar_Blip_Trigger
- 4_03_Cannon
- 4_03_Cannon_Tripod
- 4_03_Jock_Past_Water
- 4_03_Leave1
- 4_03_Leave2
- 4_03_Ob_Bar1
- 4_03_Ob_Bar2
- 4_03_Ob_Bar3
- 4_03_Ob_Bar4
- 4_03_Ob_Grounds
- 4_03_ObsDoor
- 4_03_Open_Door
- 4_03_Open_Door2
- 4_03_Player_To_Far
- 4_03_SetUp_Nerds
- 4_03_TETHER_BAR_04
- 4_03_Trigger_Wave1

### 4_04.dat

Count: 23

- 4_04_CTRLROOM
- 4_04_ENDMINE
- 4_04_EXIT
- 4_04_JOCKNIS
- 4_04_MAZE_HALL_05
- 4_04_MAZE_HALL_07
- 4_04_MAZE_HALL_08
- 4_04_MINE_ESCAPE
- 4_04_MONITOR01
- 4_04_MONITOR02
- 4_04_MONITOR03
- 4_04_MineNerds1
- 4_04_MineNerds2
- 4_04_MineNerds3
- 4_04_NerdTrig
- 4_04_REACHED_FUNHOUSE
- 4_04_Reaper01
- 4_04_Reaper02
- 4_04_Reaper03
- 4_04_Reaper04
- 4_04_Reaper05
- 4_04_Reaper06
- 4_04_ReaperRoom

### 4_05.dat

Count: 13

- 4_05_FIELD
- 4_05_failAlley
- 4_05_failMain
- 4_05_failPath
- 4_05_mascotPOI1
- 4_05_mascotPOI2
- 4_05_mascotPOI3
- 4_05_mascotPOI4
- 4_05_mascotPOI5
- 4_05_nerdAmbush
- 4_05_warnAlley
- 4_05_warnMain
- 4_05_warnPath

### 4_05cut.dat

Count: 1

- 4_05cut_fakeDoor

### 4_06.dat

Count: 29

- 4_06_BIB01
- 4_06_BIB02
- 4_06_BIB03
- 4_06_Bench_01
- 4_06_Bench_01A
- 4_06_Bench_02
- 4_06_Bench_02A
- 4_06_Bench_03
- 4_06_Bench_03A
- 4_06_Bench_04
- 4_06_Bench_04A
- 4_06_Cooler
- 4_06_Cooler_Location
- 4_06_DockingTrigger
- 4_06_Duffle_Bag
- 4_06_Field01
- 4_06_Field02
- 4_06_Field03
- 4_06_Field_Zone
- 4_06_GatObjective
- 4_06_Hack_Switch
- 4_06_InsideDockingTrigger
- 4_06_Load_Field
- 4_06_OOB01
- 4_06_OOB02
- 4_06_OOB03
- 4_06_OPAENDTRIGG
- 4_06_OPCENDTRIGG
- 4_06_OutsideGate

### 4_B1.dat

Count: 8

- 4_B1_EARNEST_PATTERN02
- 4_B1_EARNEST_PATTERN03
- plat_North
- plat_South
- plat_West
- platform_South
- platform_West
- turret_top

### 4_B2.dat

Count: 16

- FootballField
- TetherD101
- TetherD102
- TetherD103
- TetherD104
- TetherD105
- TetherD201
- TetherD202
- TetherD203
- TetherD204
- TetherD205
- TetherD301
- TetherD302
- TetherD303
- TetherD304
- TetherD305

### 4_G4.dat

Count: 19

- 4_G4_BleacherPervert
- 4_G4_BusPoster02
- 4_G4_BusPoster08
- 4_G4_BusTag2
- 4_G4_BusTag8
- 4_G4_LIBNERDS
- 4_G4_LeftTown
- 4_G4_NerdComics
- 4_G4_OutOfGrounds
- 4_G4_SchoolPoster02
- 4_G4_SchoolPoster03
- 4_G4_SchoolPoster04
- 4_G4_SchoolTag2
- 4_G4_SchoolTag3
- 4_G4_SchoolTag4
- 4_G4_TaggingTrig
- 4_G4_TaggingTrig3
- 4_G4_TiltPost1
- 4_G4_TiltTag1

### 4_S11T.dat

Count: 17

- 4_S11_AtticPlank01
- 4_S11_AtticPlank02
- 4_S11_AtticPlank03
- 4_S11_DockerDoor
- 4_S11_EndTrigger
- 4_S11_FieldTrigger
- 4_S11_GymBag
- 4_S11_GymBagTrigger
- 4_S11_JPhoto
- 4_S11_JockDiscoveryTrigger
- 4_S11_LockedDoor
- 4_S11_NerdTrigger
- 4_S11_PaddleTrigger
- 4_S11_RandomTeacherTrigger
- 4_S11_SafeZone
- 4_S11_SafeZoneA
- 4_S11_SafeZoneB

### 4_S12.dat

Count: 3

- 4_S12_MSPHILLIPS
- 4_S12_PEANUTBIKE
- 4_S12_PEANUTBIKE2

### 5_01.dat

Count: 22

- 5_01_Meet_Librarian
- 5_01_RatSpawnT01
- 5_01_RatSpawnT02
- 5_01_RatSpawnT03
- 5_01_RatSpawnT04
- 5_01_RatSpawnT05
- 5_01_RatSpawnT06
- 5_01_RatSpawnT07
- 5_01_RatSpawnT08
- 5_01_RatSpawnT09
- 5_01_RatSpawnT10
- 5_01_RatSpawnT11
- 5_01_RatSpawnT12
- 5_01_RatSpawnT13
- 5_01_RatSpawnT14
- 5_01_RatSpawnT15
- 5_01_RatSpawnT16
- 5_01_RatSpawnT17
- 5_01_RatSpawnT18
- 5_01_RatSpawnT19
- 5_01_RatSpawnT20
- 5_01_main_room_tr

### 5_02.dat

Count: 22

- 5_02_BigSmoke
- 5_02_BonfireTrigger01
- 5_02_BonfireTrigger02
- 5_02_DepopRichArea
- 5_02_DepopulateDocks
- 5_02_DockPartyCreate
- 5_02_FailTrigger
- 5_02_FinalNIS
- 5_02_Flame01
- 5_02_Flame02
- 5_02_Flame03
- 5_02_GameArea
- 5_02_GreaserHangout
- 5_02_InWarehouse
- 5_02_NearNIS
- 5_02_OnBarge
- 5_02_PortExit
- 5_02_RatCrate
- 5_02_StartRatPhoto
- 5_02_TrophyPile
- 5_02_WarehouseUpstairs
- 5_02_WarehouseUpstairs02

### 5_03.dat

Count: 30

- 5_03_1st_Floor_1st_Hall
- 5_03_Asylum_Grounds_SetUp
- 5_03_BlockB
- 5_03_Control_Room_Door
- 5_03_DOW_1
- 5_03_DOW_2
- 5_03_DOW_3
- 5_03_Exit
- 5_03_FIRE01
- 5_03_FIRE02
- 5_03_FIRE03
- 5_03_FIRE04
- 5_03_FIRE05
- 5_03_FRONT_GATE_LINE
- 5_03_GameOver
- 5_03_Gen_Johnny
- 5_03_Inside_Asylum
- 5_03_JOHNNY_END_TRIGGER
- 5_03_Johnny_Goto1
- 5_03_Johnny_Trig1
- 5_03_Johnny_Yelling
- 5_03_LEFT
- 5_03_Leaving
- 5_03_OnGrounds
- 5_03_Orderly_CS1_1
- 5_03_Player_In_CR
- 5_03_Rec_Room
- AsyBars
- AsyBars01
- AsyBars02

### 5_04.dat

Count: 40

- 5_04_AMBUSH_01
- 5_04_AMBUSH_02
- 5_04_AMBUSH_03
- 5_04_AMBUSH_04
- 5_04_AMBUSH_05
- 5_04_BANNERS_01
- 5_04_BANNERS_02
- 5_04_BANNERS_03
- 5_04_BANNERS_04
- 5_04_BANNERS_05
- 5_04_BANNERS_06
- 5_04_BANNERS_07
- 5_04_BANNERS_08
- 5_04_BANNERS_09
- 5_04_BANNERS_10
- 5_04_BANNERS_11
- 5_04_BANNERS_12
- 5_04_BANNERS_13
- 5_04_BIKE_STOP_01
- 5_04_BIKE_STOP_02
- 5_04_CHANGEROOM
- 5_04_COP_START_01
- 5_04_COP_START_02
- 5_04_CREATE_FOURTH_PEDS
- 5_04_DOOR_HACK
- 5_04_DO_CHAT
- 5_04_DO_ESCAPE
- 5_04_DO_GOAL
- 5_04_DO_NEAR_BIKE
- 5_04_DO_STOP_01
- 5_04_GYMHOOP
- 5_04_GYMWALL
- 5_04_LASTAMBUSH
- 5_04_LIGHT_01
- 5_04_LIGHT_02
- 5_04_LIGHT_03
- 5_04_LIGHT_04
- 5_04_OTHERROUTE
- 5_04_PREVENT01
- 5_04_PREVENT02

### 5_05.dat

Count: 13

- 5_05_Alley
- 5_05_BoltCutters
- 5_05_BurtonTether
- 5_05_ClearMower
- 5_05_DogFood
- 5_05_ExcludedMeatFactory
- 5_05_FactoryArea
- 5_05_LastPotty
- 5_05_POTTY
- 5_05_Park
- 5_05_ParkOut
- 5_05_RunAwayZoe
- 5_05_TBoneTarget

### 5_06.dat

Count: 9

- 5_06_BarricadeCrash
- 5_06_BarricadeDoor
- 5_06_BikeTrigger
- 5_06_Bridge
- 5_06_EndTrigger
- 5_06_RussellDoor
- 5_06_RussellGarage
- 5_06_RussellGate
- 5_06_RussellTrigger

### 5_07.dat

Count: 30

- 5_07_BarricadeNIS
- 5_07_ChemEntrance
- 5_07_DoorLocked01
- 5_07_DoorLocked02
- 5_07_ElectricDoor
- 5_07_Fire01
- 5_07_FirstZoe
- 5_07_MissionInit
- 5_07_OmarFight
- 5_07_OutsideTheOffice
- 5_07_PartThree
- 5_07_PedAttack01
- 5_07_PedAttack02
- 5_07_PedAttack03
- 5_07_Ranged01
- 5_07_Ranged02
- 5_07_SecondZoe
- 5_07_SecuritySwitch
- 5_07_SiloAttack01
- 5_07_Slaughterhouse
- 5_07_Spawner01
- 5_07_Spawner02
- 5_07_TrainSwitch
- 5_07_TrainSwitch02
- BikeFire01
- BikeFire02
- BikeFire03
- BikeFire04
- BikeFire05
- BikeFire06

### 5_09.dat

Count: 17

- 5_09_Ambush
- 5_09_CityHallArea
- 5_09_CityHallTag2
- 5_09_CityHallTag3
- 5_09_CityHall_Building
- 5_09_CityHall_Grounds
- 5_09_CityHall_Tag
- 5_09_CityHall_Tower
- 5_09_CityHall_Wall_Climbed
- 5_09_DogYard
- 5_09_Earnest_Outdoors
- 5_09_GreaserLoad
- 5_09_Greaser_Safezone
- 5_09_Paint_Yard
- 5_09_PhotoOp
- 5_09_Players_Room
- 5_09_TowerTop

### 5_Ba.dat

Count: 18

- 5_B_CRAWL
- 5_B_ChemCamShot
- 5_B_ChemCamShot02
- 5_B_DEBUG_EDGAR
- 5_B_ENTRANCE
- 5_B_FALL_INTO_SLUDGE
- 5_B_FINALSTAGE
- 5_B_GRAB_GOOD
- 5_B_LIFTDOWN
- 5_B_LIFTUP
- 5_B_LadderCamShot
- 5_B_LadderCamShot02
- 5_B_LadderCamShot03
- 5_B_LowStaircase
- 5_B_STAGE2_START
- 5_B_STEAMAREA
- 5_B_SecDoor1
- 5_B_SecDoor2

### 5_G5.dat

Count: 11

- 5_G5_GroundDoorExit
- 5_G5_Ladder04
- 5_G5_WHBackDoor
- 5_G5_WHFrontDoor
- 5_G5_WareDoorZoe
- 5_G5_Zone01
- 5_G5_Zone02
- 5_G5_Zone03
- 5_G5_Zone04
- 5_G5_finish
- 5_G5_meet_zoe

### 6_01.dat

Count: 1

- 6_01_PRINCIPALTRIG

### 6_02.dat

Count: 40

- 602_LibEntrance
- 6_02_WonderMeats
- 6_03_Fail01
- 6_03_Fail02
- 6_03_Fail03
- 6_03_GetAway
- 6_03_GymPop
- 6_03_HallPopOverride
- 6_03_NISJOCK01
- 6_03_NISJOCK02
- 6_03_NISJOCK03
- 6_03_NISJOCK04
- 6_03_NISNERD01
- 6_03_NISNERD02
- 6_03_NISNERD03
- 6_03_NISNERD04
- 6_03_NISNERD05
- 6_03_WarnFail01
- 6_03_WarnFail02
- 6_03_WarnFail03
- BitchFight1
- BitchFight2
- CopCar
- EntryToWondMeat
- ExitToWondMeat
- FactoryEntrance
- GarageRoofTrig
- GarageTrig
- GirlsDormTrig
- GirlsTrig
- HarringtonTrig
- IndustrialGates
- LibTrig
- PowerStationTrig
- SchoolEntranceTrig
- SchoolRoofTrig
- SchoolSideTrig
- SchoolTrig
- tschool_FrontGate
- tschool_ParkingGate

### 6_02a.dat

Count: 4

- 6_02A_BACKROUTE_STUDENTS
- 6_02A_IA_COPS
- 6_02A_SCHOOLFRONT_COPS
- 6_02A_SF_GIRLS

### 6_02gdorm.dat

Count: 11

- 6_02g_bottomStairs
- 6_02g_downstairs
- 6_02g_entrance
- 6_02g_fireVase02
- 6_02g_johnny
- 6_02g_livingroom
- 6_02g_loadPeds
- 6_02g_norton
- 6_02g_vase01
- 6_02g_vase02
- 6_02g_vase03

### 6_B.dat

Count: 1

- BellTowerCamera

### 6_Ba.dat

Count: 18

- 6_B_BELLS_ONE
- 6_B_BELLS_THREE
- 6_B_BELLS_TWO
- 6_B_FIRSTPLANKRUN
- 6_B_GARY_THROW_1
- 6_B_GARY_THROW_2
- 6_B_GARY_TRIGGER_1
- 6_B_GARY_TRIGGER_2
- 6_B_GARY_TRIGGER_3
- 6_B_GARY_TRIGGER_4
- 6_B_GARY_TRIGGER_5
- 6_B_GARY_TRIGGER_6
- 6_B_GLASS_TRIGGER
- 6_B_LADDER1_BEGIN
- 6_B_LADDER2_BEGIN
- 6_B_OFFROOF
- 6_B_START
- 6_B_SchoolRoofTop

### AreaTran.dat

Count: 36

- BikeBusiness
- BoysDormMain
- BusinessBike
- BusinessFirework
- BusinessGrocery
- DISABLED_SV_LibMain
- Disabled_SV_AutoMain
- Disabled_SV_BoxingRich
- Disabled_SV_ClothMain
- Disabled_SV_EnglishSchool
- Disabled_SV_GymMain
- Disabled_SV_PrincipalSchool
- Disabled_SV_Staff
- FireworkBusiness
- GroceryBusiness
- MainAuto
- MainBoysDorm
- MainGym
- MainPrep
- MainSchool
- RichBoxing
- SV_BDormCrawl
- SV_BioSchool
- SV_CarnivalFunhouse
- SV_ChemSchool
- SV_ExtBDormCrawl
- SV_GirlsDorm
- SV_GirlsDormExit
- SchoolBio
- SchoolCaf1
- SchoolCaf2
- SchoolChem
- SchoolEnglish
- SchoolMain
- SchoolNurse
- SchoolPrincipal

### BDorm_Doors.dat

Count: 9

- BdrDoorDownstairs1
- BdrDoorDownstairs2
- BdrDoorDownstairs4
- BdrDoorDownstairs5
- BdrDoorDownstairs6
- BdrDoorDownstairs7
- BdrDoorDownstairs8
- DT_DormExitDoorL
- DormExitDoorR

### BMX_Rumble.dat

Count: 1

- BMX_Warning_Trig

### Barricade_Triggers.dat

Count: 2

- IndustrialBarricade
- PoorBarricade

### Boxing.dat

Count: 7

- BoxHalfTheRing
- Boxing_Corner1
- Boxing_Corner2
- Boxing_Corner3
- Boxing_Corner4
- Corner_Check1
- Corner_Check3

### BoysDorm.dat

Count: 2

- PLAYER_ROOM
- SaveBookBoysDorm

### C3.dat

Count: 1

- C3_MAT_BOUNDARY

### C5.dat

Count: 40

- AcrossGymBack
- AngelStatue
- AutoGarage
- AutoShop
- AutoShopSide
- BDormFlag1
- BleachersL
- BleachersR
- C5_PedEvent01
- C5_PedEvent02
- C5_PedEvent03
- C5_WorkingOut1
- C5_WorkingOut2
- C5_WorkingOut3
- EquipmentRoom
- FlagLeftSchool
- FlagRightSchool
- FootballFieldEntrance
- GDormBackDr
- GDormEntrance
- GlassDome
- Gymnasium
- GymnasiumBack
- LibraryArch
- LibraryL
- LibraryR
- ParkingArchway
- PreppyL
- PreppyR
- SchoolBackR
- SchoolEntrL1
- SchoolEntrL2
- SchoolEntrR1
- SchoolEntrR2
- SchoolSecondFloor
- SchoolTower
- StatueL
- StatueR
- TrophyL
- TrophyR

### C6.dat

Count: 1

- C6_ShopBike

### CarnStore.dat

Count: 1

- StoreCarn_Area

### CarnStrik.dat

Count: 1

- HighStrikerExcluder

### CarnivalRides.dat

Count: 2

- CoasterExitTrigger
- ExitFerrisTrigger

### Chapt1Trans.dat

Count: 2

- tschool_FrontGate
- tschool_ParkingGate

### Chapt5Trans.dat

Count: 1

- C5T_POP

### ChemPlantAcid01.dat

Count: 1

- ChemPlantAcid01

### ChristmasTree.dat

Count: 1

- ChristmasTreeExclude

### EasyDrugs.dat

Count: 6

- EasyDrugs_Trash01
- EasyDrugs_Trash02
- EasyDrugs_Trash03
- EasyDrugs_Trash04
- EasyDrugs_Trash05
- EasyDrugs_Trash06

### Football_Paths.dat

Count: 1

- FootFieldTrig

### FraffyMachine.dat

Count: 1

- FRAFFY

### FreakShow.dat

Count: 4

- DT_FreakShow_Entrance
- DT_FreakShow_Exit
- FreakShow_MidgetFight
- FreakShow_Midgets

### Garages.dat

Count: 4

- Garage_BusinessArea
- Garage_PoorArea
- Garage_RichArea
- Garage_SchoolGrounds

### GarbPickDowntown.dat

Count: 2

- gd_GameArea
- gd_TrashArea

### GarbPickPoor.dat

Count: 5

- pa_GameArea
- pa_Hobo1Area
- pa_Hobo2Area
- pa_Hobo3Area
- pa_TrashArea

### GarbPickSchool.dat

Count: 2

- gs_GameArea
- gs_TrashArea

### Gdorm.dat

Count: 11

- DT_gdorm_DoorLExit
- DT_gdorm_doorL
- GDorm_GirlsOnly
- GDorm_PopOverride
- GDorm_Stall01
- GDorm_Stall02
- GDorm_UpperDoor
- GDorm_UpperDoorStorage
- RAIL_GDORM01
- RAIL_GDORM02
- gdorm_DoorR

### Global.dat

Count: 11

- 2_G2_ballTossExcluderInside
- 2_G2_ballTossExcluderOutside
- 2_G2_dunkExcluderOutside
- 2_G2_shootingExcluderInside
- 2_G2_shootingExcluderOutside
- GDormExitExclude
- JOHNNYONTHESPOT
- PO_House
- PUN_BDORM
- PUN_GDORM
- RAIL_HHOUSE01

### GoKart.dat

Count: 1

- Race3BrakeTutorial

### GoKart_Outdoor.dat

Count: 6

- BeachNoGoArea
- DePopBeachAreaRace
- DePopIndustrialAreaRace
- DePopRichAreaRace
- IndustrialNoGoArea
- RichNoGoArea

### GraffitiPunishment.dat

Count: 7

- DowntownGameArea
- GC1A_GameArea
- PoorDepop
- PoorGameArea
- SchoolDepop
- SchoolGameArea
- dowtownDepop

### GraffitiTest.dat

Count: 8

- BigTag1
- BigTag2
- BigTag3
- GreaserTag
- GreaserTagArea
- smallTag
- tag1
- tutorialTag

### HighStrikerProps.dat

Count: 1

- HSdinger

### Janitors.dat

Count: 17

- AfterSteam
- AniBroom
- DT_Janitor_MainExit
- DT_Janitor_SchoolExit
- JanDoors00
- JanDoors01
- JanDoors02
- JanDoors03b
- JanElectricProxy
- JanExtraFire
- JanFire01
- JanFire02
- JanSteamProxy
- JanSwtch00
- JanSwtch01
- JanSwtch02
- JanSwtch03a

### LawnMowing.dat

Count: 6

- LM1_GameArea
- LM2_GameArea
- LM3_Depop
- LM3_GameArea
- LM4_GameArea
- LM5_GameArea

### MGBaseballToss.dat

Count: 27

- BatterEight
- BatterFive
- BatterFour
- BatterNine
- BatterOne
- BatterSeven
- BatterSix
- BatterThree
- BatterTwo
- BonusTarget
- CatcherFive
- CatcherFour
- CatcherOne
- CatcherSeven
- CatcherSix
- CatcherThree
- CatcherTwo
- InstBatter
- InstCatcher
- InstUmpire
- UmpireFive
- UmpireFour
- UmpireOne
- UmpireSeven
- UmpireSix
- UmpireThree
- UmpireTwo

### MGDunkTank.dat

Count: 5

- DunkBackBoard
- DunkBttn
- DunkSeat
- DunkTank
- DunkTankExcluder

### MGLawnMowing2P.dat

Count: 5

- MGL2_01_GameArea
- MGL2_02_GameArea
- MGL2_03_GameArea
- MGL2_04_GameArea
- MGL2_05_GameArea

### MGShooting.dat

Count: 20

- MGS_Bonus01
- MGS_Bottle01
- MGS_Bottle02
- MGS_Bottle03
- MGS_Bottle04
- MGS_Bottle05
- MGS_Bottle06
- MGS_Bottle07
- MGS_Bottle08
- MGS_Cowboy01
- MGS_Cowboy02
- MGS_Cowboy03
- MGS_Cowboy04
- MGS_Robber01
- MGS_Robber02
- MGS_Robber03
- MGS_Robber04
- MGS_TutBottle
- MGS_TutCowboy
- MGS_TutRobber

### MGShooting2P.dat

Count: 20

- MGS2_Bonus01
- MGS2_Bottle01
- MGS2_Bottle02
- MGS2_Bottle03
- MGS2_Bottle04
- MGS2_Bottle05
- MGS2_Bottle06
- MGS2_Bottle07
- MGS2_Bottle08
- MGS2_Cowboy01
- MGS2_Cowboy02
- MGS2_Cowboy03
- MGS2_Cowboy04
- MGS2_Robber01
- MGS2_Robber02
- MGS2_Robber03
- MGS2_Robber04
- MGS2_TutBottle
- MGS2_TutCowboy
- MGS2_TutRobber

### Mailboxes_Rich.dat

Count: 25

- Rich_MailBox01
- Rich_MailBox23
- Rich_MailBox24
- Rich_MailBox25
- Rich_Mailbox02
- Rich_Mailbox03
- Rich_Mailbox04
- Rich_Mailbox05
- Rich_Mailbox06
- Rich_Mailbox07
- Rich_Mailbox08
- Rich_Mailbox09
- Rich_Mailbox10
- Rich_Mailbox11
- Rich_Mailbox12
- Rich_Mailbox13
- Rich_Mailbox14
- Rich_Mailbox15
- Rich_Mailbox16
- Rich_Mailbox17
- Rich_Mailbox18
- Rich_Mailbox19
- Rich_Mailbox20
- Rich_Mailbox21
- Rich_Mailbox22

### MainMapZones.dat

Count: 6

- ZoneBusiness
- ZoneCarnival
- ZoneIndustrial
- ZonePoor
- ZoneRich
- ZoneSchool

### MainMap_bus.dat

Count: 10

- Bus_BUS
- Bus_Loc1
- Bus_Loc3
- Bus_Loc4
- Bus_Loc5
- Bus_Loc6
- Bus_Loc7
- Bus_Loc8
- Bus_Loc9
- Bus_LocX

### MiniGameTrigger.dat

Count: 3

- CARNY_ENTRANCE
- CARNY_GAMESAREA
- CARNY_GOKARTAREA

### New.dat

Count: 1

- New_Gate

### NursingPond.dat

Count: 1

- NursingPond

### PAn_Main.dat

Count: 51

- ASYLUM_FRONT_DOOR_R
- ASYLUM_FRONT_GATE_DOOR
- AlleyPiss1
- AlleyPiss2
- AlleyPiss3
- BDormTarg
- CityHallTarg
- DT_ASYLUM_FRONT_DOOR
- DT_ASYLUM_SIDE_EXIT
- DT_Observatory
- DT_TINDUST_CHEMEX_DOOR
- GDormTarg
- LibTarg
- MeatPlant_boltcutters_FDoorC01
- MeatPlant_hide_FDoorC02
- MeatPlant_hide_FDoorC03
- NerdPath_AsySwtch
- NerdPath_AsySwtch02
- NerdPath_BRDoor
- PAlleyPiss1
- PAlleyPiss2
- PAlleyPiss3
- PAlleyPiss4
- PoorTarg1
- PoorTarg2
- SOCCER_SHOOT_OUT_01
- SOCCER_SHOOT_OUT_02
- TINDUST_BAR_DOOR_01
- TINDUST_BAR_DOOR_02
- TINDUST_BAR_DOOR_03
- TINDUST_BAR_DOOR_PORT
- TINDUST_BAR_DOOR_SWITCH_01
- TINDUST_BAR_DOOR_SWITCH_02
- TINDUST_BAR_DOOR_SWITCH_03
- TINDUST_BAR_DOOR_SWITCH_PORT
- TINDUST_ELECTRIC_SHUTOFF
- TINDUST_FIRE_DOOR_01
- TINDUST_FIRE_DOOR_02
- TINDUST_GATE_SWITCH
- TINDUST_POWER_SWITCH_01
- TINDUST_POWER_SWITCH_02
- TINDUST_REDSTAR_GATE_01
- TINDUST_REDSTAR_SECURITY_DOOR
- TINDUST_SHDOOR_03
- TINDUST_SHDOOR_04
- TINDUST_SHDOOR_05
- TINDUST_SHDOOR_06
- TINDUST_SHDOOR_07
- TINDUST_TRAIN_SWITCH_01
- TINDUST_TRAIN_SWITCH_02
- trich_SprinklerSwitch

### PAn_Prep.dat

Count: 19

- DT_PrepToMain
- Door_PrepHouse_Foyer
- Door_PrepHouse_FoyerOut
- Door_PrepHouse_Gamble
- Door_PrepHouse_Lounge
- Door_PrepHouse_Lounge_02
- Door_PrepHouse_Stairs
- Door_PrepHouse_Stairs_Lower
- Door_PrepHouse_Stairs_Upper
- HouseThirdFloor
- PAn_Prep_Armor01
- PAn_Prep_Armor02
- PAn_Prep_Armor03
- PAn_Prep_Armor04
- PAn_Prep_Armor05
- PAn_Prep_Armor06
- PAn_Prep_ESCDoorR
- PAn_Prep_Weed
- PAnim_FlyTrap

### PAn_Rich.dat

Count: 3

- Rich_target1
- Rich_target2
- Rich_target3

### P_Snow1.dat

Count: 6

- ST1_dePopSnowArea
- lvl1GameArea
- snowPile1_01
- snowPile1_02
- snowPile1_03
- snowPile1_04

### P_Snow2.dat

Count: 8

- ST2_dePopSnowArea
- lvl2GameArea
- snowPile2_01
- snowPile2_02
- snowPile2_03
- snowPile2_04
- snowPile2_05
- snowPile2_06

### P_Snow3.dat

Count: 10

- ST3_dePopSnowArea
- lvl3GameArea
- snowPile3_01
- snowPile3_02
- snowPile3_03
- snowPile3_04
- snowPile3_05
- snowPile3_06
- snowPile3_07
- snowPile3_08

### P_Snow4.dat

Count: 9

- ST4_dePopSnowArea
- TEMPCar1
- TEMPCar2
- TEMPCar3
- lvl4GameArea
- snowStage4_01
- snowStage4_02
- snowStage4_04
- snowStage4_05

### P_Snow5.dat

Count: 11

- ST5_dePopSnowArea
- TEMPCar1
- TEMPCar2
- lvl5GameArea
- lvl5_gate
- lvl5_snowPile03
- lvl5_snowPile06
- lvl5_snowPile07
- lvl5_snowPile08
- lvl5_snowPile09
- lvl5_snowPile10

### P_Snow6.dat

Count: 14

- ST6_dePopSnowArea
- TEMPCar1
- TEMPCar2
- TEMPCar3
- lvl6GameArea
- lvl6_snowPile_04
- lvl6_snowPile_05
- lvl6_snowPile_06
- lvl6_snowPile_07
- lvl6_snowPile_08
- lvl6_snowPile_09
- lvl6_snowPile_10
- lvl6_snowPile_12
- lvl6_snowPile_14

### PaperRoute.dat

Count: 22

- PR_CarStart01
- PR_CarStart02
- PR_CarStart03
- PR_CarStart04
- PR_CarStart05
- PR_CheckEquip
- PR_DogStart00
- PR_DogStart01
- PR_DogStart02
- PR_DogStart03
- PR_DogStart04
- PR_HattrickYard
- PR_HillTop
- PR_JoggerTrigger
- PR_MailManStart01
- PR_MailManStart02
- PR_MailManStart03
- PR_OldLadyNorthStart
- PR_OldLadySouthStart
- PR_PaperPickupTrigger
- PaperRoute_Excluder
- Pr_HilltopExcluder

### PedTest.dat

Count: 2

- Chair1
- Chair2

### PhotoFilters.dat

Count: 8

- Burger
- CityHall
- Flea
- Silo
- Theatre
- Toys
- Water
- Wires

### PhotoZoom.dat

Count: 33

- AcrossGymBack
- AngelStatue
- AutoGarage
- AutoShop
- AutoShopSide
- BDormFlag1
- BleachersL
- BleachersR
- EquipmentRoom
- FlagLeftSchool
- FlagRightSchool
- GDormBackDr
- GDormEntrance
- GlassDome
- Gymnasium
- GymnasiumBack
- LibraryArch
- LibraryL
- LibraryR
- ParkingArchway
- PreppyL
- PreppyR
- SchoolBackR
- SchoolEntrL1
- SchoolEntrL2
- SchoolEntrR1
- SchoolEntrR2
- SchoolSecondFloor
- SchoolTower
- StatueL
- StatueR
- TrophyL
- TrophyR

### Population.dat

Count: 34

- BadPlaceTrigger
- BullyTurf
- Carnival
- ComicShopExclude
- DT_ComicShop
- DT_DropOutAlley
- DT_GASSTATION
- DT_GreaserAlley
- DownTown
- FieldOverride
- GraveYard
- Greasers
- IndustrialArea_DropOutEnclave
- Industrial_Docks
- Industrial_Sawmill
- Jocks
- Jocks_FootballField
- Nerds
- OutsideSchool1
- POOR_TENEMENTS
- PoorArea
- Poor_DropTurf1
- PopRoads1
- Preps
- RT_Tether
- RetirementTrigger
- RichArea
- RichArea_DownTown
- Rich_Area_Corner_Courtyard
- Rich_GreaserAlley
- Rich_GreaserAlley2
- SchoolArea
- SchoolBikeTrig
- School_Basketball_Court

### PriOffice.dat

Count: 2

- POfficeExclude
- PSecretary

### RaulTest.dat

Count: 7

- 3_S09_Cover01
- 3_S09_Cover02
- 3_S09_Cover03
- 3_S09_Cover04
- 3_S09_CoverArea
- 3_S09_Dumpster01
- 3_S09_LeavingTrigger

### RobertoTest.dat

Count: 3

- NerdEncounter
- SpawnKiss
- TicketPickup

### SP_Art_Room.dat

Count: 1

- Art_Room

### SP_Asylum.dat

Count: 7

- AssyInterTone01
- AssyMain02
- AssyMainDamaged
- AssyRecRoom
- AssyShowers
- AssylumMain
- Mourge

### SP_Auditorium.dat

Count: 1

- Auditorium

### SP_BMXTrack.dat

Count: 2

- BMX_BigRoom
- BMX_Room

### SP_Barber.dat

Count: 1

- BarberShop

### SP_Bike_Shop.dat

Count: 1

- BikeShop

### SP_BoxingRing.dat

Count: 4

- Box2ndFloor
- BoxMain01
- BoxMain02
- BoxStairs

### SP_BoysDorm.dat

Count: 3

- BoysDorm_GameRm
- BoysDorm_Halls
- BoysDorm_JimmysRoom

### SP_Chem_Lab.dat

Count: 1

- AMB_CHEMLAB

### SP_Chem_Plant.dat

Count: 3

- ChemPlantLower
- ChemPlantMain
- ChemPlantStairTunnel

### SP_ClassRoom.dat

Count: 1

- Amb_ClassRoom

### SP_Comic_Shop_Rich.dat

Count: 5

- ComicShop
- NerdComputerRoom
- NerdMainRoom
- NerdSmallRoom
- NerdStairwell

### SP_FreakShow.dat

Count: 4

- FreakShow_AmbEnter
- FreakShow_AmbExit
- FreakShow_Errie01
- FreakShow_Errie02

### SP_Girls_Dorm.dat

Count: 1

- GirlsDorm_Attic

### SP_GroceryStore.dat

Count: 1

- GroceryStore

### SP_HouseOfMirrors.dat

Count: 9

- Funhouse_Auditorium
- Funhouse_ControlRm_Graveyard
- Funhouse_HauntedMaze
- Funhouse_MineShaft
- Funhouse_Sound_Graveyard
- Funhouse_Tounge
- Funhouse_UpsideDown
- Funhouse_Vortex
- Funhouse_Whackamole

### SP_JunkYard.dat

Count: 1

- AMB_JunkYard_AREA

### SP_Library.dat

Count: 3

- Library_Inner
- Library_Outer
- Library_Tunnels

### SP_MainMap.dat

Count: 3

- School_Turret
- School_TurretTripod
- WM_GoKartCreate

### SP_Midway.dat

Count: 1

- Midway_ShootGallery

### SP_Observatory.dat

Count: 1

- Observatory_Amb

### SP_Pool.dat

Count: 7

- BarberShop
- GymPoolHall
- Gym_BoysChange
- Gym_GirlsChange
- Gym_Main
- Gym_Pool01
- Gym_Pool02

### SP_Poor_Cloth.dat

Count: 2

- PoorClothing_Change
- PoorClothing_Main

### SP_Poor_Hair.dat

Count: 2

- HairPoorRm01
- HairPoorRm02

### SP_Prep_House.dat

Count: 6

- PREPHOUSE_PLANTAREA
- PrepHouse_Atrium
- PrepHouse_Entrance
- PrepHouse_Main2nd
- PrepHouse_MainRoom
- PrephouseExterior

### SP_Principal.dat

Count: 5

- Principle01
- Principle02
- Principle03
- Principle04
- Principle_AMB

### SP_Rich_Cloth.dat

Count: 2

- RichClothing_Change
- RichClothing_Main

### SP_School_Hallways.dat

Count: 11

- JainitorsRoom
- Principle_AMB
- SchoolBoysWash
- SchoolBoysWash2
- SchoolCafeteria
- SchoolGirlsWash
- SchoolGirlsWash2
- SchoolHallRoofStairway
- SchoolHalls01
- SchoolHalls02
- SchoolMainAtrium

### SP_Souvenir.dat

Count: 1

- SouvienrShop

### SP_TGOKart.dat

Count: 1

- GoKartTrack_Amb

### SP_Tenement.dat

Count: 22

- Tenements_Balcony
- Tenements_Bathroom
- Tenements_Hall01
- Tenements_Hall02
- Tenements_Hall03
- Tenements_Hole
- Tenements_Hole02
- Tenements_Rm01
- Tenements_Rm02
- Tenements_Rm03
- Tenements_Rm04
- Tenements_Rm05
- Tenements_Rm06
- Tenements_Rm07
- Tenements_Rm08
- Tenements_Rm09
- Tenements_Rm10
- Tenements_Rm11
- Tenements_Rm12
- Tenements_Rm13
- Tenements_base_stair
- Tenements_basement

### SP_Test_Area.dat

Count: 8

- AudioStPinkBankTest
- AudioStereoBankTest
- AudioStereoStreamTest
- AudioSteroPinkStreamTest
- AudioSurrBankTest
- AudioSurrPinkBankTest
- AudioSurrPinkStreamTest
- AudioSurrndStreamTest

### SP_WareHouse.dat

Count: 1

- WareHouse_Amb01

### SP_iGrsrS.dat

Count: 2

- GreaserBathroom
- GreaserMainRoom

### SP_iJockS.dat

Count: 1

- JockHideOut

### SP_iNerdS.dat

Count: 3

- NerdComputerRoom
- NerdMainRoom
- NerdStairwell

### SaveLocs.dat

Count: 5

- SaveBookDropouts
- SaveBookGreasers
- SaveBookJocks
- SaveBookNerds
- SaveBookPreps

### School_Exterior.dat

Count: 1

- EVENING_MUSIC_TRIGGER

### SecTrig.dat

Count: 1

- PTrig

### SndBnkLoad.dat

Count: 5

- BUS_SODA_01
- POORAREA_SODA_01
- RICH_SODA_01
- SCHOOLPROP_SODA_01
- SCHOOLPROP_SODA_02

### SodaNerd.dat

Count: 1

- 1_04_Soda_Nerd

### SoundBankTriggers.dat

Count: 18

- SND_BEACH
- SND_BUSINESS_AREA
- SND_CARNIVAL_AREA
- SND_CarnTunnelBank
- SND_DAM
- SND_DOCKYARD
- SND_INDUSTRIAL_AREA
- SND_POOR_AREA
- SND_RICHPARKSPRINKLERS
- SND_RICH_AREA
- SND_Roundhouse
- SND_SCHOOLPOND
- SND_SCHOOLTUNNEL01
- SND_SCHOOLTUNNEL02
- SND_SCHOOLTUNNEL03
- SND_SCHOOL_AREA
- SND_SCHOOL_ROOF
- SND_WATER

### SoundTriggers.dat

Count: 32

- AMB_BUSINESS_AREA
- AMB_Beach02_ISLAND
- AMB_CARNIVAL_AREA
- AMB_ForestBeachTunnel
- AMB_HOBOAREA
- AMB_INDUSTRIAL_AREA
- AMB_Openwater
- AMB_POOR_AREA
- AMB_RICH_AREA
- AMB_RIVER
- AMB_RIVER03
- AMB_RIVER04
- AMB_RIVERDAM
- AMB_RIVER_DOCK
- AMB_SCHOOL_AREA
- AMB_SmallBeachForest
- Amb_Carnival_Tunnel
- Amb_ForestTrainTunnels
- Amb_ForestTunnels
- Amb_RichAreaCliff
- Amb_SchoolRoofTop
- Amb_TownHallRoofTop
- Asylum
- BEACH_AREA_P
- Carn_Tunnel_Reverb
- Cemetary
- Chemical_Plant_Roof
- Forest
- Ind_SpazMeats
- PoorTrainTunnel
- Powerplant_Sequrity
- TrainYard

### SpawnTest.dat

Count: 20

- Boxtest
- DT_SpawnTest3
- LockerTest
- STEALTH_PORTAPOTTY
- ST_CRATE_01
- ST_CRATE_02
- ST_CRATE_03
- ST_DOOR
- SmallCrate1
- SmallCrate10
- SmallCrate11
- SmallCrate2
- SmallCrate3
- SmallCrate5
- SmallCrate6
- SmallCrate7
- SmallCrate9
- SpawnTest_Door1
- SpawnTest_Door2
- SpawnTest_Trig1

### Store.dat

Count: 14

- ComicBedExclude
- ComicPopTrig
- DT_CarnCurt02
- DT_ibkshop_Door
- DT_icomshp_Basement
- DT_icomshp_Door
- DT_igrocery_Door
- FMDoor01N
- FMDoorN
- FMDoorN01
- Store_DT_BikeArea
- Store_DT_ComicArea
- Store_DT_GeneralArea
- icomshp_Basement

### TFight01.dat

Count: 8

- Spud_Cannon_Bottom
- Spud_Cannon_Top
- TFIGHT01_Barricade
- TFIGHT01_Cannon_Nerd
- TFIGHT01_Door1
- TFIGHT01_Door2
- TFIGHT01_Door3
- TFIGHT01_Door4

### TFight02.dat

Count: 2

- TF02_Fight1
- TF02_Fight2

### TenErrands.dat

Count: 10

- TEN_FIRE01
- TEN_FIRE02
- TEN_FIRE03
- TEN_FIRE04
- TEN_FIRE05
- TEN_FIRE06
- TEN_FIRE07
- TEN_FIRE08
- TEN_FIRE09
- TEN_FIRE10

### TestBaseballToss.dat

Count: 23

- BatterEight
- BatterFive
- BatterFour
- BatterNine
- BatterOne
- BatterSeven
- BatterSix
- BatterThree
- BatterTwo
- CatcherFive
- CatcherFour
- CatcherOne
- CatcherSeven
- CatcherSix
- CatcherThree
- CatcherTwo
- UmpireFive
- UmpireFour
- UmpireOne
- UmpireSeven
- UmpireSix
- UmpireThree
- UmpireTwo

### TestBikeObjectives.dat

Count: 1

- TestBikeGraffiti

### TestMailboxTarget.dat

Count: 1

- TestMailboxTarget

### TestProjDetection.dat

Count: 1

- TestProjDetectionWall

### TestTriggerEvent.dat

Count: 1

- TestTriggerEvent

### Test_4_02.dat

Count: 33

- 4_02_Algie_Final_Stand
- 4_02_Algie_Left_Lib
- 4_02_Bar_01
- 4_02_Bar_02
- 4_02_Bar_03
- 4_02_Breaker_Box
- 4_02_Delete_Wave1
- 4_02_Delete_Wave3
- 4_02_Eavesdrop
- 4_02_Finale
- 4_02_NERDS
- 4_02_Nerd_Ambush1
- 4_02_Nerd_Ambush2
- 4_02_Nerd_Deleter
- 4_02_O_R1_1T
- 4_02_O_R2_1T
- 4_02_O_WN1_1T
- 4_02_O_WN2_1T
- 4_02_O_WN3_1T
- 4_02_O_WN4_1T
- 4_02_O_W_F_1T
- 4_02_PREFECT1
- 4_02_PREFECT2
- 4_02_P_Wave2
- 4_02_P_Wave3
- 4_02_P_Wave4
- 4_02_Player_On_CannonT
- 4_02_Player_Out_Of_Lib
- 4_02_Spotted_Scout
- 4_02_Spud_Cannon
- 4_02_Spud_Tripod
- 4_02_TEMP_Cannon_Line2
- 4_02_WATER

### eventsAsylum.dat

Count: 1

- AsylumPatrols

### eventsAuditorium.dat

Count: 2

- DT_auditorium_doorL
- auditorium_doorR

### eventsAutoShop.dat

Count: 1

- DT_autoshop_doorL

### eventsBDorm.dat

Count: 6

- DormChemistrySet
- DormDoorTrig1
- DormDoorTrig2
- DormDoorTrig3
- DormDoorTrig4
- DormTVTrig

### eventsBoxing.dat

Count: 2

- BoxingTurfTrigger
- Boxing_Tether

### eventsCafeteria.dat

Count: 1

- LunchLadyTrigger

### eventsClassroom.dat

Count: 1

- DT_classr_doorL

### eventsGymAndPool.dat

Count: 7

- DT_gym_doorL
- DT_pool_doorL
- INPOOLAREA
- gyml_doorR
- pool_boyslocker
- pool_doorR
- pool_girlslocker

### eventsObservatory.dat

Count: 2

- DT_observatory_doorL
- observatory_doorR

### eventsPoorHair.dat

Count: 1

- DT_phair_doorL

### eventsSchoolHalls.dat

Count: 8

- BoysBathroom1
- BoysBathroom2
- CafTrigger
- GirlsBathroom1
- GirlsBathroom2
- HallsPopTrigger
- SAVEBOOKSCHOOL
- SchoolStoreExc

### eventsStaffRoom.dat

Count: 1

- DT_staff_doorL

### funhouse.dat

Count: 18

- FUNHOUSE_CURTAIN_OPEN
- FUNHOUSE_GRAVECONTROL
- FUNHOUSE_GRAVES
- FUNHOUSE_GRAVEYARD
- FUNHOUSE_GRAVE_TO_MAZE_TRANS
- FUNHOUSE_MAZE
- FUNHOUSE_MAZE_TO_GRAVE_TRANS
- FUNHOUSE_MINE
- FUNHOUSE_MINE_ROCKS
- FUNHOUSE_MINE_STEAM_01
- FUNHOUSE_MINE_STEAM_02
- FUNHOUSE_MINE_STEAM_03
- FUNHOUSE_PILLOW_ROOM
- FUNHOUSE_P_TO_G_TRANS
- FUNHOUSE_SCAFFOLD
- FUNHOUSE_UPSIDEDOWN_ROOM
- FUNHOUSE_U_TO_G_TRANS
- FUNHOUSE_VORTEX_ENTRANCE

### gym_pool.dat

Count: 1

- gym_pool

### iChemPlant.dat

Count: 3

- 5_B_CHEM_DOOR
- 5_B_CHEM_DOOR_2
- DT_ChemPlant_DoorL

### iSaveZones.dat

Count: 19

- BdrDoorL
- BdrDoorL01
- BdrDoorL01
- BdrDoorL02
- BdrDoorL02
- DRPDoor
- DRPDoor01
- DT_iSafeDrop_DoorL
- DT_iSafeGrsr_DoorL
- DT_iSafeJock_DoorL
- DT_iSafeNerd_DoorL
- DT_iSafePrep_DoorL
- ESCDoorL
- ESCDoorL04
- ESCDoorL05
- ESCDoorL06
- ESCDoorR
- FMDoor
- FMDoor01

### iasylum.dat

Count: 30

- AsyDoorB
- AsyDoors
- AsyDoors10
- AsyDoors11
- AsyDoors12
- AsyDoors13
- AsyDoors14
- AsyDoors15
- CellDoor
- CellDoor12
- CellDoor13
- CellDoor14
- CellDoor15
- CellDoor16
- CellDoor17
- CellDoor18
- CellDoor19
- CellDoor20
- CellDoor21
- DT_ASYLUM_BACK_EXIT
- DT_ASYLUM_EXITL
- ESCDoorR
- FMDoor
- FMDoor02
- FMDoor03
- FMDoor04
- FMDoor05
- FMDoor06
- FMDoor07
- FMDoor08

### iballtos.dat

Count: 3

- BBatter
- BCatcher
- BUmpire

### ibarber.dat

Count: 5

- DT_barber_exit
- DT_salon_exit
- Store_BarberPoor_Area
- Store_Barber_Area
- Store_HairSalon_Area

### iboxing.dat

Count: 14

- DT_iboxing_DoorL
- IBOXING_SWEATER_TRIG
- iboxing_BoxRopes
- iboxing_BoxRopes01
- iboxing_BoxRopes02
- iboxing_BoxRopes03
- iboxing_ESCDoorL
- iboxing_ESCDoorL01
- iboxing_ESCDoorR
- iboxing_ESCDoorR01
- iboxing_IntDoor02
- iboxing_barvault01
- iboxing_barvault02
- iboxing_fakeCoronaTrigger

### iboxing_punchingbags.dat

Count: 3

- BXPBag
- BXPBag01
- BXPBag02

### icloth_p.dat

Count: 2

- DT_iclothp_doorL
- icloth_p_trigger

### icloth_r.dat

Count: 2

- DT_iclothr_DoorL
- RCLTH_Trigger

### ifunhous.dat

Count: 53

- DT_FunhouseTheaterCarnival
- DT_ifunhous_FMDoor
- DT_ifunhous_FMDoorA
- funCurtn
- funCurtn01
- fun_MazeEntryDoor
- ifunhous_CtrlRoom
- ifunhous_CtrlRoomCtrl
- ifunhous_EndMine
- ifunhous_FLbBook
- ifunhous_FLbLader
- ifunhous_FMTrapDr00L
- ifunhous_FMTrapDr00O
- ifunhous_FMTrapDr01L
- ifunhous_FMTrapDr01O
- ifunhous_FMTrapDr02L
- ifunhous_FMTrapDr02O
- ifunhous_FMTrapDr03L
- ifunhous_FMTrapDr03O
- ifunhous_FMTrapSw
- ifunhous_FMTrapSw01
- ifunhous_FMTrapSw01b
- ifunhous_FMTrapSw02
- ifunhous_FMTrapSw02b
- ifunhous_FMTrapSw03
- ifunhous_FMTrapSw03b
- ifunhous_FMTrapSw04
- ifunhous_FMTrapSw04b
- ifunhous_FMTrapSw05
- ifunhous_FMTrapSw05b
- ifunhous_FMTrapSw06
- ifunhous_FMTrapSw06b
- ifunhous_FMTrapSw07
- ifunhous_FMTrapSw07b
- ifunhous_FMTrapSwb
- ifunhous_MineEnd
- ifunhous_MineMze
- ifunhous_MzeMine
- ifunhous_Reeper00
- ifunhous_Reeper00b
- ifunhous_Reeper01
- ifunhous_Reeper01b
- ifunhous_Reeper02
- ifunhous_Reeper02b
- ifunhous_funMinerB
- ifunhous_funMinerD
- ifunhous_funMinerG
- ifunhous_funMinerH
- ifunhous_funMinerI
- ifunhous_funMinerX1
- ifunhous_funMinerX2
- ifunhous_funMinerX3
- ifunhous_funMinerX4

### isc_lib.dat

Count: 3

- DT_LibraryExitR
- ESCDoorL
- isclib_Globe

### isc_offi.dat

Count: 1

- BdrDoorL

### isc_pool.dat

Count: 9

- GymPool_PopOverride
- LckrGymA01
- LckrGymA02
- LckrGymA03
- LckrGymB
- LckrGymB01
- LckrGymB02
- LckrGymB03
- LckrGymM

### ischool_doors.dat

Count: 36

- DT_ISCHOOL_BIO
- DT_ISCHOOL_CHEM
- DT_ischool_Art
- DT_ischool_AuditorBalc
- DT_ischool_AuditorDoorL
- DT_ischool_BackDoorLeft
- DT_ischool_BackDoorRight
- DT_ischool_Classroom
- DT_ischool_Door01
- DT_ischool_FrontDoorL
- DT_ischool_FrontDoorRight
- DT_ischool_HallWind
- DT_ischool_Janitor
- DT_ischool_RoofDoor
- DT_ischool_Staff
- JanDoor02
- RAIL_HALLWAY01
- RAIL_HALLWAY02
- RAIL_HALLWAY03
- RAIL_HALLWAY04
- ischool_CafDoor2R
- ischool_Door00
- ischool_Door02
- ischool_Door05
- ischool_Door06
- ischool_Door09
- ischool_Door19
- ischool_Door21
- ischool_Door23
- ischool_Door24
- ischool_Door25
- ischool_Door28
- ischool_Door30
- ischool_FrontDoorR
- ischool_StoreArea
- ischool_StoreDoor

### ischool_fountains.dat

Count: 9

- ischool_fountains_SCFount
- ischool_fountains_SCFount03
- ischool_fountains_SCFount04
- ischool_fountains_SCFount05
- ischool_fountains_SCFount06
- ischool_fountains_SCFount09
- ischool_fountains_SCFount12
- ischool_fountains_SCFount15
- ischool_fountains_SCFount16

### ischool_lockers.dat

Count: 25

- NLock01A
- NLock01A01
- NLock01A02
- NLock01B
- NLock01B01
- NLock01B02
- NLock01B04
- NLock01B05
- NLock01B06
- NLock01B07
- NLock02A
- NLock02A01
- NLock02A02
- NLock02A03
- NLock02B
- NLock02B01
- NLock02B02
- NLock02B03
- NLock02B04
- NLock02B05
- NLock02B06
- NLock02B07
- NLock02B08
- NLock02B09
- NLock02B10

### iwarehouse.dat

Count: 2

- DT_whouse_front
- DT_whouse_roof

### mlee_pickups.dat

Count: 1

- crate01

### mm_retirement.dat

Count: 6

- CHTrespass
- GasStop1
- GasStop2
- LawnMowerTrigger
- MailmanTrigger
- RichFolkTrigger

### stopsigns.dat

Count: 32

- \_SSI_00
- \_SSI_01
- \_SSI_02
- \_SSI_03
- \_SSI_04
- \_SSI_05
- \_SSI_06
- \_SSI_07
- \_SSI_08
- \_SSI_09
- \_SSI_10
- \_SSI_11
- \_SSI_12
- \_SSI_13
- \_SSI_14
- \_SSI_15
- \_SSI_16
- \_SSI_17
- \_SSI_18
- \_SSI_19
- \_SSI_20
- \_SSI_21
- \_SSI_22
- \_SSI_23
- \_SSI_24
- \_SSI_25
- \_SSI_26
- \_SSI_27
- \_SSI_28
- \_SSI_29
- \_SSI_30
- \_SSI_31

### tBMX.dat

Count: 3

- BMX_GarageDoor
- DT_BMXGarageDoor
- DT_tBMX_leave

### tags.dat

Count: 106

- DT_Medium_001
- DT_Medium_002
- DT_Medium_003
- DT_Medium_004
- DT_Medium_005
- DT_Medium_006
- DT_Medium_007
- DT_Medium_008
- DT_Medium_009
- DT_Medium_010
- DT_Medium_011
- DT_Medium_012
- DT_Medium_013
- DT_Medium_014
- DT_Medium_015
- DT_Medium_016
- DT_Medium_017
- DT_Medium_019
- DT_Medium_020
- DT_Medium_021
- DT_Medium_022
- DT_Medium_023
- DT_Medium_024
- DT_Medium_025
- IA_medium01
- IA_medium02
- IA_medium03
- IA_medium04
- IA_medium05
- IA_medium06
- IA_medium07
- PoorArea_Medium_001
- PoorArea_Medium_002
- PoorArea_Medium_004
- PoorArea_Medium_005
- PoorArea_Medium_006
- PoorArea_Medium_007
- PoorArea_Medium_008
- PoorArea_Medium_009
- PoorArea_Medium_010
- PoorArea_Medium_013
- PoorArea_Medium_014
- PoorArea_Medium_015
- PoorArea_Medium_016
- PoorArea_Medium_017
- PoorArea_Medium_018
- PoorArea_Medium_019
- PoorArea_Medium_020
- PoorArea_Medium_021
- PoorArea_Medium_022
- PoorArea_Medium_023
- PoorArea_Medium_024
- PoorArea_Medium_025
- PoorArea_Medium_026
- PoorArea_Medium_027
- PoorArea_Medium_028
- PoorArea_Medium_029
- PoorArea_Medium_030
- RA_Medium01
- RA_Medium02
- RA_Medium03
- RA_Medium04
- RA_Medium05
- RA_Medium06
- RA_Medium07
- RA_Medium08
- RA_Medium10
- RA_Medium11
- RA_Medium12
- RA_Medium13
- RA_Medium14
- RA_Medium15
- RA_Medium16
- RA_Medium17
- RA_Medium18
- RA_Medium19
- RA_Medium20
- RA_Medium21
- RA_Medium22
- RA_Medium23
- RA_Medium24
- RA_medium09
- SG_Medium01
- SG_Medium02
- SG_Medium03
- SG_Medium04
- SG_Medium05
- SG_Medium06
- SG_Medium07
- SG_Medium08
- SG_Medium09
- SG_Medium10
- SG_Medium11
- SG_Medium12
- SG_Medium14
- SG_Medium15
- SG_Medium16
- SG_Medium17
- SG_Medium18
- SG_Medium19
- SG_Medium20
- SO_Medium01
- SO_Medium02
- SO_Medium03
- SO_Medium04
- SO_Medium05

### tags_dorm.dat

Count: 2

- BD_Medium1
- BD_Medium2

### tags_hallways.dat

Count: 8

- SH_Medium01
- SH_Medium02
- SH_Medium03
- SH_Medium04
- SH_Medium05
- SH_Medium07
- SH_Medium08
- SH_Medium09

### tbarrels.dat

Count: 1

- tbarrels_Sbarels1

### tbusines.dat

Count: 2

- tbusiness_GarbCanA08
- tbusiness_MotelDor

### tbusines_BMXGate.dat

Count: 1

- tbusiness_BMXGate

### tbusines_doors.dat

Count: 46

- BA_BMXGarage
- BA_DoorStr01
- BA_DoorStr02
- BA_DoorStr03
- BA_DoorStr04
- BA_DoorStr05
- BA_DoorStr07
- BA_DoorStr08
- BA_PrepDoor02
- BA_PrepDoor03
- BA_PrepDoor04
- BA_PrepDoor05
- BA_PrepDoor06
- BA_PrepDoor09
- BA_PrepDoor10
- BA_PrepDoor11
- DT_BMXGarage
- DT_tbusines_BikeShopDoor
- DT_tbusines_ClothDoor
- DT_tbusines_ComicShopDoor
- DT_tbusines_FirewShopDoor
- DT_tbusines_GenShop1Door
- DT_tbusines_GenShop2Door
- DT_tbusines_SafeNerd
- DT_tbusiness_FirewBusDoor
- DT_tbusiness_Recorddoor
- DT_tbusiness_barber
- DT_tpoor_BMX
- DT_tpoor_Barber
- DT_tpoor_SafeGreaser
- DT_tpoor_tenwindow
- bu_DoorStr10
- bu_PrepDoor13
- bu_PrepDoor14
- bu_PrepDoor15
- bu_PrepDoor16
- bu_PrepDoor17
- bu_PrepDoor18
- bu_PrepDoor19
- bu_PrepDoor20
- bu_PrepDoor21
- bu_PrepDoor22
- bu_PrepDoor23
- bu_PrepDoor24
- bu_PrepDoor25
- hardwareback

### tcarni.dat

Count: 11

- Coaster
- DT_CarnCurt01
- DT_FreakEntrance
- DT_FreakExit
- Ferris
- FunTeeth
- Squid
- carnGate01
- carnGate02
- carnGate03
- carnGate04

### tenements.dat

Count: 2

- DT_Tenement_Window
- TENEMENTS_FIRE_ESCAPE_CAMERA

### testMandyRatFlee.dat

Count: 1

- tmrf_ratBoundary

### testSafeCut.dat

Count: 1

- testSafeCut_startCut

### tindustrial.dat

Count: 1

- TINDUST_ASYLUM

### tindustrial_doors.dat

Count: 9

- DT_indoor_TattooShop
- DT_indoor_whouseFront
- DT_indoor_whouseRoof
- DT_tBMX_enter
- DT_tind_SafeDrop
- Ind_DoorStr02
- Ind_DoorStr1
- Ind_MedicalDoor
- Ind_PoliceDoor

### tphoto.dat

Count: 1

- TPHOTO_FIRE

### tphotoglass.dat

Count: 1

- TPHOTO_FIREG

### trich.dat

Count: 14

- ESCDoorL05
- ESCDoorR05
- FortuneTeller
- Hattrick_gate
- PETEYPIER
- RAIL_RICH01
- RAIL_RICH02
- RAIL_RICH03
- RAIL_RICH04
- RAIL_RICH05
- RAIL_RICH06
- TadGates02
- trich_TadGates
- trich_TadGates01

### trich_doors.dat

Count: 52

- ChezLouis
- DT_trich_BarberDoor
- DT_trich_BikeShopDoor
- DT_trich_BoxingDoor01
- DT_trich_BoxingDoor02
- DT_trich_ClothRichDoor
- DT_trich_FirewShopDoor
- DT_trich_GenShopDoor
- DT_trich_SafePrep
- HattrickDoor
- RA_DoorStr02
- RA_DoorStr05
- RA_DoorStr06
- RA_DoorStr07
- RA_DoorStr08
- RA_DoorStr09
- RA_PrepDoor02
- RA_PrepDoor03
- RA_PrepDoor04
- RA_PrepDoor05
- RA_PrepDoor06
- RA_PrepDoor07
- RA_PrepDoor08
- RA_PrepDoor09
- RA_PrepDoor10
- RA_PrepDoor11
- RA_PrepDoor12
- RA_PrepDoor13
- RA_PrepDoor14
- RA_PrepDoor15
- RG_FW_enter_m
- RG_FW_enter_s
- RG_FW_exit_m
- RG_FW_exit_s
- RG_RC_enter_m
- RG_RC_enter_s
- RG_RC_exit_m
- RG_RC_exit_s
- RG_SQ_enter_m
- RG_SQ_exit_m
- TadBackDoorL
- TadBackDoorR
- TadFrontDoorL
- TadFrontDoorR
- TadShud
- TadShud01
- TadShud02
- TadShud03
- TadShud04
- TadShud05
- icecream
- valeHotelDoor

### tschool_doors.dat

Count: 25

- DT_tschool_AutoShopL
- DT_tschool_BoysDormL
- DT_tschool_ExtWind
- DT_tschool_GirlsDormL
- DT_tschool_GirlsDormSideL
- DT_tschool_GymL
- DT_tschool_LibraryL
- DT_tschool_PoolL
- DT_tschool_PreppyL
- DT_tschool_RoofDoor
- DT_tschool_SafeJock
- DT_tschool_SchoolFrontDoorL
- DT_tschool_SchoolLeftBackDoor
- DT_tschool_SchoolRightBackDoor
- DT_tschool_SchoolRightFrontDoor
- DT_tschool_SchoolSideDoorL
- tschool_BoysDormR
- tschool_FieldR
- tschool_GirlsDormR
- tschool_GymR
- tschool_LibraryR
- tschool_PoolR
- tschool_PreppyR
- tschool_SchoolFrontDoorR
- tschool_SchoolLeftFrontDoor

### tschool_garagedoors.dat

Count: 3

- SCgrdoor
- SCgrdoor01
- SCgrdoor02

### tschool_maindoors.dat

Count: 8

- BusDoors
- EggBDorm
- EggGDorm
- RAIL_SCHOOL01
- RAIL_SCHOOL02
- ScGate_Observatory
- boysDormCourtyard
- girlsDormCourtyard

### ttest.dat

Count: 42

- Armor
- BBChair
- BMXGate
- BNews
- BSign
- BTable
- BalanceBeam
- BenchA
- BenchB
- BenchC
- BottleB
- BottleC
- BottleD
- BottleE
- BoxRopes
- CrateBrk
- Dumpster
- GarbCanA
- GasSign
- GnomeB
- GnomeD
- Incin
- LifeGrd
- NLock01A
- NLock03B
- Picnic
- PokerTbl
- PortaPoo
- RMailbox
- SCFount
- SCLock01
- SCLock02
- SCLock03
- SC_Crest
- SGTargBTrig
- SandCasl
- Snowman
- Stable
- TennFrid
- TennWash
- gnomeA
- pChair
