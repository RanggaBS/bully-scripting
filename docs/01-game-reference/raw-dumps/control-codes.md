---
description: Control codes are special sequences embedded within game text that act as inline instructions for the engine.
---

# Control Codes

Control codes are special sequences embedded within game text that act as inline instructions for the engine. They are usually wrapped in delimiters (in this case tildes `~`) and direct the game to perform actions such as inserting a line break, showing an icon, or triggering a contextual button display. Rather than being visible to the player as raw text, these codes control how the text is formatted and how certain UI elements are rendered during gameplay.

This page documents the results of analyzing the **decompiled XML localization files** from _Bully: Anniversary Edition_ (mobile). The analysis was performed using a community-made tool ([EdnessP](https://github.com/EdnessP)) that extracts the XML data. Note that this applies specifically to the AE version; the _Scholarship Edition_ (PC) uses a different localization system (`Config/Text/{American,British,French,...}.{dir,img}` plus `.bin` files inside the `.img`). While many control codes are likely shared, differences in frequency and content may exist due to AE’s additional features.

## Global Summary

This section provides the total frequency of each control code across all analyzed XML files.

|    # | Control Code                | Total Count |
| ---: | --------------------------- | ----------: |
|   1. | `~$~`                       |         120 |
|   2. | `~1~`                       |          16 |
|   3. | `~4_05_bull_piss~`          |          14 |
|   4. | `~ACCELERATE~`              |         103 |
|   5. | `~ACTION~`                  |        1344 |
|   6. | `~ATTACK~`                  |         119 |
|   7. | `~ATTACK_L~`                |          34 |
|   8. | `~ATTACK_R~`                |         165 |
|   9. | `~B~`                       |          32 |
|  10. | `~BIKE_ATTACK_L~`           |           8 |
|  11. | `~BIKE_ATTACK_R~`           |           8 |
|  12. | `~BIKE_TRICK~`              |           8 |
|  13. | `~BRAKE~`                   |          87 |
|  14. | `~BULLY_CREST~`             |           8 |
|  15. | `~CANCEL~`                  |         540 |
|  16. | `~CLASS_CONTINUE~`          |          17 |
|  17. | `~CLASS_DELETE~`            |          26 |
|  18. | `~CLASS_EXIT~`              |         189 |
|  19. | `~CLASS_INFO~`              |         211 |
|  20. | `~CLASS_RETRY~`             |          17 |
|  21. | `~CLASS_SABOTAGE_ICON~`     |          16 |
|  22. | `~CLASS_SCRAMBLE~`          |          16 |
|  23. | `~CLASS_SELECT~`            |         641 |
|  24. | `~CLASS_START~`             |          17 |
|  25. | `~CONFIRM~`                 |         485 |
|  26. | `~COW_DANCE_END~`           |           8 |
|  27. | `~COW_DANCE_START~`         |           8 |
|  28. | `~CROUCH~`                  |          56 |
|  29. | `~DECREASE_BET~`            |          31 |
|  30. | `~DGB_CATCH~`               |          16 |
|  31. | `~DGB_DODGE~`               |           8 |
|  32. | `~DGB_JUMP~`                |           8 |
|  33. | `~DGB_PASS~`                |          16 |
|  34. | `~DGB_SWITCH~`              |           8 |
|  35. | `~DGB_THROW~`               |          16 |
|  36. | `~DISMOUNT~`                |           8 |
|  37. | `~Drücke ~`                 |           1 |
|  38. | `~FIRE_WEAPON~`             |         304 |
|  39. | `~GIVE_ITEM1~`              |           8 |
|  40. | `~GIVE_ITEM2~`              |           8 |
|  41. | `~GRAPPLE~`                 |          40 |
|  42. | `~GRAPPLE_TAKEDOWN~`        |           8 |
|  43. | `~HAND_BRAKE~`              |          15 |
|  44. | `~HAND_BREAK~`              |           1 |
|  45. | `~HELP~`                    |           8 |
|  46. | `~HORN~`                    |           8 |
|  47. | `~HUMILIATE~`               |          41 |
|  48. | `~INCREASE_BET~`            |          31 |
|  49. | `~JUMP~`                    |          48 |
|  50. | `~LOAD~`                    |           8 |
|  51. | `~LOOK_BACK~`               |          32 |
|  52. | `~MANUAL_LOCK~`             |         368 |
|  53. | `~MG_THROW_BALL~`           |          25 |
|  54. | `~OLLIE~`                   |           8 |
|  55. | `~PHOTO_RETRY~`             |           8 |
|  56. | `~P_ZOOM_IN~`               |          56 |
|  57. | `~P_ZOOM_OUT~`              |          65 |
|  58. | `~R1~`                      |          17 |
|  59. | `~R2~`                      |         390 |
|  60. | `~REVERSAL_FOUR~`           |           8 |
|  61. | `~REVERSAL_ONE~`            |           8 |
|  62. | `~REVERSAL_THREE~`          |           8 |
|  63. | `~REVERSAL_TWO~`            |           8 |
|  64. | `~RUN~`                     |          80 |
|  65. | `~SAVE~`                    |           8 |
|  66. | `~SAVE_RETRY~`              |          16 |
|  67. | `~SCROLL_WEAPL~`            |         112 |
|  68. | `~SCROLL_WEAPR~`            |         120 |
|  69. | `~SHOVEL~`                  |          15 |
|  70. | `~SHOW_OPTIONS~`            |          63 |
|  71. | `~SHOW_PRIM_OBJ~`           |          38 |
|  72. | `~SHOW_SEC_OBJ~`            |           8 |
|  73. | `~SOCCER_KEEPUP1~`          |           8 |
|  74. | `~SOCCER_KEEPUP2~`          |           8 |
|  75. | `~SOCCER_KEEPUP3~`          |           8 |
|  76. | `~SOCCER_KEEPUP4~`          |           8 |
|  77. | `~TAG_COMBO1~`              |         184 |
|  78. | `~TAG_COMBO2~`              |         216 |
|  79. | `~TAG_COMBO3~`              |         120 |
|  80. | `~TAG_COMBO4~`              |         112 |
|  81. | `~TAG_START~`               |         104 |
|  82. | `~TAKE_PHOTO~`              |          23 |
|  83. | `~THUMBS_DOWN~`             |          56 |
|  84. | `~THUMBS_UP~`               |         136 |
|  85. | `~TREE_TURN_AROUND~`        |           8 |
|  86. | `~WEAPON_FIRE~`             |          16 |
|  87. | `~WII_B~`                   |           8 |
|  88. | `~WII_RPAD~`                |           8 |
|  89. | `~a~`                       |         420 |
|  90. | `~ambient~`                 |          40 |
|  91. | `~bike~`                    |          32 |
|  92. | `~blipdown~`                |          16 |
|  93. | `~blipup~`                  |          16 |
|  94. | `~bullet~`                  |         602 |
|  95. | `~bus~`                     |          16 |
|  96. | `~button_chem_cylinder~`    |           8 |
|  97. | `~cent~`                    |           7 |
|  98. | `~class~`                   |          24 |
|  99. | `~clothing~`                |           8 |
| 100. | `~copyr~`                   |          16 |
| 101. | `~ddown~`                   |         223 |
| 102. | `~dleft~`                   |         275 |
| 103. | `~dright~`                  |         275 |
| 104. | `~dup~`                     |         223 |
| 105. | `~enemy~`                   |           8 |
| 106. | `~f~`                       |          77 |
| 107. | `~g~`                       |          69 |
| 108. | `~genstore~`                |           8 |
| 109. | `~h~`                       |          40 |
| 110. | `~hud_accelerate~`          |          35 |
| 111. | `~hud_back~`                |          14 |
| 112. | `~hud_bicycle~`             |           8 |
| 113. | `~hud_block~`               |           7 |
| 114. | `~hud_brake~`               |          28 |
| 115. | `~hud_button_b~`            |          14 |
| 116. | `~hud_button_l1~`           |           7 |
| 117. | `~hud_button_r1~`           |           7 |
| 118. | `~hud_button_x~`            |         147 |
| 119. | `~hud_button_y~`            |          14 |
| 120. | `~hud_buy~`                 |          16 |
| 121. | `~hud_camera~`              |          23 |
| 122. | `~hud_check~`               |         278 |
| 123. | `~hud_climb~`               |          16 |
| 124. | `~hud_clothes~`             |           8 |
| 125. | `~hud_crouch~`              |          22 |
| 126. | `~hud_drop_jetpack~`        |          24 |
| 127. | `~hud_ebrake~`              |          14 |
| 128. | `~hud_grab~`                |          37 |
| 129. | `~hud_horn~`                |           7 |
| 130. | `~hud_info~`                |           8 |
| 131. | `~hud_jump~`                |          34 |
| 132. | `~hud_left~`                |           8 |
| 133. | `~hud_melee~`               |           7 |
| 134. | `~hud_minus~`               |          14 |
| 135. | `~hud_plus~`                |          14 |
| 136. | `~hud_prank~`               |          14 |
| 137. | `~hud_punch~`               |         168 |
| 138. | `~hud_right~`               |           8 |
| 139. | `~hud_save~`                |          23 |
| 140. | `~hud_sleep~`               |           8 |
| 141. | `~hud_spraycan~`            |           7 |
| 142. | `~hud_takedown~`            |          14 |
| 143. | `~hud_target~`              |          92 |
| 144. | `~hud_throw~`               |          49 |
| 145. | `~hud_turn_left~`           |           6 |
| 146. | `~hud_up~`                  |           7 |
| 147. | `~hud_x~`                   |          14 |
| 148. | `~hud_yes~`                 |          42 |
| 149. | `~hudelems_social_errands~` |          23 |
| 150. | `~i~`                       |        1976 |
| 151. | `~infinity~`                |           8 |
| 152. | `~job~`                     |          24 |
| 153. | `~left~`                    |          56 |
| 154. | `~leftyrighty~`             |         154 |
| 155. | `~logo~`                    |           8 |
| 156. | `~lstick~`                  |         234 |
| 157. | `~mission~`                 |          47 |
| 158. | `~n~`                       |        9172 |
| 159. | `~nbsp~`                    |         167 |
| 160. | `~o~`                       |           9 |
| 161. | `~objective~`               |          56 |
| 162. | `~q~`                       |           8 |
| 163. | `~race~`                    |          16 |
| 164. | `~right~`                   |          56 |
| 165. | `~rightylefty~`             |          56 |
| 166. | `~rstick~`                  |         138 |
| 167. | `~s_flower~`                |          15 |
| 168. | `~s_greet~`                 |          53 |
| 169. | `~s_humil~`                 |          78 |
| 170. | `~s_kiss~`                  |          15 |
| 171. | `~s_pay~`                   |          61 |
| 172. | `~s_shove~`                 |          69 |
| 173. | `~s_sorry~`                 |          68 |
| 174. | `~s_taunt2~`                |          15 |
| 175. | `~save~`                    |          16 |
| 176. | `~special1~`                |          45 |
| 177. | `~special2~`                |          23 |
| 178. | `~special3~`                |          23 |
| 179. | `~start~`                   |           8 |
| 180. | `~tod~`                     |           8 |
| 181. | `~vendetta~`                |          16 |
| 182. | `~w~`                       |         112 |
| 183. | `~x~`                       |          56 |
| 184. | `~y~`                       |          23 |
| 185. | `~z~`                       |         228 |

## Per File Analysis

This section provides a breakdown of control code usage by file.

### 1-02b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 1-02c_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 1-02d_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |

### 1-02e_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 1-03_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 1-06b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 2     |
| `~n~`        | 1     |

### 1-07_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 1-08_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 1-09_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 1-09b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 8     |

### 1-1-1_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 1-1-2_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 1-b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 2     |
| `~n~`        | 2     |

### 1-bb_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 2     |

### 1-bc_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |
| `~nbsp~`     | 1     |

### 1-g1_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 1-s01_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |
| `~nbsp~`     | 1     |

### 1_01.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 1_02.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 17    |
| `~nbsp~`     | 1     |

### 1_02a.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |

### 1_02b.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 22    |

### 1_02c.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 2     |
| `~n~`        | 1     |

### 1_03.xml

| Control Code    | Count |
| --------------- | ----- |
| `~n~`           | 49    |
| `~ACTION~`      | 8     |
| `~MANUAL_LOCK~` | 8     |
| `~FIRE_WEAPON~` | 8     |
| `~CROUCH~`      | 7     |
| `~P_ZOOM_OUT~`  | 7     |
| `~nbsp~`        | 1     |

### 1_04.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 14    |
| `~nbsp~`     | 1     |

### 1_05.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 35    |
| `~nbsp~`     | 1     |

### 1_06_01.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 10    |

### 1_07.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 1_08.xml

| Control Code    | Count |
| --------------- | ----- |
| `~n~`           | 27    |
| `~CROUCH~`      | 14    |
| `~P_ZOOM_OUT~`  | 7     |
| `~MANUAL_LOCK~` | 7     |

### 1_09.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |
| `~nbsp~`     | 4     |

### 1_10.xml

| Control Code   | Count |
| -------------- | ----- |
| `~n~`          | 18    |
| `~CROUCH~`     | 7     |
| `~P_ZOOM_OUT~` | 7     |
| `~nbsp~`       | 1     |

### 1_11.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 12    |

### 1_11x1.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 13    |

### 1_11x2.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 18    |
| `~ACTION~`   | 16    |

### 1_11xp.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 104   |
| `~n~`        | 32    |
| `~mission~`  | 8     |

### 1_b.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 2     |
| `~n~`        | 1     |

### 1_g1.xml

| Control Code | Count |
| ------------ | ----- |
| `~ACTION~`   | 48    |
| `~n~`        | 6     |

### 1_s01.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 19    |

### 2-01_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 2-03_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 2-04_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 1     |

### 2-05_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 9     |

### 2-07_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 2-08_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 2-g2_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |
| `~nbsp~`     | 1     |

### 2-s02_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |
| `~nbsp~`     | 1     |

### 2-s05b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |
| `~nbsp~`     | 1     |

### 2-s05c_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 1     |

### 2-s07_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |
| `~nbsp~`     | 1     |

### 2_01.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 16    |
| `~n~`        | 10    |

### 2_02.xml

| Control Code      | Count |
| ----------------- | ----- |
| `~n~`             | 20    |
| `~BIKE_ATTACK_L~` | 8     |
| `~BIKE_ATTACK_R~` | 8     |

### 2_03.xml

| Control Code | Count |
| ------------ | ----- |
| `~ACTION~`   | 8     |
| `~n~`        | 6     |

### 2_04.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 2_05.xml

| Control Code | Count |
| ------------ | ----- |
| `~ACTION~`   | 8     |
| `~n~`        | 3     |
| `~nbsp~`     | 1     |

### 2_06.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 23    |

### 2_07.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 2_08.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 8     |

### 2_b.xml

| Control Code | Count |
| ------------ | ----- |
| `~ACTION~`   | 8     |
| `~n~`        | 6     |

### 2_g2.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 14    |
| `~genstore~` | 8     |

### 2_r03.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~i~`            | 24    |
| `~MANUAL_LOCK~`  | 8     |
| `~FIRE_WEAPON~`  | 8     |
| `~SCROLL_WEAPL~` | 8     |
| `~SCROLL_WEAPR~` | 8     |
| `~n~`            | 6     |

### 2_s02.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 16    |

### 2_s04.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 18    |
| `~nbsp~`     | 4     |

### 2_s05.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 78    |
| `~i~`        | 16    |
| `~nbsp~`     | 3     |

### 2_s06.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 11    |
| `~nbsp~`     | 1     |

### 2_s07.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 10    |

### 3-01_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |

### 3-01aa_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 3-01ab_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 1     |

### 3-01ba_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |
| `~nbsp~`     | 1     |

### 3-01ca_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 6     |
| `~nbsp~`     | 1     |

### 3-01da_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3-01db_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |
| `~nbsp~`     | 1     |

### 3-01dc_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 1     |

### 3-03_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 3-04_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3-04b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |
| `~nbsp~`     | 1     |

### 3-05_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 3-06_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |
| `~nbsp~`     | 1     |

### 3-0_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 3-b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3-bd_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3-g3_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 3-r05a_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 3-r07_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |

### 3-s03_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 3-s08_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3-s10_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |
| `~nbsp~`     | 1     |

### 3-s11_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 3-s11c_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |
| `~nbsp~`     | 1     |

### 3_01.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 14    |

### 3_01a.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 7     |

### 3_01c.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 8     |
| `~n~`        | 2     |

### 3_01d.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 34    |
| `~i~`        | 24    |

### 3_02.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 8     |

### 3_04.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 12    |

### 3_05.xml

| Control Code | Count |
| ------------ | ----- |
| `~ACTION~`   | 8     |
| `~n~`        | 7     |

### 3_06.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 6     |

### 3_07.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 3_08.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3_09.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 16    |
| `~ACTION~`   | 8     |
| `~n~`        | 1     |

### 3_b.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 8     |
| `~n~`        | 5     |
| `~nbsp~`     | 1     |

### 3_g3.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |

### 3_r05a.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 3_r05b.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 16    |
| `~ACTION~`   | 8     |
| `~n~`        | 3     |

### 3_r07.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3_r08.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 8     |

### 3_r09.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 63    |
| `~nbsp~`     | 1     |

### 3_r09_d.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 3_r09_j.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 1     |
| `~n~`        | 1     |

### 3_r09_n.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 3_s03.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 16    |

### 3_s08.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 16    |
| `~ACTION~`   | 8     |

### 3_s10.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 10    |
| `~i~`        | 8     |

### 3_s11.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 18    |
| `~ACTION~`   | 8     |

### 4-01_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |

### 4-02_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 4-03_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 4-04_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 4-05_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 4-06_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 4-0_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 2     |
| `~n~`        | 1     |

### 4-b1_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 4-g4_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 1     |

### 4-s12_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 4-s12b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~nbsp~`     | 3     |

### 4_01.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 8     |

### 4_02.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 9     |

### 4_03.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 4_03_2d.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 13    |

### 4_04.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 12    |
| `~RUN~`      | 8     |
| `~ACTION~`   | 8     |

### 4_05.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 20    |
| `~ACTION~`   | 8     |
| `~nbsp~`     | 3     |

### 4_06.xml

| Control Code        | Count |
| ------------------- | ----- |
| `~n~`               | 84    |
| `~ACTION~`          | 24    |
| `~MANUAL_LOCK~`     | 8     |
| `~RUN~`             | 8     |
| `~COW_DANCE_START~` | 8     |
| `~COW_DANCE_END~`   | 8     |
| `~nbsp~`            | 2     |

### 4_07.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 4_b1.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 13    |
| `~nbsp~`     | 4     |

### 4_b2.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 4_g4.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 27    |

### 4_g5.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 4_g6.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 4_s12.xml

| Control Code | Count |
| ------------ | ----- |
| `~a~`        | 16    |
| `~n~`        | 8     |

### 5-01_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |
| `~nbsp~`     | 1     |

### 5-02_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 5-02b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 5-03_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 7     |

### 5-04_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 7     |
| `~nbsp~`     | 1     |

### 5-05_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 6     |

### 5-06_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 6     |

### 5-07_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 5-09_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |
| `~nbsp~`     | 1     |

### 5-09b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |
| `~nbsp~`     | 1     |

### 5-0_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 5-b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 5-bc_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |
| `~nbsp~`     | 1     |

### 5-g5_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 5_01.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 10    |
| `~nbsp~`     | 1     |

### 5_02.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 24    |

### 5_03.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 14    |
| `~ACTION~`   | 8     |

### 5_04.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 9     |

### 5_05.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 12    |

### 5_06.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 5_07.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 10    |
| `~nbsp~`     | 1     |

### 5_07a.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 25    |
| `~i~`        | 16    |
| `~nbsp~`     | 1     |

### 5_07b.xml

| Control Code    | Count |
| --------------- | ----- |
| `~n~`           | 16    |
| `~MANUAL_LOCK~` | 7     |
| `~CROUCH~`      | 7     |
| `~P_ZOOM_OUT~`  | 7     |

### 5_07c.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 5     |

### 5_09.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### 5_b.xml

| Control Code    | Count |
| --------------- | ----- |
| `~n~`           | 11    |
| `~MANUAL_LOCK~` | 8     |
| `~CROUCH~`      | 7     |
| `~P_ZOOM_OUT~`  | 7     |

### 5_g5.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 40    |
| `~n~`        | 29    |
| `~nbsp~`     | 1     |

### 6-02b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### 6-0_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 6-b_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 6-bb_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 3     |

### 6-bc_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 6-bd_sub.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 6_01.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### 6_02.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 8     |
| `~ACTION~`   | 8     |

### 6_03.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 18    |
| `~nbsp~`     | 1     |

### 6_b.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 15    |
| `~left~`     | 8     |
| `~lstick~`   | 8     |
| `~right~`    | 8     |

### classart.xml

| Control Code       | Count |
| ------------------ | ----- |
| `~CLASS_EXIT~`     | 24    |
| `~CLASS_INFO~`     | 16    |
| `~CLASS_CONTINUE~` | 8     |
| `~CLASS_RETRY~`    | 8     |
| `~CLASS_START~`    | 8     |
| `~n~`              | 7     |
| `~nbsp~`           | 1     |

### classbiology.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 655   |
| `~CLASS_SELECT~` | 344   |
| `~R2~`           | 320   |
| `~CLASS_EXIT~`   | 16    |
| `~lstick~`       | 16    |
| `~rstick~`       | 16    |
| `~ATTACK_R~`     | 16    |
| `~CLASS_INFO~`   | 16    |
| `~i~`            | 16    |
| `~z~`            | 8     |

### classchem.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 45    |
| `~CLASS_SELECT~` | 8     |
| `~ATTACK_L~`     | 8     |
| `~ATTACK_R~`     | 8     |
| `~CLASS_EXIT~`   | 8     |
| `~CLASS_INFO~`   | 8     |

### classenglish.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 63    |
| `~CLASS_SELECT~` | 24    |
| `~CLASS_DELETE~` | 16    |
| `~i~`            | 16    |
| `~FIRE_WEAPON~`  | 16    |
| `~CLASS_EXIT~`   | 8     |
| `~lstick~`       | 8     |
| `~ACTION~`       | 8     |
| `~z~`            | 8     |
| `~CLASS_INFO~`   | 8     |

### classgeography.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 67    |
| `~CLASS_SELECT~` | 39    |
| `~i~`            | 24    |
| `~R2~`           | 23    |
| `~CLASS_EXIT~`   | 16    |
| `~R1~`           | 8     |
| `~CLASS_INFO~`   | 8     |
| `~z~`            | 8     |

### classmath.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 49    |
| `~i~`            | 16    |
| `~CLASS_SELECT~` | 16    |
| `~CLASS_INFO~`   | 16    |
| `~CLASS_EXIT~`   | 16    |
| `~CONFIRM~`      | 8     |
| `~lstick~`       | 8     |
| `~rstick~`       | 8     |
| `~R2~`           | 8     |
| `~ATTACK_R~`     | 8     |
| `~z~`            | 8     |

### classmusic.xml

| Control Code    | Count |
| --------------- | ----- |
| `~i~`           | 8     |
| `~MANUAL_LOCK~` | 8     |

### classphoto.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 15    |

### classphotography2p.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 84    |
| `~CLASS_SELECT~` | 31    |
| `~i~`            | 16    |
| `~R1~`           | 8     |
| `~CLASS_EXIT~`   | 8     |
| `~lstick~`       | 8     |
| `~ATTACK_R~`     | 8     |
| `~SHOW_OPTIONS~` | 8     |
| `~CLASS_INFO~`   | 8     |
| `~z~`            | 8     |
| `~Drücke ~`      | 1     |

### classshop.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 50    |
| `~CLASS_SELECT~` | 8     |
| `~ATTACK_L~`     | 8     |
| `~ATTACK_R~`     | 8     |
| `~CLASS_EXIT~`   | 8     |
| `~CLASS_INFO~`   | 8     |

### coaster.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### dodgeballgame.xml

| Control Code    | Count |
| --------------- | ----- |
| `~n~`           | 26    |
| `~DGB_PASS~`    | 16    |
| `~DGB_THROW~`   | 16    |
| `~DGB_CATCH~`   | 16    |
| `~CANCEL~`      | 8     |
| `~DGB_JUMP~`    | 8     |
| `~DGB_DODGE~`   | 8     |
| `~FIRE_WEAPON~` | 8     |
| `~DGB_SWITCH~`  | 8     |

### e.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 7     |

### frontend.xml

| Control Code    | Count |
| --------------- | ----- |
| `~n~`           | 704   |
| `~i~`           | 328   |
| `~CANCEL~`      | 240   |
| `~dup~`         | 216   |
| `~ddown~`       | 216   |
| `~dright~`      | 208   |
| `~dleft~`       | 208   |
| `~a~`           | 184   |
| `~CONFIRM~`     | 176   |
| `~z~`           | 136   |
| `~x~`           | 56    |
| `~f~`           | 39    |
| `~right~`       | 32    |
| `~left~`        | 32    |
| `~LOOK_BACK~`   | 24    |
| `~ACTION~`      | 16    |
| `~SAVE_RETRY~`  | 16    |
| `~PHOTO_RETRY~` | 8     |
| `~$~`           | 8     |
| `~BULLY_CREST~` | 8     |
| `~start~`       | 8     |
| `~ATTACK~`      | 8     |
| `~infinity~`    | 8     |
| `~CROUCH~`      | 7     |
| `~P_ZOOM_OUT~`  | 7     |
| `~nbsp~`        | 1     |

### general.xml

| Control Code                | Count |
| --------------------------- | ----- |
| `~n~`                       | 3093  |
| `~ACTION~`                  | 1080  |
| `~i~`                       | 928   |
| `~bullet~`                  | 602   |
| `~MANUAL_LOCK~`             | 272   |
| `~TAG_COMBO2~`              | 216   |
| `~TAG_COMBO1~`              | 184   |
| `~FIRE_WEAPON~`             | 183   |
| `~CANCEL~`                  | 176   |
| `~a~`                       | 144   |
| `~CONFIRM~`                 | 136   |
| `~THUMBS_UP~`               | 136   |
| `~TAG_COMBO3~`              | 120   |
| `~w~`                       | 112   |
| `~SCROLL_WEAPR~`            | 112   |
| `~TAG_COMBO4~`              | 112   |
| `~SCROLL_WEAPL~`            | 104   |
| `~$~`                       | 96    |
| `~TAG_START~`               | 96    |
| `~ACCELERATE~`              | 95    |
| `~lstick~`                  | 95    |
| `~BRAKE~`                   | 79    |
| `~nbsp~`                    | 70    |
| `~g~`                       | 69    |
| `~rstick~`                  | 64    |
| `~RUN~`                     | 64    |
| `~s_humil~`                 | 57    |
| `~THUMBS_DOWN~`             | 56    |
| `~objective~`               | 56    |
| `~P_ZOOM_IN~`               | 56    |
| `~s_shove~`                 | 48    |
| `~HUMILIATE~`               | 41    |
| `~h~`                       | 40    |
| `~ambient~`                 | 40    |
| `~s_sorry~`                 | 40    |
| `~JUMP~`                    | 40    |
| `~s_pay~`                   | 40    |
| `~SHOW_PRIM_OBJ~`           | 38    |
| `~bike~`                    | 32    |
| `~mission~`                 | 32    |
| `~s_greet~`                 | 32    |
| `~dleft~`                   | 25    |
| `~dright~`                  | 25    |
| `~z~`                       | 24    |
| `~f~`                       | 24    |
| `~job~`                     | 24    |
| `~class~`                   | 24    |
| `~ATTACK~`                  | 23    |
| `~P_ZOOM_OUT~`              | 23    |
| `~TAKE_PHOTO~`              | 23    |
| `~y~`                       | 23    |
| `~vendetta~`                | 16    |
| `~hudelems_social_errands~` | 16    |
| `~copyr~`                   | 16    |
| `~save~`                    | 16    |
| `~blipup~`                  | 16    |
| `~blipdown~`                | 16    |
| `~WEAPON_FIRE~`             | 16    |
| `~GRAPPLE~`                 | 16    |
| `~race~`                    | 16    |
| `~bus~`                     | 16    |
| `~1~`                       | 16    |
| `~SHOW_OPTIONS~`            | 15    |
| `~o~`                       | 9     |
| `~tod~`                     | 8     |
| `~SOCCER_KEEPUP4~`          | 8     |
| `~q~`                       | 8     |
| `~s_taunt2~`                | 8     |
| `~logo~`                    | 8     |
| `~BIKE_TRICK~`              | 8     |
| `~DISMOUNT~`                | 8     |
| `~REVERSAL_THREE~`          | 8     |
| `~SOCCER_KEEPUP3~`          | 8     |
| `~GIVE_ITEM2~`              | 8     |
| `~right~`                   | 8     |
| `~left~`                    | 8     |
| `~SOCCER_KEEPUP1~`          | 8     |
| `~SHOW_SEC_OBJ~`            | 8     |
| `~SHOVEL~`                  | 8     |
| `~HORN~`                    | 8     |
| `~TREE_TURN_AROUND~`        | 8     |
| `~LOOK_BACK~`               | 8     |
| `~REVERSAL_ONE~`            | 8     |
| `~R2~`                      | 8     |
| `~GIVE_ITEM1~`              | 8     |
| `~s_flower~`                | 8     |
| `~s_kiss~`                  | 8     |
| `~REVERSAL_TWO~`            | 8     |
| `~OLLIE~`                   | 8     |
| `~INCREASE_BET~`            | 8     |
| `~DECREASE_BET~`            | 8     |
| `~enemy~`                   | 8     |
| `~B~`                       | 8     |
| `~REVERSAL_FOUR~`           | 8     |
| `~HELP~`                    | 8     |
| `~LOAD~`                    | 8     |
| `~SAVE~`                    | 8     |
| `~SOCCER_KEEPUP2~`          | 8     |
| `~clothing~`                | 8     |
| `~CROUCH~`                  | 7     |
| `~cent~`                    | 7     |
| `~dup~`                     | 7     |
| `~ddown~`                   | 7     |
| `~HAND_BRAKE~`              | 7     |
| `~HAND_BREAK~`              | 1     |

### gokart.xml

| Control Code | Count |
| ------------ | ----- |
| `~a~`        | 16    |

### gokart_sr1.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 4     |

### gokart_sr2.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 2     |

### gokart_sr3.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 1     |

### gokartraces.xml

| Control Code   | Count |
| -------------- | ----- |
| `~a~`          | 16    |
| `~n~`          | 16    |
| `~ACCELERATE~` | 8     |
| `~BRAKE~`      | 8     |
| `~HAND_BRAKE~` | 8     |

### graffiticleanup.xml

| Control Code  | Count |
| ------------- | ----- |
| `~i~`         | 24    |
| `~n~`         | 13    |
| `~TAG_START~` | 8     |
| `~lstick~`    | 8     |
| `~a~`         | 8     |

### lawnmowing.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 16    |
| `~n~`        | 2     |

### mgart2p.xml

| Control Code       | Count |
| ------------------ | ----- |
| `~CLASS_EXIT~`     | 24    |
| `~CLASS_INFO~`     | 16    |
| `~CLASS_CONTINUE~` | 8     |
| `~CLASS_START~`    | 8     |
| `~CLASS_RETRY~`    | 8     |
| `~WII_B~`          | 8     |
| `~n~`              | 3     |

### mgbaseballtoss.xml

| Control Code      | Count |
| ----------------- | ----- |
| `~n~`             | 34    |
| `~special1~`      | 8     |
| `~CONFIRM~`       | 8     |
| `~CANCEL~`        | 8     |
| `~i~`             | 8     |
| `~B~`             | 8     |
| `~lstick~`        | 8     |
| `~rstick~`        | 8     |
| `~MG_THROW_BALL~` | 8     |

### mgbiology2p.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 1195  |
| `~CLASS_SELECT~` | 40    |
| `~i~`            | 8     |
| `~CLASS_EXIT~`   | 8     |
| `~lstick~`       | 8     |
| `~ATTACK_R~`     | 8     |
| `~SHOW_OPTIONS~` | 8     |
| `~CLASS_INFO~`   | 8     |

### mgcarnistriker.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 23    |
| `~CONFIRM~`  | 8     |
| `~CANCEL~`   | 8     |
| `~ACTION~`   | 8     |

### mgchem2p.xml

| Control Code            | Count |
| ----------------------- | ----- |
| `~n~`                   | 49    |
| `~CLASS_SABOTAGE_ICON~` | 16    |
| `~CLASS_SELECT~`        | 16    |
| `~ATTACK_L~`            | 8     |
| `~ATTACK_R~`            | 8     |
| `~CLASS_EXIT~`          | 8     |
| `~CLASS_INFO~`          | 8     |

### mgdarts.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 64    |
| `~n~`        | 33    |
| `~CONFIRM~`  | 24    |
| `~CANCEL~`   | 8     |

### mgdunktank.xml

| Control Code      | Count |
| ----------------- | ----- |
| `~n~`             | 64    |
| `~CONFIRM~`       | 32    |
| `~MG_THROW_BALL~` | 17    |
| `~lstick~`        | 9     |
| `~rstick~`        | 9     |
| `~B~`             | 8     |
| `~CLASS_INFO~`    | 8     |
| `~CANCEL~`        | 7     |
| `~ACTION~`        | 7     |
| `~nbsp~`          | 1     |

### mgenglish2p.xml

| Control Code       | Count |
| ------------------ | ----- |
| `~n~`              | 65    |
| `~CLASS_SELECT~`   | 24    |
| `~CANCEL~`         | 16    |
| `~ACTION~`         | 16    |
| `~CLASS_SCRAMBLE~` | 16    |
| `~CLASS_INFO~`     | 16    |
| `~i~`              | 16    |
| `~CLASS_EXIT~`     | 8     |
| `~lstick~`         | 8     |
| `~SHOW_OPTIONS~`   | 8     |
| `~z~`              | 8     |

### mghacky.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 33    |
| `~CONFIRM~`      | 16    |
| `~CANCEL~`       | 16    |
| `~lstick~`       | 8     |
| `~rstick~`       | 8     |
| `~$~`            | 8     |
| `~INCREASE_BET~` | 8     |
| `~DECREASE_BET~` | 8     |

### mglawnmowing2p.xml

| Control Code | Count |
| ------------ | ----- |
| `~n~`        | 56    |

### mgmath2p.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 250   |
| `~CLASS_SELECT~` | 16    |
| `~CLASS_INFO~`   | 16    |
| `~i~`            | 16    |
| `~CONFIRM~`      | 8     |
| `~CLASS_EXIT~`   | 8     |
| `~lstick~`       | 8     |
| `~ATTACK_R~`     | 8     |
| `~SHOW_OPTIONS~` | 8     |
| `~z~`            | 8     |

### mgmusic2p.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 38    |
| `~MANUAL_LOCK~`  | 8     |
| `~FIRE_WEAPON~`  | 8     |
| `~SHOW_OPTIONS~` | 8     |
| `~CLASS_INFO~`   | 8     |
| `~CLASS_SELECT~` | 8     |

### mgshooting2p.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 212   |
| `~i~`            | 48    |
| `~FIRE_WEAPON~`  | 32    |
| `~ATTACK_R~`     | 16    |
| `~special3~`     | 8     |
| `~special1~`     | 8     |
| `~special2~`     | 8     |
| `~CONFIRM~`      | 8     |
| `~CANCEL~`       | 8     |
| `~lstick~`       | 8     |
| `~MANUAL_LOCK~`  | 8     |
| `~SHOW_OPTIONS~` | 8     |
| `~CLASS_INFO~`   | 8     |
| `~CLASS_SELECT~` | 8     |

### mgshootinggallery.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 95    |
| `~i~`            | 48    |
| `~FIRE_WEAPON~`  | 16    |
| `~ATTACK_R~`     | 8     |
| `~CLASS_DELETE~` | 8     |
| `~WII_RPAD~`     | 8     |
| `~CLASS_EXIT~`   | 8     |
| `~CLASS_INFO~`   | 8     |
| `~B~`            | 8     |
| `~lstick~`       | 8     |
| `~rstick~`       | 8     |
| `~special3~`     | 8     |
| `~special1~`     | 8     |
| `~special2~`     | 8     |
| `~CONFIRM~`      | 8     |
| `~CANCEL~`       | 8     |
| `~CLASS_SELECT~` | 8     |

### mgsocpen.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 34    |
| `~i~`            | 32    |
| `~CONFIRM~`      | 16    |
| `~CANCEL~`       | 16    |
| `~$~`            | 8     |
| `~CLASS_INFO~`   | 8     |
| `~INCREASE_BET~` | 8     |
| `~DECREASE_BET~` | 8     |
| `~ACTION~`       | 8     |
| `~z~`            | 8     |

### mobile.xml

| Control Code                | Count |
| --------------------------- | ----- |
| `~n~`                       | 471   |
| `~hud_check~`               | 278   |
| `~hud_punch~`               | 168   |
| `~leftyrighty~`             | 154   |
| `~hud_button_x~`            | 147   |
| `~hud_target~`              | 92    |
| `~rightylefty~`             | 56    |
| `~hud_throw~`               | 49    |
| `~dleft~`                   | 42    |
| `~dright~`                  | 42    |
| `~hud_yes~`                 | 42    |
| `~hud_grab~`                | 37    |
| `~hud_accelerate~`          | 35    |
| `~hud_jump~`                | 34    |
| `~s_sorry~`                 | 28    |
| `~CONFIRM~`                 | 28    |
| `~hud_brake~`               | 28    |
| `~hud_drop_jetpack~`        | 24    |
| `~hud_save~`                | 23    |
| `~hud_camera~`              | 23    |
| `~hud_crouch~`              | 22    |
| `~FIRE_WEAPON~`             | 22    |
| `~a~`                       | 22    |
| `~s_greet~`                 | 21    |
| `~s_humil~`                 | 21    |
| `~s_pay~`                   | 21    |
| `~special1~`                | 21    |
| `~CANCEL~`                  | 21    |
| `~s_shove~`                 | 21    |
| `~hud_buy~`                 | 16    |
| `~hud_climb~`               | 16    |
| `~hud_prank~`               | 14    |
| `~lstick~`                  | 14    |
| `~hud_minus~`               | 14    |
| `~hud_plus~`                | 14    |
| `~hud_back~`                | 14    |
| `~hud_button_y~`            | 14    |
| `~hud_button_b~`            | 14    |
| `~hud_takedown~`            | 14    |
| `~4_05_bull_piss~`          | 14    |
| `~hud_x~`                   | 14    |
| `~rstick~`                  | 14    |
| `~hud_ebrake~`              | 14    |
| `~hud_clothes~`             | 8     |
| `~hud_info~`                | 8     |
| `~hud_sleep~`               | 8     |
| `~hud_bicycle~`             | 8     |
| `~button_chem_cylinder~`    | 8     |
| `~hud_left~`                | 8     |
| `~hud_right~`               | 8     |
| `~MANUAL_LOCK~`             | 8     |
| `~CLASS_EXIT~`              | 8     |
| `~CLASS_INFO~`              | 8     |
| `~CLASS_SELECT~`            | 8     |
| `~hud_up~`                  | 7     |
| `~hud_melee~`               | 7     |
| `~special3~`                | 7     |
| `~special2~`                | 7     |
| `~hudelems_social_errands~` | 7     |
| `~INCREASE_BET~`            | 7     |
| `~DECREASE_BET~`            | 7     |
| `~mission~`                 | 7     |
| `~SHOVEL~`                  | 7     |
| `~s_kiss~`                  | 7     |
| `~s_flower~`                | 7     |
| `~hud_horn~`                | 7     |
| `~hud_spraycan~`            | 7     |
| `~hud_block~`               | 7     |
| `~s_taunt2~`                | 7     |
| `~hud_button_l1~`           | 7     |
| `~hud_button_r1~`           | 7     |
| `~hud_turn_left~`           | 6     |
| `~nbsp~`                    | 4     |
| `~ - Turn around~`          | 1     |
| `~ ~`                       | 1     |
| `~~`                        | 1     |

### mpart.xml

| Control Code       | Count |
| ------------------ | ----- |
| `~CLASS_EXIT~`     | 3     |
| `~CLASS_INFO~`     | 2     |
| `~CLASS_CONTINUE~` | 1     |
| `~CLASS_RETRY~`    | 1     |
| `~CLASS_START~`    | 1     |

### mpbiology.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 56    |
| `~CLASS_SELECT~` | 30    |
| `~R2~`           | 27    |
| `~CLASS_EXIT~`   | 2     |
| `~lstick~`       | 2     |
| `~rstick~`       | 2     |
| `~ATTACK_R~`     | 2     |
| `~CLASS_INFO~`   | 2     |
| `~i~`            | 2     |
| `~z~`            | 1     |

### mpchem.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 5     |
| `~CLASS_SELECT~` | 1     |
| `~ATTACK_L~`     | 1     |
| `~ATTACK_R~`     | 1     |
| `~CLASS_EXIT~`   | 1     |
| `~CLASS_INFO~`   | 1     |

### mpenglish.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 6     |
| `~CLASS_SELECT~` | 3     |
| `~CLASS_DELETE~` | 2     |
| `~i~`            | 2     |
| `~FIRE_WEAPON~`  | 2     |
| `~CLASS_EXIT~`   | 1     |
| `~lstick~`       | 1     |
| `~ACTION~`       | 1     |
| `~z~`            | 1     |
| `~CLASS_INFO~`   | 1     |

### mpgeography.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 8     |
| `~CLASS_SELECT~` | 5     |
| `~R2~`           | 3     |
| `~i~`            | 3     |
| `~CLASS_EXIT~`   | 2     |
| `~R1~`           | 1     |
| `~CLASS_INFO~`   | 1     |
| `~z~`            | 1     |

### mpmath.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 34    |
| `~i~`            | 2     |
| `~CLASS_SELECT~` | 2     |
| `~CLASS_INFO~`   | 2     |
| `~CLASS_EXIT~`   | 2     |
| `~CONFIRM~`      | 1     |
| `~lstick~`       | 1     |
| `~rstick~`       | 1     |
| `~R2~`           | 1     |
| `~ATTACK_R~`     | 1     |
| `~z~`            | 1     |

### mpmusic.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 4     |
| `~MANUAL_LOCK~`  | 2     |
| `~CLASS_SELECT~` | 1     |
| `~FIRE_WEAPON~`  | 1     |
| `~CLASS_EXIT~`   | 1     |
| `~CLASS_INFO~`   | 1     |
| `~i~`            | 1     |

### mpshop.xml

| Control Code     | Count |
| ---------------- | ----- |
| `~n~`            | 5     |
| `~CLASS_SELECT~` | 1     |
| `~ATTACK_L~`     | 1     |
| `~ATTACK_R~`     | 1     |
| `~CLASS_EXIT~`   | 1     |
| `~CLASS_INFO~`   | 1     |

### nt_dares.xml

| Control Code | Count |
| ------------ | ----- |
| `~left~`     | 8     |
| `~right~`    | 8     |
| `~CONFIRM~`  | 8     |

### p_snow.xml

| Control Code | Count |
| ------------ | ----- |
| `~i~`        | 8     |
| `~n~`        | 1     |

### testmissionlog.xml

| Control Code | Count |
| ------------ | ----- |
| `~a~`        | 14    |
| `~i~`        | 14    |
| `~f~`        | 14    |

### wrestling1.xml

| Control Code         | Count |
| -------------------- | ----- |
| `~n~`                | 95    |
| `~ATTACK~`           | 88    |
| `~ATTACK_R~`         | 64    |
| `~GRAPPLE~`          | 24    |
| `~nbsp~`             | 17    |
| `~MANUAL_LOCK~`      | 16    |
| `~ACTION~`           | 8     |
| `~GRAPPLE_TAKEDOWN~` | 8     |
| `~JUMP~`             | 8     |
| `~ATTACK_L~`         | 8     |
