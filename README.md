# SNAFU Weapons Documentation

Every weapon, attachment, magazine and ammo type defined in the SNAFU weapon packs, sorted by weapon type.
Everything here was read from the mod's `config.cpp` / `*_config.cpp` files. Class names are exactly as in the configs,
so you can copy them into `types.xml`, trader configs or loadouts.

## Overview

| Type | Weapons (incl. color variants) |
|---|---|
| [Sniper Rifles](#sniper-rifles) | 31 |
| [DMR / Marksman Rifles](#dmr--marksman-rifles) | 28 |
| [Assault & Battle Rifles (AR)](#assault--battle-rifles-ar) | 69 |
| [Light Machine Guns (LMG)](#light-machine-guns-lmg) | 10 |
| [Submachine Guns (SMG) & PDWs](#submachine-guns-smg--pdws) | 17 |
| [Shotguns](#shotguns) | 8 |
| [Pistols & Revolvers](#pistols--revolvers) | 11 |
| [Test / Duplicate Classes](#test--duplicate-classes) | 3 |
| **Total spawnable weapons** | **177** |

Also in this document: [Attachments](#attachments), [Attachment slots](#attachment-slots), [Magazines](#magazines), [Ammunition](#ammunition), [Mod folders](#mod-folders).

**How to read the tables**

- **Class name**: the spawn name used in `types.xml`.
- **Caliber**: what the gun is chambered for. The exact ammo classes are in [Ammunition](#ammunition).
- **Magazines**: mod magazines by class name. "vanilla: ..." means the gun also takes those vanilla DayZ magazine families.
- **Attachment slots**: the slot names on the gun. See [Attachment slots](#attachment-slots) for which items fit each slot.
- **Mod**: the PBO folder the weapon comes from.

## Sniper Rifles

Bolt-action and anti-materiel rifles. 31 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `SNAFU_FRF2` | FR-F2 Sniper Rifle | .308 Win / 7.62x51mm | SemiAuto | `SNAFU_FRF2_Mag` | [list](#snafu_frf2) | SNAFU_WW2 |
| `GCGN_M700` | Remington Model 700 | .308 Win / 7.62x51mm | Single | `GCGN_M700_Mag` | [list](#gcgn_m700) | GCGN_Guns |
| `SNAFU_M48` | Zastava M48 | .308 Win / 7.62x51mm | Single | internal (loads rounds directly) | [list](#snafu_m48) | SNAFU_WW2 |
| `SNAFU_AWM_GUN` | AWM 338 | .338 Lapua Magnum | Single | `SNAFU_AWM_Mag` | [list](#snafu_awm_gun) | SNAFU_Guns_01 |
| `SNAFUM98B_Atac_GUN` | Atac M98B | .338 Lapua Magnum | SemiAuto | `SNAFUM98B_Mag` | [list](#snafum98b_atac_gun) | SNAFU_Guns_01 |
| `SNAFUT5000_Dkmcc_GUN` | DKMC T5000 | .338 Lapua Magnum | Single | `SNAFUT5000_Mag` | [list](#snafut5000_dkmcc_gun) | SNAFU_Guns_01 |
| `SNAFUDVL10M2` | DVL-10 M2 | .338 Lapua Magnum | Single | `SNAFUDVL10M2_5rdMag` | [list](#snafudvl10m2) | SNAFU_Guns_06 |
| `SNAFUM98B_Digi_GUN` | Digi M98B | .338 Lapua Magnum | SemiAuto | `SNAFUM98B_Mag` | [list](#snafum98b_atac_gun) | SNAFU_Guns_01 |
| `SNAFUM98B_Ger_GUN` | Ger M98B | .338 Lapua Magnum | SemiAuto | `SNAFUM98B_Mag` | [list](#snafum98b_atac_gun) | SNAFU_Guns_01 |
| `SNAFUM98B_Mc_GUN` | MC M98B | .338 Lapua Magnum | SemiAuto | `SNAFUM98B_Mag` | [list](#snafum98b_atac_gun) | SNAFU_Guns_01 |
| `SNAFUM24_GUN` | SNAFU M24A3 | .338 Lapua Magnum | Single | `SNAFUM24_Mag` | [list](#snafum24_gun) | SNAFU_Guns_01 |
| `SNAFUSRSA2` | SRS A2 | .338 Lapua Magnum | Single | `SNAFUSRSA2_10rdMag` | [list](#snafusrsa2) | SNAFU_Guns_06 |
| `SNAFUM98B_Snow_GUN` | Snow M98B | .338 Lapua Magnum | SemiAuto | `SNAFUM98B_Mag` | [list](#snafum98b_atac_gun) | SNAFU_Guns_01 |
| `SNAFUT5000_Snow_GUN` | Snow T5000 | .338 Lapua Magnum | Single | `SNAFUT5000_Mag` | [list](#snafut5000_dkmcc_gun) | SNAFU_Guns_01 |
| `SNAFUTac21` | Tac-21 | .338 Lapua Magnum | Single | `SNAFUTac21_5rdMag` | [list](#snafutac21) | SNAFU_Guns_06 |
| `SNAFUM98B_Wood_GUN` | Wood M98B | .338 Lapua Magnum | SemiAuto | `SNAFUM98B_Mag` | [list](#snafum98b_atac_gun) | SNAFU_Guns_01 |
| `SNAFUT5000_Wood_GUN` | Wood T5000 | .338 Lapua Magnum | Single | `SNAFUT5000_Mag` | [list](#snafut5000_dkmcc_gun) | SNAFU_Guns_01 |
| `SNAFU_M300BK` | CheyTac M300 Black | .408 CheyTac | Single | `GCGN_M200_Mag`<br>`SNAFU_M300Mag` | [list](#snafu_m300bk) | SNAFU_Guns_02 |
| `SNAFU_M300TAN` | CheyTac M300 Desert | .408 CheyTac | Single | `GCGN_M200_Mag`<br>`SNAFU_M300Mag` | [list](#snafu_m300bk) | SNAFU_Guns_02 |
| `SNAFU_M300Green` | CheyTac M300 Forest | .408 CheyTac | Single | `GCGN_M200_Mag`<br>`SNAFU_M300Mag` | [list](#snafu_m300bk) | SNAFU_Guns_02 |
| `GCGN_M200` | M200 CheyTac Black | .408 CheyTac | Single | `GCGN_M200_Mag`<br>`SNAFU_M300Mag` | [list](#gcgn_m200) | GCGN_Guns |
| `SNAFU_M200Green` | M200 CheyTac Green | .408 CheyTac | Single | `GCGN_M200_Mag`<br>`SNAFU_M300Mag` | [list](#gcgn_m200) | GCGN_Guns |
| `SNAFU_M200SNOW` | M200 CheyTac Snow | .408 CheyTac | Single | `GCGN_M200_Mag`<br>`SNAFU_M300Mag` | [list](#gcgn_m200) | GCGN_Guns |
| `GCGN_M200_Tan` | M200 CheyTac Tan | .408 CheyTac | Single | `GCGN_M200_Mag`<br>`SNAFU_M300Mag` | [list](#gcgn_m200) | GCGN_Guns |
| `SNAFUM96` | M96 | .408 CheyTac | Single | `SNAFUM96_5rdMag` | [list](#snafum96) | SNAFU_Guns_06 |
| `SNAFU_AS50_GUN` | AS50 | .50 BMG | SemiAuto | `SNAFU_AS50_Mag` | [list](#snafu_as50_gun) | SNAFU_Guns_01 |
| `GCGN_M82_Barret` | GCGN M82 Barret Black | .50 BMG | SemiAuto | `GCGN_M82_Mag` | [list](#gcgn_m82_barret) | GCGN_Guns |
| `SNAFUGM6Lynx` | GM6 Lynx | .50 BMG | SemiAuto | `SNAFUGM6Lynx_5rdMag` | [list](#snafugm6lynx) | SNAFU_Guns_06 |
| `SNAFUAX50_GUN` | SNAFU AX50 | .50 BMG | SemiAuto | `SNAFUAX50_Mag` | [list](#snafuax50_gun) | SNAFU_Guns_01 |
| `SNAFUVSSK` | VSSK | 12.7x55mm / 12.7x55mm AP | SemiAuto | `SNAFUVSSK_5rdMag` | [list](#snafuvssk) | SNAFU_Guns_02 |
| `SNAFUAlligator` | Snipex Alligator | 14.5x114mm | Single | `SNAFUAlligator_5rdMag` | [list](#snafualligator) | SNAFU_Guns_06 |

## DMR / Marksman Rifles

Semi-automatic precision rifles, plus classic semi-auto and lever-action rifles. 28 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `GCGN_M1Garand` | M1Garand | .30-06 Springfield | SemiAuto | internal (loads rounds directly) | [list](#gcgn_m1garand) | GCGN_Guns |
| `SNHK417_Gun` | Heckler & Koch HK417 | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag` | [list](#snhk417_gun) | Guns_01 |
| `GCGN_M110_Black` | M110 Semi-Automatic Black | .308 Win / 7.62x51mm | SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag` | [list](#gcgn_m110_black) | GCGN_Guns |
| `GCGN_M110_Green` | M110 Semi-Automatic Green | .308 Win / 7.62x51mm | SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag` | [list](#gcgn_m110_black) | GCGN_Guns |
| `GCGN_M110_Tan` | M110 Semi-Automatic Tan | .308 Win / 7.62x51mm | SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag` | [list](#gcgn_m110_black) | GCGN_Guns |
| `SNAFUM1A_Black` | M1A | .308 Win / 7.62x51mm | SemiAuto | `SNAFU_M14_Mag`<br>`SNAFUM1A_20rdMag` | [list](#snafum1a_black) | SNAFU_Guns_06 |
| `SNAFUM1A_Green` | M1A | .308 Win / 7.62x51mm | SemiAuto | `SNAFU_M14_Mag`<br>`SNAFUM1A_20rdMag` | [list](#snafum1a_black) | SNAFU_Guns_06 |
| `SNAFUM1A_Tan` | M1A | .308 Win / 7.62x51mm | SemiAuto | `SNAFU_M14_Mag`<br>`SNAFUM1A_20rdMag` | [list](#snafum1a_black) | SNAFU_Guns_06 |
| `SNAFU_Saint_Gun` | SAINT VICTOR 308 | .308 Win / 7.62x51mm | SemiAuto | `SNAFU_Saint_Mag` | [list](#snafu_saint_gun) | SNAFU_Guns_02 |
| `SNAFURSASS_dkmc_GUN` | SNAFU RSASS DKMC | .308 Win / 7.62x51mm | SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag`<br>`SNAFURSASS_Mag` | [list](#snafursass_dkmc_gun) | SNAFU_Guns_01 |
| `SNAFURSASS_od_GUN` | SNAFU RSASS OD | .308 Win / 7.62x51mm | SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag`<br>`SNAFURSASS_Mag` | [list](#snafursass_dkmc_gun) | SNAFU_Guns_01 |
| `SNAFURSASS_Wood_GUN` | SNAFU RSASS Wood | .308 Win / 7.62x51mm | SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag`<br>`SNAFURSASS_Mag` | [list](#snafursass_dkmc_gun) | SNAFU_Guns_01 |
| `SNAFU_SR25_Gun` | SNAFU SR25 | .308 Win / 7.62x51mm | SemiAuto | `GCGN_M110_Mag`<br>`SNAFU_SR25_Mag`<br>`SNHK417_Mag`<br>`SNAFU_Saint_Mag`<br>`SNAFURSASS_Mag` | [list](#snafu_sr25_gun) | SNAFU_Guns_01 |
| `SNAFU_M76` | Zastava M76 | .308 Win / 7.62x51mm | SemiAuto | `SNAFU_M76_Mag` | [list](#snafu_m76) | SNAFU_WW2 |
| `SNAFUGevar_Black` | Gevar Mk-3 Black | .338 Lapua Magnum | SemiAuto | `SNAFUGevar_10rdMag` | [list](#snafugevar_black) | SNAFU_Guns_06 |
| `SNAFUGevar_Green` | Gevar Mk-3 Green | .338 Lapua Magnum | SemiAuto | `SNAFUGevar_10rdMag` | [list](#snafugevar_black) | SNAFU_Guns_06 |
| `SNAFUGevar_Grey` | Gevar Mk-3 Grey | .338 Lapua Magnum | SemiAuto | `SNAFUGevar_10rdMag` | [list](#snafugevar_black) | SNAFU_Guns_06 |
| `SNAFUGevar_Tan` | Gevar Mk-3 Tan | .338 Lapua Magnum | SemiAuto | `SNAFUGevar_10rdMag` | [list](#snafugevar_black) | SNAFU_Guns_06 |
| `SNAFUKivaari_Black_GUN` | Kivaari Black | .338 Lapua Magnum | SemiAuto | `SNAFUKivaari_10rdMag`<br>`SNAFUKivaari_25rdMag` | [list](#snafukivaari_black_gun) | SNAFU_Guns_03 |
| `SNAFUKivaari_Grey_GUN` | Kivaari Grey | .338 Lapua Magnum | SemiAuto | `SNAFUKivaari_10rdMag`<br>`SNAFUKivaari_25rdMag` | [list](#snafukivaari_black_gun) | SNAFU_Guns_03 |
| `SNAFUKivaari_Snow_GUN` | Kivaari Snow | .338 Lapua Magnum | SemiAuto | `SNAFUKivaari_10rdMag`<br>`SNAFUKivaari_25rdMag` | [list](#snafukivaari_black_gun) | SNAFU_Guns_03 |
| `SNAFUKivaari_Tan_GUN` | Kivaari Tan | .338 Lapua Magnum | SemiAuto | `SNAFUKivaari_10rdMag`<br>`SNAFUKivaari_25rdMag` | [list](#snafukivaari_black_gun) | SNAFU_Guns_03 |
| `SNAFU_MAR10_Black_GUN` | MAR10 Black | .338 Lapua Magnum | SemiAuto | `SNAFU_Mar10_15rnd_Mag` | [list](#snafu_mar10_black_gun) | SNAFU_Guns_03 |
| `SNAFUMarlin1895` | Marlin 1895 | .45-70 Government | Single | internal (loads rounds directly) | [list](#snafumarlin1895) | SNAFU_Guns_06 |
| `SNAFU_CALI_GUN` | JJFU Nomad | 5.56x45mm | SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_cali_gun) | SNAFU_Guns_01 |
| `SNAFUMk12` | Mk 12 Mod 1 | 5.56x45mm | SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMk12_20rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumk12) | SNAFU_Guns_06 |
| `SNAFU_RDB` | RDB-17 | 5.56x45mm | SemiAuto | vanilla: STANAG, CMAG | [list](#snafu_rdb) | SNAFU_Guns_05 |
| `SNAFU_SKS` | Zastava M59/66 PAP | 7.62x39mm | SemiAuto | `SNAFU_SKS_10Rnd_Mag`<br>`SNAFU_SKS_30Rnd_Mag` | [list](#snafu_sks) | SNAFU_WW2 |

## Assault & Battle Rifles (AR)

Select-fire rifles and carbines. 69 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `SNAFU_M1918A2` | M1918 Browning Rifle | .30-06 Springfield | FullAuto, SemiAuto | `SNAFU_M1918A2_Mag` | - | SNAFU_WW2 |
| `SNAFU_AR15SPRBK` | 300AC AR15 BK | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_ar15sprbk) | SNAFU_Guns_02 |
| `SNAFUAR15_SPR_Black_GUN` | 300AC AR15 Black | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_ar15sprbk) | SNAFU_Guns_02 |
| `SNAFUAR15_SPR_Tan_GUN` | 300AC AR15 Tan | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_ar15sprbk) | SNAFU_Guns_02 |
| `SNAFU_AR15SPRTAN` | 300AC AR15 Tan | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_ar15sprbk) | SNAFU_Guns_02 |
| `SNAFU_M4300AC_10_GUN` | 300AC Carbine M4-10in | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_m4300ac_10_gun) | SNAFU_Guns_02 |
| `SNAFU_M4300AC_14_GUN` | 300AC Carbine M4-14in | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_m4300ac_14_gun) | SNAFU_Guns_02 |
| `SNAFU_M4300AC_16_GUN` | 300AC Carbine M4-16in | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_m4300ac_16_gun) | SNAFU_Guns_02 |
| `SNAFU_M4300AC_14DV_GUN` | 300AC Carbine M4-Vanilla | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_m4300ac_14dv_gun) | SNAFU_Guns_02 |
| `SNAFUHoneyBadger_Black` | AAC Honey Badger | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFUHoneyBadger_30rdMag_Black`<br>`SNAFUHoneyBadger_30rdMag_Tan` | [list](#snafuhoneybadger_black) | SNAFU_Guns_06 |
| `SNAFUHoneyBadger_Tan` | AAC Honey Badger | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFUHoneyBadger_30rdMag_Black`<br>`SNAFUHoneyBadger_30rdMag_Tan` | [list](#snafuhoneybadger_black) | SNAFU_Guns_06 |
| `SNAFU_KAC_Gun` | KAC PDW | .300 AAC Blackout | FullAuto, SemiAuto | `SNAFU_CMAG30300_Black`<br>`SNAFU_CMAG30300_Tan`<br>`SNAFU_CMAG40300_Black`<br>`SNAFU_CMAG40300_Tan`<br>`SNAFU_CMAG60300_Black`<br>`SNAFU_CMAG60300_Tan`<br>`SNAFU_BMAG300_Tan`<br>`SNAFU_BMAG300_Black`<br>`SNAFUAR15_SPR_30RND_Mag`<br>`SNAFUAR15_SPR_40RND_Mag`<br>`SNAFUAR15_SPR_60RND_Mag`<br>`SNAFUAR15_SPR_100RND_Mag`<br>`SNAFU_KAC_Mag` | [list](#snafu_kac_gun) | SNAFU_Guns_01 |
| `SNAFU_AK308` | AK-308 Assault Rifle | .308 Win / 7.62x51mm | FullAuto, Burst, SemiAuto | `SNAFU_AK308_Mag` | [list](#snafu_ak308) | SNAFU_Guns |
| `SNAFUDSASA58_Gun` | DSA SA58 | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `SA58_DrumMag`<br>`SA58_30RND_BK`<br>`SA58_30RND_WBK`<br>`SA58_30RND_DT`<br>`GCGN_Mag_FAL_50Rnd`<br>vanilla: FAL | [list](#snafudsasa58_gun) | SNAFU_Guns_02 |
| `SNAFU_G3A3` | G3A3 | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `SNAFU_G3A3_20rdMag` | [list](#snafu_g3a3) | SNAFU_Guns_05 |
| `SNAFU_M14` | M14 Battle Rifle | .308 Win / 7.62x51mm | SemiAuto, FullAuto | `SNAFU_M14_Mag`<br>`SNAFUM1A_20rdMag` | [list](#snafu_m14) | SNAFU_WW2 |
| `SNSA58_Gun` | SA58 | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `SA58_DrumMag`<br>`SA58_30RND_BK`<br>`SA58_30RND_WBK`<br>`SA58_30RND_DT`<br>`GCGN_Mag_FAL_50Rnd`<br>vanilla: FAL | [list](#snsa58_gun) | Guns_01 |
| `Snafu_ScarH_Black_GUN` | SNAFU Scar-H BK | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `Snafu_ScarH_25RND_Mag_Tan`<br>`Snafu_ScarH_25RND_Mag_Snow`<br>`Snafu_ScarH_25RND_Mag_OD`<br>`Snafu_ScarH_25RND_Mag_DKMC`<br>`Snafu_ScarH_25RND_Mag_BK`<br>`Modified_SA58_30RND_BK`<br>`Modified_SA58_30RND_WBK`<br>`Modified_SA58_30RND_DT`<br>`SNAFU_ScarH_100RND_Mag_Black`<br>`SNAFU_ScarH_100RND_Mag_Tan` | [list](#snafu_scarh_black_gun) | SNAFU_Guns_03 |
| `Snafu_ScarH_DKMC_GUN` | SNAFU Scar-H DKMC | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `Snafu_ScarH_25RND_Mag_Tan`<br>`Snafu_ScarH_25RND_Mag_Snow`<br>`Snafu_ScarH_25RND_Mag_OD`<br>`Snafu_ScarH_25RND_Mag_DKMC`<br>`Snafu_ScarH_25RND_Mag_BK`<br>`Modified_SA58_30RND_BK`<br>`Modified_SA58_30RND_WBK`<br>`Modified_SA58_30RND_DT`<br>`SNAFU_ScarH_100RND_Mag_Black`<br>`SNAFU_ScarH_100RND_Mag_Tan` | [list](#snafu_scarh_black_gun) | SNAFU_Guns_03 |
| `Snafu_ScarH_OD_GUN` | SNAFU Scar-H OD | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `Snafu_ScarH_25RND_Mag_Tan`<br>`Snafu_ScarH_25RND_Mag_Snow`<br>`Snafu_ScarH_25RND_Mag_OD`<br>`Snafu_ScarH_25RND_Mag_DKMC`<br>`Snafu_ScarH_25RND_Mag_BK`<br>`Modified_SA58_30RND_BK`<br>`Modified_SA58_30RND_WBK`<br>`Modified_SA58_30RND_DT`<br>`SNAFU_ScarH_100RND_Mag_Black`<br>`SNAFU_ScarH_100RND_Mag_Tan` | [list](#snafu_scarh_black_gun) | SNAFU_Guns_03 |
| `Snafu_ScarH_Snow_GUN` | SNAFU Scar-H Snow | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `Snafu_ScarH_25RND_Mag_Tan`<br>`Snafu_ScarH_25RND_Mag_Snow`<br>`Snafu_ScarH_25RND_Mag_OD`<br>`Snafu_ScarH_25RND_Mag_DKMC`<br>`Snafu_ScarH_25RND_Mag_BK`<br>`Modified_SA58_30RND_BK`<br>`Modified_SA58_30RND_WBK`<br>`Modified_SA58_30RND_DT`<br>`SNAFU_ScarH_100RND_Mag_Black`<br>`SNAFU_ScarH_100RND_Mag_Tan` | [list](#snafu_scarh_black_gun) | SNAFU_Guns_03 |
| `Snafu_ScarH_Tan_GUN` | SNAFU Scar-H Tan | .308 Win / 7.62x51mm | FullAuto, SemiAuto | `Snafu_ScarH_25RND_Mag_Tan`<br>`Snafu_ScarH_25RND_Mag_Snow`<br>`Snafu_ScarH_25RND_Mag_OD`<br>`Snafu_ScarH_25RND_Mag_DKMC`<br>`Snafu_ScarH_25RND_Mag_BK`<br>`Modified_SA58_30RND_BK`<br>`Modified_SA58_30RND_WBK`<br>`Modified_SA58_30RND_DT`<br>`SNAFU_ScarH_100RND_Mag_Black`<br>`SNAFU_ScarH_100RND_Mag_Tan` | [list](#snafu_scarh_black_gun) | SNAFU_Guns_03 |
| `SNAFUASh12` | ASh-12.7 | 12.7x55mm | FullAuto, SemiAuto | `SNAFUASh12_20rdMag` | [list](#snafuash12) | SNAFU_Guns_06 |
| `SNAFU_AK12A` | AK-12 Assault Rifle | 5.45x39mm | FullAuto, Burst, SemiAuto | `SNAFU_AK12_Mag`<br>`SNAFU_RPK16_Black_Mag`<br>`SNAFU_RPK16_Green_Mag`<br>`SNAFU_RPK16_Tan_Mag`<br>vanilla: AK74 | [list](#snafu_ak12a) | SNAFU_Guns |
| `SNAFU_AEK545_Gun` | SNAFU AEK545 | 5.45x39mm | SemiAuto, FullAuto, Burst | `SNAFU_AK12_Mag`<br>`SNAFU_RPK16_Black_Mag`<br>`SNAFU_RPK16_Green_Mag`<br>`SNAFU_RPK16_Tan_Mag`<br>vanilla: AK74 | [list](#snafu_aek545_gun) | SNAFU_Guns_01 |
| `SNAFU_ADAR_Modular16_GUN` | 5.56 ADAR 16in | 5.56x45mm | SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_adar_modular16_gun) | SNAFU_Guns_02 |
| `SNAFU_AR15_Modular16_GUN` | 5.56 AR15 16in | 5.56x45mm | SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_ar15_modular16_gun) | SNAFU_Guns_02 |
| `M4_6933_Gun` | 5.56 Carbine M4-10in | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#m4_6933_gun) | SNAFU_Guns_02 |
| `SNAFU_M4556_Modular10_GUN` | 5.56 Carbine M4-10in | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_m4556_modular10_gun) | SNAFU_Guns_02 |
| `SNAFU_M4556_Modular14_GUN` | 5.56 Carbine M4-14in | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_m4556_modular14_gun) | SNAFU_Guns_02 |
| `SNAFU_M4556_Modular16_GUN` | 5.56 Carbine M4-16in | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_m4556_modular16_gun) | SNAFU_Guns_02 |
| `GCGN_M4A1` | 5.56 Carbine M4-Vanilla | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#gcgn_m4a1) | SNAFU_Guns_02 |
| `SNAFU_M4556_Modular14DV_GUN` | 5.56 Carbine M4-Vanilla | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_m4556_modular14dv_gun) | SNAFU_Guns_02 |
| `SNAFU_AK19` | AK-19 Assault Rifle | 5.56x45mm | FullAuto, Burst, SemiAuto | vanilla: AK101 | [list](#snafu_ak19) | SNAFU_Guns |
| `SNAFUAUG_BK` | AUG A3 Black | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafuaug_bk) | SNAFU_Guns_06 |
| `SNAFUAUG` | AUG A3 Green | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafuaug_bk) | SNAFU_Guns_06 |
| `SNAFU_AK5C` | Ak 5C | 5.56x45mm | FullAuto, SemiAuto | vanilla: STANAG, CMAG | [list](#snafu_ak5c) | SNAFU_Guns_05 |
| `SNAFU_BR18` | BR18 | 5.56x45mm | FullAuto, SemiAuto | vanilla: STANAG, CMAG | [list](#snafu_br18) | SNAFU_Guns_05 |
| `SNAFU_CZ805_Gun` | CZ805 | 5.56x45mm | FullAuto, Burst, SemiAuto | `GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_cz805_gun) | SNAFU_Guns_01 |
| `SNAFUFAMAS` | FAMAS | 5.56x45mm | FullAuto, Burst, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafufamas) | SNAFU_Guns_06 |
| `SCAR_Gun` | FN SCAR 556 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#scar_gun) | Guns_01 |
| `GCGN_HK416` | Heckler & Koch HK416 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#gcgn_hk416) | GCGN_Guns |
| `HK416_Gun` | Heckler & Koch HK416 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#hk416_gun) | Guns_01 |
| `IA2_Gun` | IA2 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#ia2_gun) | Guns_01 |
| `SNAFU_LVOA556_GUN` | LVOA 5.56 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_lvoa556_gun) | SNAFU_Guns_02 |
| `SNAFUMDARCAR_Black` | MDAR Carbine Black | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARCAR_Green` | MDAR Carbine Green | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARCAR_Tan` | MDAR Carbine Tan | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARRIF_Black` | MDAR Rifle Black | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARRIF_Green` | MDAR Rifle Green | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARRIF_Tan` | MDAR Rifle Tan | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARSBR_Black` | MDAR SBR Black | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARSBR_Green` | MDAR SBR Green | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `SNAFUMDARSBR_Tan` | MDAR SBR Tan | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFUMDAR_30rndMagB`<br>`SNAFUMDAR_30rndMagT`<br>`SNAFUMDAR_60rndMagB`<br>`SNAFUMDAR_60rndMagT`<br>`SNAFUAUG_30rdMag`<br>vanilla: STANAG, CMAG | [list](#snafumdarcar_black) | SNAFU_Guns_02 |
| `MK18_Gun` | MK18 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#mk18_gun) | Guns_01 |
| `ACR_Gun` | Remington ACR | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`GCGN_Acr_Mag`<br>vanilla: STANAG, CMAG | [list](#acr_gun) | Guns_01 |
| `SNAFUSA80` | SA-80 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafusa80) | SNAFU_Guns_06 |
| `SNAFU_Saint556_Gun` | SAINT VICTOR 5.56 | 5.56x45mm | SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafu_saint556_gun) | SNAFU_Guns_02 |
| `SG550_Gun` | SG550 | 5.56x45mm | FullAuto, SemiAuto, Burst | `SG550_Mag` | [list](#sg550_gun) | Guns_01 |
| `SG552_Gun` | SG552 | 5.56x45mm | FullAuto, SemiAuto, Burst | `SG550_Mag` | [list](#sg552_gun) | Guns_01 |
| `SNAFUTAR21_Black` | TAR-21 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafutar21_black) | SNAFU_Guns_06 |
| `SNAFUTAR21_Green` | TAR-21 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafutar21_black) | SNAFU_Guns_06 |
| `SNAFUTAR21_Tan` | TAR-21 | 5.56x45mm | FullAuto, SemiAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>vanilla: STANAG, CMAG | [list](#snafutar21_black) | SNAFU_Guns_06 |
| `SNAFU_AK103A` | AK-103 Assault Rifle | 7.62x39mm | FullAuto, SemiAuto | `SNAFU_AK103_Mag`<br>vanilla: AKM, AKM Palm, AKM Drum | [list](#snafu_ak103a) | SNAFU_Guns |
| `SNAFU_MK4710Gun` | MK47 10in | 7.62x39mm | FullAuto, SemiAuto | `SNAFU_AK103_Mag`<br>vanilla: AKM, AKM Palm, AKM Drum | [list](#snafu_mk4710gun) | SNAFU_Guns_02 |
| `SNAFU_MK4716Gun` | MK47 16in | 7.62x39mm | FullAuto, SemiAuto | `SNAFU_AK103_Mag`<br>vanilla: AKM, AKM Palm, AKM Drum | [list](#snafu_mk4716gun) | SNAFU_Guns_02 |
| `GCGN_Vepr` | VEPR | 7.62x39mm | SemiAuto | `GCGN_VEPR_10rnd` | [list](#gcgn_vepr) | GCGN_Guns |
| `SNAFU_M70` | Zastava M70 | 7.62x39mm | FullAuto, SemiAuto | `SNAFU_AK103_Mag`<br>vanilla: AKM, AKM Palm, AKM Drum | [list](#snafu_m70) | SNAFU_WW2 |
| `SNAFUSR3_Vikhr` | SR-3 Assault Rifle | 9x39mm / 9x39mm AP | SemiAuto, FullAuto | `Mag_VSS_10Rnd`<br>`Mag_VAL_20Rnd`<br>`SR3_Vikhr_Mag`<br>`SNAFU_SR3Vikhr_Mag` | [list](#snafusr3_vikhr) | SNAFU_Guns_03 |

## Light Machine Guns (LMG)

Belt-fed or high-capacity automatic weapons. 10 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `SNAFU_M60` | M60 | .308 Win / 7.62x51mm | FullAuto | `SNAFU_M60_100rdMag` | [list](#snafu_m60) | SNAFU_Guns_05 |
| `SNAFU_RPK16_Black` | RPK-16 Black | 5.45x39mm | FullAuto, SemiAuto | `SNAFU_RPK16_Black_Mag`<br>`SNAFU_RPK16_Green_Mag`<br>`SNAFU_RPK16_Tan_Mag`<br>vanilla: AK74 | [list](#snafu_rpk16_black) | SNAFU_Guns |
| `SNAFU_RPK16_Green` | RPK-16 Green | 5.45x39mm | FullAuto, SemiAuto | `SNAFU_RPK16_Black_Mag`<br>`SNAFU_RPK16_Green_Mag`<br>`SNAFU_RPK16_Tan_Mag`<br>vanilla: AK74 | [list](#snafu_rpk16_black) | SNAFU_Guns |
| `SNAFU_RPK16_Tan` | RPK-16 Tan | 5.45x39mm | FullAuto, SemiAuto | `SNAFU_RPK16_Black_Mag`<br>`SNAFU_RPK16_Green_Mag`<br>`SNAFU_RPK16_Tan_Mag`<br>vanilla: AK74 | [list](#snafu_rpk16_black) | SNAFU_Guns |
| `GCGN_M249` | M249 | 5.56x45mm | FullAuto | `GCGN_M249_Mag` | [list](#gcgn_m249) | GCGN_Guns |
| `SNAFU_U100` | Ultimax 100 | 5.56x45mm | FullAuto | `SNAFU_PMAG556_Black`<br>`SNAFU_PMAG556_Grey`<br>`SNAFU_PMAG556_OD`<br>`SNAFU_PMAG556_Tan`<br>`SNAFU_BMAG556_Black`<br>`SNAFU_BMAG556_Tan`<br>`SNAFU_CMAG30556_Black`<br>`SNAFU_CMAG30556_Tan`<br>`SNAFU_CMAG40556_Black`<br>`SNAFU_CMAG40556_Tan`<br>`SNAFU_CMAG60556_Black`<br>`SNAFU_CMAG60556_Tan`<br>`GCGN_HK416_Mag`<br>`SNAFU_U100_Mag`<br>vanilla: STANAG, CMAG | - | SNAFU_WW2 |
| `SNAFU_Bren` | Bren | 7.62x39mm | FullAuto | `SNAFU_Bren_30rdMag` | [list](#snafu_bren) | SNAFU_Guns_05 |
| `SNAFURPD` | RPD | 7.62x39mm | FullAuto | `SNAFURPD_100rdMag` | [list](#snafurpd) | SNAFU_Guns_05 |
| `Snafu_PKP_NBlack_GUN` | SNAFU PKP | 7.62x54mmR | FullAuto | `Snafu_PKP_250RND_Mag` | [list](#snafu_pkp_nblack_gun) | SNAFU_Guns_01 |
| `Snafu_PKP_Black_GUN` | SNAFU Rusty PKP | 7.62x54mmR | FullAuto | `Snafu_PKP_250RND_Mag` | [list](#snafu_pkp_nblack_gun) | SNAFU_Guns_01 |

## Submachine Guns (SMG) & PDWs

Pistol-caliber and PDW-caliber automatic weapons. 17 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `SNAFUVECTOR_45acp_GUN` | KRISS Vector 45ACP | .45 ACP | FullAuto, SemiAuto, Burst | `SNAFUVECTOR_45acp_Mag` | [list](#snafuvector_45acp_gun) | SNAFU_Guns_01 |
| `SNAFU_PDW_45ACP` | PDW 45ACP | .45 ACP | FullAuto, SemiAuto | `SNAFU_PDW_45ACP_Mag` | [list](#snafu_pdw_45acp) | SNAFU_Guns |
| `SNAFUThompsonMk2` | Thompson Mk2 | .45 ACP | FullAuto, SemiAuto | `SNAFUThompsonMk2_30rdMag` | [list](#snafuthompsonmk2) | SNAFU_Guns_06 |
| `GCGN_MP7` | MP7 | 4.6x30mm | SemiAuto, FullAuto | `GCGN_MP7_40Rnd` | [list](#gcgn_mp7) | GCGN_Guns |
| `SNAFUP90` | P90 | 5.7x28mm | FullAuto, SemiAuto | `SNAFUP90_50rdMag` | [list](#snafup90) | SNAFU_Guns_06 |
| `SNAFUPPSh` | PPSh-41 | 7.62x25mm Tokarev | FullAuto | `SNAFUPPSh_71rdMag` | [list](#snafuppsh) | SNAFU_Guns_05 |
| `SNAFUPPSKN` | PPSKN-42 | 7.62x39mm | FullAuto, SemiAuto | `SNAFUPPSKN_30rdMag` | [list](#snafuppskn) | SNAFU_Guns_06 |
| `SNAFU_Agram_GUN` | Agram 2000 | 9x19mm | FullAuto, SemiAuto | `SNAFU_Agram_32rnd_Mag` | [list](#snafu_agram_gun) | SNAFU_Guns_01 |
| `SNAFUKH9` | KH9 | 9x19mm | SemiAuto | `SNAFUKH9_30rdMag` | [list](#snafukh9) | SNAFU_Guns_06 |
| `SNAFUVECTOR_9mm_GUN` | KRISS Vector 9mm | 9x19mm | FullAuto, SemiAuto, Burst | `SNAFUVECTOR_9mm_Mag` | [list](#snafuvector_45acp_gun) | SNAFU_Guns_01 |
| `SNAFU_MP9_GUN` | MP9 | 9x19mm | FullAuto, SemiAuto, Burst | `SNAFU_MP9_30rnd_Mag` | [list](#snafu_mp9_gun) | SNAFU_Guns_01 |
| `SNAFU_PDW_9mm` | PDW 9mm | 9x19mm | FullAuto, SemiAuto | `SNAFU_PDW_9mm_Mag` | [list](#snafu_pdw_45acp) | SNAFU_Guns |
| `SNAFU_MPX_GUN` | SIG Sauer MPX | 9x19mm | FullAuto, SemiAuto | `SNAFU_MPX_30rnd_Mag` | [list](#snafu_mpx_gun) | SNAFU_Guns_01 |
| `SNAFUSten` | STEN Mk III | 9x19mm | FullAuto, SemiAuto | `SNAFUSten_32rdMag` | [list](#snafusten) | SNAFU_Guns_05 |
| `Tec9_Gun` | Tec9 | 9x19mm | SemiAuto, Burst | `Tec9_Mag` | [list](#tec9_gun) | Guns_01 |
| `SNAFUUzi` | UZI | 9x19mm | FullAuto, SemiAuto | `SNAFUUzi_32rdMag`<br>`SNAFUUzi_72rdMag` | [list](#snafuuzi) | SNAFU_Guns_06 |
| `GCGN_Vityaz` | Vityaz-SN PP19-01 | 9x19mm | SemiAuto, FullAuto | `GCGN_Vityaz_Mag` | [list](#gcgn_vityaz) | GCGN_Guns |

## Shotguns

12 gauge weapons. 8 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `AA12_Gun` | AA12 | 12 Gauge | SemiAuto, FullAuto | `AA12_Mag` | [list](#aa12_gun) | Guns_01 |
| `GCGN_BenelliM4` | Benelli M2 | 12 Gauge | SemiAuto | internal (loads rounds directly) | [list](#gcgn_benellim4) | GCGN_Guns |
| `SN_Auto_Shotgun` | SN Auto Shotgun | 12 Gauge | Single, FullAuto | `SN_Auto_Shotgun_Mag` | [list](#sn_auto_shotgun) | SNAFU_Guns |
| `SN_M870` | SN M870 | 12 Gauge | Single | internal (loads rounds directly) | [list](#sn_m870) | SNAFU_Guns |
| `Spas12_Gun` | Spas12 | 12 Gauge | SemiAuto | internal (loads rounds directly) | [list](#spas12_gun) | Guns_01 |
| `SNAFU_TP82S` | TP-82 Shotgun | 12 Gauge | Single, Burst | internal (loads rounds directly) | [list](#snafu_tp82s) | SNAFU_Guns |
| `SNAFU_Trenchgun` | Trench Gun | 12 Gauge | Single | internal (loads rounds directly) | - | SNAFU_WW2 |
| `VR80_Gun` | VR80 Shotgun | 12 Gauge | Single, FullAuto | `VR80_Magazine_5rd`<br>`VR80_Magazine_10rd` | [list](#vr80_gun) | Guns_01 |

## Pistols & Revolvers

Sidearms. 11 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `SNAFUChiappaRhino` | Chiappa Rhino | .357 Magnum | Single | internal (loads rounds directly) | [list](#snafuchiapparhino) | SNAFU_Guns_05 |
| `SNAFUAPS` | APS | .380 ACP | SemiAuto, FullAuto | `SNAFUAPS_20rdMag` | [list](#snafuaps) | SNAFU_Guns_06 |
| `SNAFUSWM629` | Smith & Wesson Model 629 | .44 Magnum | Single | internal (loads rounds directly) | [list](#snafuswm629) | SNAFU_Guns_05 |
| `SN_USP` | SN USP | .45 ACP | Single | `SN_USP_Mag` | [list](#sn_usp) | SNAFU_Guns |
| `SNAFUMagnum500` | Model 500 Competitor | .500 S&W Magnum | Single | internal (loads rounds directly) | [list](#snafumagnum500) | SNAFU_Guns_06 |
| `SNAFU_Fort12_GUN` | Fort12 | 9x19mm | SemiAuto | `SNAFU_Fort12_12rnd_Mag` | [list](#snafu_fort12_gun) | SNAFU_Guns_01 |
| `SNAFU_PL14HQP` | Lebedev-PL14 Pistol | 9x19mm | Single | `SNAFU_PL14HQP_Mag` | [list](#snafu_pl14hqp) | SNAFU_Guns |
| `SN_Glock19` | SN Glock19 | 9x19mm | Single | vanilla: Glock | [list](#sn_glock19) | SNAFU_Guns |
| `SN_M9` | SN M9 | 9x19mm | Single | `SN_M9_Mag` | [list](#sn_m9) | SNAFU_Guns |
| `SN_Mp443` | SN Mp443 | 9x19mm | Single | `SN_Mp443_Mag` | [list](#sn_mp443) | SNAFU_Guns |
| `SN_Springfield` | XD Sub-Compact | 9x19mm | Single | `SN_Springfield_Mag` | [list](#sn_springfield) | SNAFU_Guns |

## Test / Duplicate Classes

Spawnable (scope=2) classes that look like test or placeholder entries. Probably keep them out of your types.xml. 3 classes.

| Class name | Name | Caliber | Fire modes | Magazines | Attachments | Mod |
|---|---|---|---|---|---|---|
| `SN_AKM` | $STR_cfgWeapons_AKM0 | 7.62x39mm (inherits vanilla AKM) | inherits AKM | inherits vanilla AKM | [list](#sn_akm) | SNAFU_Guns_01 |
| `SN_AKM_TESTBED` | testing AKM | 7.62x39mm (inherits vanilla AKM) | inherits AKM | inherits vanilla AKM | [list](#sn_akm_testbed) | SNAFU_Guns_01 |
| `SR3_Vikhr_Gun` | REPLACE SR-3 Assault Rifle | 9x39mm / 9x39mm AP | SemiAuto, FullAuto | `Mag_VSS_10Rnd`<br>`Mag_VAL_20Rnd`<br>`SR3_Vikhr_Mag`<br>`SNAFU_SR3Vikhr_Mag` | [list](#sr3_vikhr_gun) | SNAFU_Guns_03 |

## Attachments

199 attachment items, grouped by type. **Slot** is the slot the item goes into; check [Attachment slots](#attachment-slots) for which weapons have that slot.

The optics come in four mount versions of the same scope: normal (`weaponOptics`), **AK** (`weaponOpticsAK`, AK side rail), **Hunting** (`weaponOpticsHunting`, bolt-action and hunting rifles) and **Mosin** (`weaponOpticsMosin`).

### Optics

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `GCGN_M84_Optic` | M84 Scope | `GCGN_M84_Optic` | GCGN_Guns |
| `SNAFU_Aimpoint_ACO` | Aimpoint ACO | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_Aimpoint_M5` | Aimpoint M5 | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_AKAimpoint_ACO` | AK Aimpoint ACO | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKAimpoint_M5` | AK Aimpoint M5 | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKElcan` | AK Elcan 4X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKEOTech_EXPS3` | AK EOTech EXPS3 | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKHuntingOptic` | SNAFU AK DMR Optic 12X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKKahles` | AK Kahles 9X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKLeupold_Mark8` | AK AKLeupold Mark8 10X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKNightforce` | AK Nightforce 12X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKTango6T_Black` | AK Tango6T Black 6X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKTango6T_Snow` | AK Tango6T Snow 6X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKTango6T_Tan` | AK Tango6T Tan 6X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKTango6T_Wood` | AK Tango6T Wood 6X | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKTrijicon` | AK Trijicon | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKTrijicon_Docter` | AK Trijicon Docter | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_AKWalther` | AK Walther | `weaponOpticsAK` | SNAFU_Scopes |
| `SNAFU_Docter` | Docter Reflex | `pistolOptics`, `weaponOpticsCrossbow` | SNAFU_Scopes |
| `SNAFU_Elcan` | Elcan 4X | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_EOTech_EXPS3` | EOTech EXPS3 | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_HAimpoint_ACO` | Hunting Aimpoint ACO | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HAimpoint_M5` | Hunting Aimpoint M5 | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HElcan` | Hunting Elcan 4X | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HEOTech_EXPS3` | Hunting EOTech EXPS3 | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HHuntingOptic` | SNAFU Hunting DMR Optic 12X | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HKahles` | Hunting Kahles 9X | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HLeupold_Mark8` | Hunting Leupold Mark8 10X | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HNightforce` | Hunting Nightforce 12X | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HTrijicon` | Hunting Trijicon | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HTrijicon_Docter` | Hunting Trijicon Docter | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_HuntingOptic` | SNAFU AR DMR Optic 12X | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_HWalther` | Hunting Walther | `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_IRONMODOptic` | Iron Sight | `weaponOptics` | SNAFU_Guns_02 |
| `SNAFU_Kahles` | SNAFU Kahles 9X | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_Kobra` | Kobra | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_Leupold_Mark8` | Leupold Mark8 10X | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_M14Optic` | M14 Optic | `SNAFU_M14Optic` | SNAFU_WW2 |
| `SNAFU_MAimpoint_ACO` | Mosin Aimpoint ACO | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MAimpoint_M5` | Mosin Aimpoint M5 | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MElcan` | Mosin Elcan 4X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MEOTech_EXPS3` | Mosin EOTech EXPS3 | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MHuntingOptic` | SNAFU Mosin DMR Optic 12X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MKahles` | Mosin Kahles 9X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MLeupold_Mark8` | Mosin Leupold Mark8 10X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MNightforce` | Mosin Nightforce 12X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MTango6T_Black` | Mosin Tango6T Black 6X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MTango6T_Snow` | Mosin Tango6T Snow 6X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MTango6T_Tan` | SNAFU MTango6T Tan 6X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MTango6T_Wood` | Mosin Tango6T Wood 6X | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MTrijicon` | Mosin Trijicon | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MTrijicon_Docter` | Mosin Trijicon Docter | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_MWalther` | Mosin Walther | `weaponOpticsMosin` | SNAFU_Scopes |
| `SNAFU_Nightforce` | SNAFU Nightforce 12X | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_Tango6T_Black` | Tango6T Black 6X | `weaponOptics`, `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_Tango6T_Snow` | Tango6T Snow 6X | `weaponOptics`, `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_Tango6T_Tan` | Tango6T Tan 6X | `weaponOptics`, `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_Tango6T_Wood` | Tango6T Wood 6X | `weaponOptics`, `weaponOpticsHunting` | SNAFU_Scopes |
| `SNAFU_Trijicon` | Trijicon | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_Trijicon_Docter` | Trijicon Docter | `weaponOptics` | SNAFU_Scopes |
| `SNAFU_Walther` | Walther MRS | `weaponOptics` | SNAFU_Scopes |

### Suppressors & Muzzle Devices

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `GCGN_M1Garand_FlashHider` | M1Garand Flash Hider | `GCGN_M1Garand_FH` | GCGN_Guns |
| `GCGN_M1Garand_Supp` | M1 Garand Suppressor | `GCGN_M1Garand_Muzzle` | GCGN_Guns |
| `SNAFU_408_Suppressor_T` | 50Bmg & 408 Suppressor Tan | `snafu50bmg` | SNAFU_Guns_02 |
| `SNAFU_50bmg_Suppressor_B` | 50Bmg & 408 Suppressor Black | `snafu50bmg` | SNAFU_Guns_02 |
| `SNAFU_50bmg_Suppressor_M` | 50Bmg & 408 Suppressor BMC | `snafu50bmg` | SNAFU_Guns_02 |
| `SNAFU_50bmg_Suppressor_S` | 50Bmg & 408 Suppressor Snow | `snafu50bmg` | SNAFU_Guns_02 |
| `SNAFU_50bmg_Suppressor_U` | 50Bmg & 408 Suppressor Urban | `snafu50bmg` | SNAFU_Guns_02 |
| `SNAFU_50bmg_Suppressor_W` | 50Bmg & 408 Suppressor Woodland | `snafu50bmg` | SNAFU_Guns_02 |
| `SNAFU_Agram_Suppressor_Black` | Universal Agram SUP BK | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFU_AK19Muzzel` | AK19 Muzzle | `weaponMuzzelSNAFU` | SNAFU_Guns |
| `SNAFU_AK308Muzzel` | AK308 Muzzel | `weaponMuzzelSNAFU` | SNAFU_Guns |
| `SNAFU_HeramuzzelF` | Hera Muzzel | `weaponMuzzelSNAFU` | SNAFU_Guns_02 |
| `SNAFU_LNormalized_Suppressor_Black` | Legion AK Platform Suppressor Black | `weaponMuzzleAK` | SNAFU_Guns_02 |
| `SNAFU_LNormalized_Suppressor_Green` | Legion AK Platform Suppressor Green | `weaponMuzzleAK` | SNAFU_Guns_02 |
| `SNAFU_LStandardized_Suppressor_Black` | Universal Legion BK SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFU_LStandardized_Suppressor_Green` | Universal Legion BK Green | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFU_MK47Muzzel` | MK47 Muzzel | `weaponMuzzelSNAFU` | SNAFU_Guns_02 |
| `SNAFU_MPX_Suppressor_Black` | Universal MPX SUP BK | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFU_MuzzelFF` | Standard Muzzel | `weaponMuzzelSNAFU` | SNAFU_Guns_02 |
| `SNAFU_Normalized_Suppressor_Black` | AK Platform Suppressor Black | `weaponMuzzleAK` | SNAFU_Guns_02 |
| `SNAFU_Normalized_Suppressor_Green` | AK Platform Suppressor Green | `weaponMuzzleAK` | SNAFU_Guns_02 |
| `Snafu_ScarH_SIL_Black` | Universal BK ScarH SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `Snafu_ScarH_SIL_Tan` | Universal Tan ScarH SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFU_SPMOD` | Universal Standard SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFU_SR25_Supp` | Universal SR25 Suppressor | `suppressorImpro`, `sr25Muzzle` | SNAFU_Guns_02 |
| `SNAFU_SR3Vikhr_Supp` | SR3 Suppressor | `SR3S` | SNAFU_Guns_02 |
| `SNAFU_Standardized_Suppressor_Black` | Universal Cordura BK SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFU_Standardized_Suppressor_Green` | Universal Cordura Green SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFUAR15_SPR_SIL` | Universal 300AC SUP | `suppressorImpro`, `snafu300acsupp` | SNAFU_Guns_02 |
| `SNAFUAR15_SPR_SQSIL` | Universal 300AC SQ SUP | `suppressorImpro`, `snafu300acsupp` | SNAFU_Guns_02 |
| `SNAFUGevar_Suppressor_Black` | Universal Mk3 BK SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFUGevar_Suppressor_Green` | Universal Mk3 Green SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFUGevar_Suppressor_Tan` | Universal Mk3 Tan SUP | `suppressorImpro`, `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFUKivaari_338_Supp` | 338 Suppressor | `SNAFU338_Suppressor` | SNAFU_Guns_02 |
| `SNAFUMDAR_Supp_Black` | MDAR SUP BK | `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SNAFUMDAR_Supp_Tan` | MDAR SUP TAN | `weaponMuzzleM4` | SNAFU_Guns_02 |
| `SR3_Vikhr_Supp` | Replace SR3 Suppressor | `SR3S` | SNAFU_Guns_02 |
| `Test_SNAFU_MuzzelF` | Test Version Standard Muzzel | `weaponMuzzelSNAFU` | SNAFU_Guns_02 |

### Handguards

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SNAFU_AK_HG` | AK HG. | `SNAFUWeaponHandguardAK` | SNAFU_Guns |
| `SNAFU_DSAHG1` | DSA HG Standard | `SNAFUDSASA58` | SNAFU_Guns_02 |
| `SNAFU_DSAHG2` | DSA HG Rails | `SNAFUDSASA58` | SNAFU_Guns_02 |
| `SNAFU_GADAR` | ADAR HG | `weaponHGAdarNA` | SNAFU_Guns_02 |
| `SNAFU_HG625` | AR/M4 6.5in QUAD HG | `weaponHGSNAFU10` | SNAFU_Guns_02 |
| `SNAFU_HGGS` | AR/M4 6.5in Poly HG | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_HGMlok` | AR/M4 SRS 15in Mlok HG | `weaponHGSNAFU16` | SNAFU_Guns_02 |
| `SNAFU_HGMlok_Tan` | SRS 15in Mlok HG Tan | `weaponHGSNAFU16` | SNAFU_Guns_02 |
| `SNAFU_LVOAHG` | LVOA Rail HG | `weaponHGSNAFU16NA` | SNAFU_Guns_02 |
| `SNAFU_M249HG` | M249 Black Handguard | `SNAFUM249HG` | GCGN_Guns |
| `SNAFU_M60_Handguard_E3` | M60E3 Handguard | `SNAFUM60Handguard` | SNAFU_Guns_05 |
| `SNAFU_M60_Handguard_E4` | M60E4 Handguard | `SNAFUM60Handguard` | SNAFU_Guns_05 |
| `SNAFU_MCMR07` | AR/M4 7in Mlok HG | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MCMR08` | AR/M4 8in Mlok HG | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MCMR09` | AR/M4 9in Mlok HG | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MCMR10` | AR/M4 10in Mlok HG | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MCMR13` | AR/M4 13in Mlok HG | `weaponHGSNAFU14NA` | SNAFU_Guns_02 |
| `SNAFU_MCMR15` | AR/M4 15in Mlok HG | `weaponHGSNAFU16NA` | SNAFU_Guns_02 |
| `SNAFU_MK10` | AR/M4 10in Rail HG | `weaponHGSNAFU10` | SNAFU_Guns_02 |
| `SNAFU_MK13` | AR/M4 13in Rail HG | `weaponHGSNAFU14` | SNAFU_Guns_02 |
| `SNAFU_MK15` | AR/M4 15in Rail HG | `weaponHGSNAFU16` | SNAFU_Guns_02 |
| `SNAFU_MK47HG` | MK47 HG | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MK7` | AR/M4 7in Rail HG | `weaponHGSNAFU10` | SNAFU_Guns_02 |
| `SNAFU_MK9` | AR/M4 9in Rail HG | `weaponHGSNAFU10` | SNAFU_Guns_02 |
| `SNAFU_MOEFS` | MOE FS Black | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MOEFS_Grey` | MOE FS Tan | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MOEFS_OD` | MOE FS Tan | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MOEFS_Tan` | MOE FS Tan | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MOELS` | MOE LS Black | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MOELS_Grey` | MOE LS Tan | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MOELS_OD` | MOE LS Tan | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_MOELS_Tan` | MOE LS Tan | `weaponHGSNAFU10NA` | SNAFU_Guns_02 |
| `SNAFU_SR3HG` | SR3 HG | `SNAFUSR3HG` | SNAFU_Guns_03 |

### Stocks

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SA58_Stock` | SA58_Stock | `weaponButtstockFal` | Guns_01 |
| `SNAFU_AK19_Stock` | AK 19 Stock. | `weaponButtstockAK` | SNAFU_Guns |
| `SNAFU_AK_AR_Stock` | AK 308 Stock. | `weaponButtstockAK` | SNAFU_Guns |
| `SNAFU_M200S_BK` | M200 Black Stock | `SNAFUM200Stock` | GCGN_Guns |
| `SNAFU_M200S_Green` | M200 Green Stock | `SNAFUM200Stock` | GCGN_Guns |
| `SNAFU_M200S_Snow` | M200 Snow Stock | `SNAFUM200Stock` | GCGN_Guns |
| `SNAFU_M200S_Tan` | M200 Tan Stock | `SNAFUM200Stock` | GCGN_Guns |
| `SNAFU_M249Stock` | M249 Black Stock | `SNAFUM249Stock` | GCGN_Guns |
| `SNAFU_M4SS_Stock` | M4 Standard Stock. | `weaponButtstockM4` | SNAFU_Guns_02 |
| `SNAFU_MK47_Stock` | MK47 Standard Stock. | `weaponButtstockM4` | SNAFU_Guns_02 |
| `SNAFU_MOE_Stock` | M4 MOE Stock. | `weaponButtstockM4` | SNAFU_Guns_02 |
| `SNAFU_PRSGen3_Stock` | M4 PRSGen3 Stock. | `weaponButtstockM4` | SNAFU_Guns_02 |
| `SNAFU_SADAR_Stock` | ADAR Wood Stock. | `weaponButtstockADAR` | SNAFU_Guns_02 |
| `SNAFU_SBA_Stock` | M4 SBA Stock. | `weaponButtstockM4` | SNAFU_Guns_02 |
| `SNAFU_SCQR_Stock` | M4 CQR Stock. | `weaponButtstockCQR` | SNAFU_Guns_02 |
| `SNAFU_UBR_Stock` | M4 UBR Stock. | `weaponButtstockM4` | SNAFU_Guns_02 |
| `SNAFU_WSR3Stock` | SR3 Stock. | `SNAFUWSR3Stock` | SNAFU_Guns_03 |
| `SNAFUDSASA58_Stock` | DSA SA58_Stock | `weaponButtstockFal` | SNAFU_Guns_02 |

### Grips & Foregrips

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SA58_FGrip` | Vertical Grip | `FGRIP` | Guns_01 |
| `SNAFU_AFG_02_Black` | AFG Grip Black | `snafuar15afg` | SNAFU_Guns_02 |
| `SNAFU_AFG_02_OD` | AFG Grip OD | `snafuar15afg` | SNAFU_Guns_02 |
| `SNAFU_AFG_02_Tan` | AFG Grip Tan | `snafuar15afg` | SNAFU_Guns_02 |
| `SNAFU_FGCR_Grip` | CQR Foregrip | `weaponGripCQR` | SNAFU_Guns_02 |
| `SNAFU_FGKAC_Grip` | KAC Foregrip | `weaponGripKAAR` | SNAFU_Guns_02 |
| `SNAFU_GIGripColtA2` | GI Pistol Grip BK | `weaponrgripSNAFU` | SNAFU_Guns_02 |
| `SNAFU_M249Grip` | M249 Black Grip | `SNAFUM249Grip` | GCGN_Guns |
| `SNAFU_PistolGripColtA2` | Standard Pistol Grip | `weaponrgripSNAFU` | SNAFU_Guns_02 |
| `SNAFU_SR3Grip` | SR3 Grip | `SNAFUSR3Grip` | SNAFU_Guns_03 |
| `SNAFU_TACGripColtA2_BK` | TAC Pistol Grip BK | `weaponrgripSNAFU` | SNAFU_Guns_02 |
| `SNAFU_TACGripColtA2_Grey` | TAC Pistol Grip Grey | `weaponrgripSNAFU` | SNAFU_Guns_02 |
| `SNAFU_TACGripColtA2_OD` | TAC Pistol Grip ODK | `weaponrgripSNAFU` | SNAFU_Guns_02 |
| `SNAFU_TACGripColtA2_Tan` | TAC Pistol Grip Tan | `weaponrgripSNAFU` | SNAFU_Guns_02 |
| `SNAFUAR15_AFG` | SNAFU AFG | `snafuar15afg` | SNAFU_Guns_02 |
| `SNAFUMPX_Grip` | MPX Vertical Grip | `snafuar15afg` | SNAFU_Guns_01 |
| `SNAFUScar_AFG_BK` | SNAFU Scar AFG BK | `snafuar15afg` | SNAFU_Guns_02 |
| `SNAFUScar_AFG_Tan` | SNAFU Scar AFG Tan | `snafuar15afg` | SNAFU_Guns_02 |

### Bipods

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SNAFU_AtlasBipod` | SNAFU Atlas Bipod | `snafuweaponBipod` | SNAFU_Guns_02 |
| `SNAFU_Bipod` | SNAFU Old SR25 Bipod | `snafuweaponBipod` | SNAFU_Guns_02 |
| `SNAFU_M200B_BK` | M200 Black Bipod | `SNAFUM200Bipod` | GCGN_Guns |
| `SNAFU_M249Bipod` | M249 Black Bipod | `SNAFUM249Bipod` | GCGN_Guns |
| `SNAFU_ModBipod` | SNAFU Rail Bipod | `snafuweaponBipod` | SNAFU_Guns_02 |
| `SNAFU_NPKPBIPOD` | PKP & PKM Bipod | `PKPBIPOD` | SNAFU_Guns_01 |
| `SNAFU_PKPBIPOD` | PKP & PKM Rusty Bipod | `PKPBIPOD` | SNAFU_Guns_01 |
| `SNAFU_VSSKbipod` | SNAFU VSSK Bipod | `snafuvsskBipod` | SNAFU_Guns_02 |

### Lights & Lasers

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SNAFU_PEQ1_Laser` | PEQ1 Laser | `SNAFUPEQLASER` | SNAFU_Guns_02 |
| `SNAFUUniversalLight` | Picatinny Light | `weaponFlashlight`, `helmetFlashlight` | SNAFU_Guns_02 |

### Shotgun Chokes

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SNAFU_Shotgunchoke_Black` | 10% Choke Black | `SNAFUShotgunchoke` | SNAFU_Guns_02 |
| `SNAFU_Shotgunchoke_Blue` | 20% Choke Blue | `SNAFUShotgunchoke` | SNAFU_Guns_02 |
| `SNAFU_Shotgunchoke_Brown` | 30% Choke Brown | `SNAFUShotgunchoke` | SNAFU_Guns_02 |
| `SNAFU_Shotgunchoke_Green` | 40% Choke Green | `SNAFUShotgunchoke` | SNAFU_Guns_02 |
| `SNAFU_Shotgunchoke_Purple` | 50% Choke Purple | `SNAFUShotgunchoke` | SNAFU_Guns_02 |
| `SNAFU_Shotgunchoke_Red` | 60% Choke Red | `SNAFUShotgunchoke` | SNAFU_Guns_02 |
| `SNAFU_Shotgunchoke_Tur` | 80% Choke Tur | `SNAFUShotgunchoke` | SNAFU_Guns_02 |
| `SNAFU_Shotgunchoke_Yellow` | 100% Choke Yellow | `SNAFUShotgunchoke` | SNAFU_Guns_02 |

### Melee

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SNAFU_Kabar` | Kabar | `Knife` | SNAFU_Guns |

### Revolver Parts (internal)

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `SNAFUChiappaRhino_Cylinder` | - | `RevolverCylinderSNAFUChiappaRhino` | SNAFU_Guns_05 |
| `SNAFUChiappaRhino_Ejector` | - | `RevolverEjectorSNAFUChiappaRhino` | SNAFU_Guns_05 |
| `SNAFUMagnum500_Cylinder` | - | `RevolverCylinderSNAFUMagnum500` | SNAFU_Guns_06 |
| `SNAFUMagnum500_Ejector` | - | `RevolverEjectorSNAFUMagnum500` | SNAFU_Guns_06 |
| `SNAFUSWM629_Cylinder` | - | `RevolverCylinderSNAFUSWM629` | SNAFU_Guns_05 |
| `SNAFUSWM629_Ejector` | - | `RevolverEjectorSNAFUSWM629` | SNAFU_Guns_05 |

### Other

| Class name | Name | Slot | Mod |
|---|---|---|---|
| `GCGN_M1Garand_Bayonet` | M1Garand Byonet | `GCGN_M1Garand_Bayonet` | GCGN_Guns |
| `SNAFU_AK_Mount_Base` | SNAFU AK Mount | - | SNAFU_Scopes |
| `SNAFU_Hunting_Mount_Base` | SNAFU Hunting Mount | - | SNAFU_Scopes |
| `SNAFU_M60_ScopeMount` | M60 Scope Mount | `SNAFUM60ScopeMount` | SNAFU_Guns_05 |
| `SNAFU_Mosin_Mount_Base` | SNAFU Mosin Mount | - | SNAFU_Scopes |
| `SNAFU_SKS_Bayonet` | Zastava M59/66 PAP Byonet | `SNAFU_SKS_Bayonet` | SNAFU_WW2 |

## Attachments per weapon

Which SNAFU attachments (by class name) fit each weapon. Color variants with the same attachments share one entry.
**Vanilla-only slots** take only vanilla DayZ items (for example `weaponWrap` = ghillie wraps). Vanilla slots like `weaponOptics` or `weaponMuzzleM4` also accept vanilla items on top of the SNAFU ones listed.

### Sniper Rifles

#### SNAFU_FRF2

**FR-F2 Sniper Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HWalther`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_M700

**Remington Model 700**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M48

**Zastava M48**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_MAimpoint_ACO`, `SNAFU_MAimpoint_M5`, `SNAFU_MElcan`, `SNAFU_MEOTech_EXPS3`, `SNAFU_MHuntingOptic`, `SNAFU_MKahles`, `SNAFU_MLeupold_Mark8`, `SNAFU_MNightforce`, `SNAFU_MTango6T_Black`, `SNAFU_MTango6T_Snow`, `SNAFU_MTango6T_Tan`, `SNAFU_MTango6T_Wood`, `SNAFU_MTrijicon`, `SNAFU_MTrijicon_Docter`, `SNAFU_MWalther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_AWM_GUN

**AWM 338**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUM98B_Atac_GUN

**Atac M98B** · Variants: `SNAFUM98B_Atac_GUN`, `SNAFUM98B_Digi_GUN`, `SNAFUM98B_Ger_GUN`, `SNAFUM98B_Mc_GUN`, `SNAFUM98B_Snow_GUN`, `SNAFUM98B_Wood_GUN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUT5000_Dkmcc_GUN

**DKMC T5000** · Variants: `SNAFUT5000_Dkmcc_GUN`, `SNAFUT5000_Snow_GUN`, `SNAFUT5000_Wood_GUN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUDVL10M2

**DVL-10 M2**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUM24_GUN

**SNAFU M24A3**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUSRSA2

**SRS A2**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUTac21

**Tac-21**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M300BK

**CheyTac M300 Black** · Variants: `SNAFU_M300BK`, `SNAFU_M300TAN`, `SNAFU_M300Green`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W` |
| Grips & Foregrips | `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_M200

**M200 CheyTac Black** · Variants: `GCGN_M200`, `SNAFU_M200Green`, `SNAFU_M200SNOW`, `GCGN_M200_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W` |
| Stocks | `SNAFU_M200S_BK`, `SNAFU_M200S_Green`, `SNAFU_M200S_Snow`, `SNAFU_M200S_Tan` |
| Bipods | `SNAFU_M200B_BK` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUM96

**M96**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_AS50_GUN

**AS50**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_M82_Barret

**GCGN M82 Barret Black**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUGM6Lynx

**GM6 Lynx**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUAX50_GUN

**SNAFU AX50**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUVSSK

**VSSK**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Bipods | `SNAFU_VSSKbipod` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUAlligator

**Snipex Alligator**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Vanilla-only slots | `weaponWrap` |

### DMR / Marksman Rifles

#### GCGN_M1Garand

**M1Garand**

| Type | Attachments |
|---|---|
| Optics | `GCGN_M84_Optic` |
| Suppressors & Muzzle Devices | `GCGN_M1Garand_FlashHider`, `GCGN_M1Garand_Supp` |
| Other | `GCGN_M1Garand_Bayonet` |
| Vanilla-only slots | `weaponWrap` |

#### SNHK417_Gun

**Heckler & Koch HK417**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_M110_Black

**M110 Semi-Automatic Black** · Variants: `GCGN_M110_Black`, `GCGN_M110_Green`, `GCGN_M110_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUM1A_Black

**M1A** · Variants: `SNAFUM1A_Black`, `SNAFUM1A_Green`, `SNAFUM1A_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_Saint_Gun

**SAINT VICTOR 308**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MK10`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFURSASS_dkmc_GUN

**SNAFU RSASS DKMC** · Variants: `SNAFURSASS_dkmc_GUN`, `SNAFURSASS_od_GUN`, `SNAFURSASS_Wood_GUN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_SR25_Gun

**SNAFU SR25**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M76

**Zastava M76**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUGevar_Black

**Gevar Mk-3 Black** · Variants: `SNAFUGevar_Black`, `SNAFUGevar_Green`, `SNAFUGevar_Grey`, `SNAFUGevar_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUKivaari_Black_GUN

**Kivaari Black** · Variants: `SNAFUKivaari_Black_GUN`, `SNAFUKivaari_Grey_GUN`, `SNAFUKivaari_Snow_GUN`, `SNAFUKivaari_Tan_GUN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_MAR10_Black_GUN

**MAR10 Black**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFUKivaari_338_Supp` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUMarlin1895

**Marlin 1895**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_CALI_GUN

**JJFU Nomad**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUMk12

**Mk 12 Mod 1**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_RDB

**RDB-17**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_SKS

**Zastava M59/66 PAP**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_MAimpoint_ACO`, `SNAFU_MAimpoint_M5`, `SNAFU_MElcan`, `SNAFU_MEOTech_EXPS3`, `SNAFU_MHuntingOptic`, `SNAFU_MKahles`, `SNAFU_MLeupold_Mark8`, `SNAFU_MNightforce`, `SNAFU_MTango6T_Black`, `SNAFU_MTango6T_Snow`, `SNAFU_MTango6T_Tan`, `SNAFU_MTango6T_Wood`, `SNAFU_MTrijicon`, `SNAFU_MTrijicon_Docter`, `SNAFU_MWalther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Other | `SNAFU_SKS_Bayonet` |
| Vanilla-only slots | `weaponWrap` |

### Assault & Battle Rifles (AR)

#### SNAFU_AR15SPRBK

**300AC AR15 BK** · Variants: `SNAFU_AR15SPRBK`, `SNAFUAR15_SPR_Black_GUN`, `SNAFUAR15_SPR_Tan_GUN`, `SNAFU_AR15SPRTAN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_LVOAHG`, `SNAFU_MCMR15`, `SNAFU_MK15` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M4300AC_10_GUN

**300AC Carbine M4-10in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MK10`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M4300AC_14_GUN

**300AC Carbine M4-14in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_GADAR`, `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MCMR13`, `SNAFU_MK10`, `SNAFU_MK13`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap`, `WeaponHandguardM4` |

#### SNAFU_M4300AC_16_GUN

**300AC Carbine M4-16in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_GADAR`, `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_LVOAHG`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MCMR13`, `SNAFU_MCMR15`, `SNAFU_MK10`, `SNAFU_MK13`, `SNAFU_MK15`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M4300AC_14DV_GUN

**300AC Carbine M4-Vanilla**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap`, `WeaponHandguardM4` |

#### SNAFUHoneyBadger_Black

**AAC Honey Badger** · Variants: `SNAFUHoneyBadger_Black`, `SNAFUHoneyBadger_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_KAC_Gun

**KAC PDW**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |

#### SNAFU_AK308

**AK-308 Assault Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_AK_HG` |
| Stocks | `SNAFU_AK19_Stock`, `SNAFU_AK_AR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUDSASA58_Gun

**DSA SA58**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Handguards | `SNAFU_DSAHG1`, `SNAFU_DSAHG2` |
| Stocks | `SA58_Stock`, `SNAFUDSASA58_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_G3A3

**G3A3**

| Type | Attachments |
|---|---|
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M14

**M14 Battle Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_M14Optic` |
| Vanilla-only slots | `weaponWrap` |

#### SNSA58_Gun

**SA58**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Stocks | `SA58_Stock`, `SNAFUDSASA58_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### Snafu_ScarH_Black_GUN

**SNAFU Scar-H BK** · Variants: `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HuntingOptic`, `SNAFU_HWalther`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUASh12

**ASh-12.7**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_AK12A

**AK-12 Assault Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_AK_HG` |
| Stocks | `SNAFU_AK19_Stock`, `SNAFU_AK_AR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_AEK545_Gun

**SNAFU AEK545**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |

#### SNAFU_ADAR_Modular16_GUN

**5.56 ADAR 16in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_GADAR`, `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_LVOAHG`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MCMR13`, `SNAFU_MCMR15`, `SNAFU_MK10`, `SNAFU_MK13`, `SNAFU_MK15`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_AR15_Modular16_GUN

**5.56 AR15 16in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_GADAR`, `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_LVOAHG`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MCMR13`, `SNAFU_MCMR15`, `SNAFU_MK10`, `SNAFU_MK13`, `SNAFU_MK15`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### M4_6933_Gun

**5.56 Carbine M4-10in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MK10`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M4556_Modular10_GUN

**5.56 Carbine M4-10in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MK10`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M4556_Modular14_GUN

**5.56 Carbine M4-14in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_GADAR`, `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MCMR13`, `SNAFU_MK10`, `SNAFU_MK13`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap`, `WeaponHandguardM4` |

#### SNAFU_M4556_Modular16_GUN

**5.56 Carbine M4-16in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_GADAR`, `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_LVOAHG`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MCMR13`, `SNAFU_MCMR15`, `SNAFU_MK10`, `SNAFU_MK13`, `SNAFU_MK15`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_M4A1

**5.56 Carbine M4-Vanilla**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap`, `WeaponHandguardM4` |

#### SNAFU_M4556_Modular14DV_GUN

**5.56 Carbine M4-Vanilla**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap`, `WeaponHandguardM4` |

#### SNAFU_AK19

**AK-19 Assault Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_AK_HG` |
| Stocks | `SNAFU_AK19_Stock`, `SNAFU_AK_AR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUAUG_BK

**AUG A3 Black** · Variants: `SNAFUAUG_BK`, `SNAFUAUG`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_AK5C

**Ak 5C**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_BR18

**BR18**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_CZ805_Gun

**CZ805**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |

#### SNAFUFAMAS

**FAMAS**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SCAR_Gun

**FN SCAR 556**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_HK416

**Heckler & Koch HK416**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### HK416_Gun

**Heckler & Koch HK416**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### IA2_Gun

**IA2**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_LVOA556_GUN

**LVOA 5.56**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_LVOAHG`, `SNAFU_MCMR15`, `SNAFU_MK15` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUMDARCAR_Black

**MDAR Carbine Black** · Variants: `SNAFUMDARCAR_Black`, `SNAFUMDARCAR_Green`, `SNAFUMDARCAR_Tan`, `SNAFUMDARRIF_Black`, `SNAFUMDARRIF_Green`, `SNAFUMDARRIF_Tan`, `SNAFUMDARSBR_Black`, `SNAFUMDARSBR_Green`, `SNAFUMDARSBR_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### MK18_Gun

**MK18**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### ACR_Gun

**Remington ACR**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUSA80

**SA-80**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_Saint556_Gun

**SAINT VICTOR 5.56**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MK10`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SADAR_Stock`, `SNAFU_SBA_Stock`, `SNAFU_SCQR_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SG550_Gun

**SG550**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SG552_Gun

**SG552**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUTAR21_Black

**TAR-21** · Variants: `SNAFUTAR21_Black`, `SNAFUTAR21_Green`, `SNAFUTAR21_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_AK103A

**AK-103 Assault Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_MK4710Gun

**MK47 10in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MK10`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SBA_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_MK4716Gun

**MK47 16in**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MK47Muzzel`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_MuzzelFF`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_HG625`, `SNAFU_HGGS`, `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_LVOAHG`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MCMR13`, `SNAFU_MCMR15`, `SNAFU_MK10`, `SNAFU_MK13`, `SNAFU_MK15`, `SNAFU_MK47HG`, `SNAFU_MK7`, `SNAFU_MK9`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` |
| Stocks | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SBA_Stock`, `SNAFU_UBR_Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Bipods | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_Vepr

**VEPR**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_M70

**Zastava M70**

| Type | Attachments |
|---|---|
| Suppressors & Muzzle Devices | `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUSR3_Vikhr

**SR-3 Assault Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther` |
| Suppressors & Muzzle Devices | `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_MK47Muzzel`, `SNAFU_MuzzelFF`, `SNAFU_SR3Vikhr_Supp`, `SR3_Vikhr_Supp`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_SR3HG` |
| Stocks | `SNAFU_WSR3Stock` |
| Grips & Foregrips | `SNAFU_SR3Grip` |
| Vanilla-only slots | `weaponWrap` |

### Light Machine Guns (LMG)

#### SNAFU_M60

**M60**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Handguards | `SNAFU_M60_Handguard_E3`, `SNAFU_M60_Handguard_E4` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Other | `SNAFU_M60_ScopeMount` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_RPK16_Black

**RPK-16 Black** · Variants: `SNAFU_RPK16_Black`, `SNAFU_RPK16_Green`, `SNAFU_RPK16_Tan`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### GCGN_M249

**M249**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Handguards | `SNAFU_M249HG` |
| Stocks | `SNAFU_M249Stock` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_FGKAC_Grip`, `SNAFU_M249Grip` |
| Bipods | `SNAFU_M249Bipod` |
| Lights & Lasers | `SNAFU_PEQ1_Laser`, `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_Bren

**Bren**

| Type | Attachments |
|---|---|
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFURPD

**RPD**

| Type | Attachments |
|---|---|
| Suppressors & Muzzle Devices | `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green` |
| Vanilla-only slots | `weaponWrap` |

#### Snafu_PKP_NBlack_GUN

**SNAFU PKP** · Variants: `Snafu_PKP_NBlack_GUN`, `Snafu_PKP_Black_GUN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Bipods | `SNAFU_NPKPBIPOD`, `SNAFU_PKPBIPOD` |
| Vanilla-only slots | `weaponWrap` |

### Submachine Guns (SMG) & PDWs

#### SNAFUVECTOR_45acp_GUN

**KRISS Vector 45ACP** · Variants: `SNAFUVECTOR_45acp_GUN`, `SNAFUVECTOR_9mm_GUN`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `pistolMuzzle` |

#### SNAFU_PDW_45ACP

**PDW 45ACP** · Variants: `SNAFU_PDW_45ACP`, `SNAFU_PDW_9mm`

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `pistolMuzzle`, `weaponWrap` |

#### SNAFUThompsonMk2

**Thompson Mk2**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Vanilla-only slots | `weaponWrap`, `pistolMuzzle` |

#### GCGN_MP7

**MP7**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `pistolMuzzle` |

#### SNAFUP90

**P90**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFUPPSh

**PPSh-41**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `weaponWrap` |

#### SNAFUPPSKN

**PPSKN-42**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_Agram_GUN

**Agram 2000**

| Type | Attachments |
|---|---|
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |

#### SNAFUKH9

**KH9**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `pistolMuzzle` |

#### SNAFU_MP9_GUN

**MP9**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `pistolMuzzle` |

#### SNAFU_MPX_GUN

**SIG Sauer MPX**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGCR_Grip`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |

#### SNAFUSten

**STEN Mk III**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `weaponWrap`, `pistolMuzzle` |

#### Tec9_Gun

**Tec9**

| Type | Attachments |
|---|---|
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `pistolMuzzle` |

#### SNAFUUzi

**UZI**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Vanilla-only slots | `weaponWrap`, `pistolMuzzle` |

#### GCGN_Vityaz

**Vityaz-SN PP19-01**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Stocks | `SNAFU_AK19_Stock`, `SNAFU_AK_AR_Stock` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Vanilla-only slots | `WeaponHandguardAK`, `weaponWrap`, `pistolMuzzle` |

### Shotguns

#### AA12_Gun

**AA12**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Grips & Foregrips | `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFU_FGKAC_Grip`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Shotgun Chokes | `SNAFU_Shotgunchoke_Black`, `SNAFU_Shotgunchoke_Blue`, `SNAFU_Shotgunchoke_Brown`, `SNAFU_Shotgunchoke_Green`, `SNAFU_Shotgunchoke_Purple`, `SNAFU_Shotgunchoke_Red`, `SNAFU_Shotgunchoke_Tur`, `SNAFU_Shotgunchoke_Yellow` |

#### GCGN_BenelliM4

**Benelli M2**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Shotgun Chokes | `SNAFU_Shotgunchoke_Black`, `SNAFU_Shotgunchoke_Blue`, `SNAFU_Shotgunchoke_Brown`, `SNAFU_Shotgunchoke_Green`, `SNAFU_Shotgunchoke_Purple`, `SNAFU_Shotgunchoke_Red`, `SNAFU_Shotgunchoke_Tur`, `SNAFU_Shotgunchoke_Yellow` |
| Vanilla-only slots | `weaponWrap` |

#### SN_Auto_Shotgun

**SN Auto Shotgun**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Shotgun Chokes | `SNAFU_Shotgunchoke_Black`, `SNAFU_Shotgunchoke_Blue`, `SNAFU_Shotgunchoke_Brown`, `SNAFU_Shotgunchoke_Green`, `SNAFU_Shotgunchoke_Purple`, `SNAFU_Shotgunchoke_Red`, `SNAFU_Shotgunchoke_Tur`, `SNAFU_Shotgunchoke_Yellow` |
| Vanilla-only slots | `weaponWrap` |

#### SN_M870

**SN M870**

| Type | Attachments |
|---|---|
| Lights & Lasers | `SNAFUUniversalLight` |
| Shotgun Chokes | `SNAFU_Shotgunchoke_Black`, `SNAFU_Shotgunchoke_Blue`, `SNAFU_Shotgunchoke_Brown`, `SNAFU_Shotgunchoke_Green`, `SNAFU_Shotgunchoke_Purple`, `SNAFU_Shotgunchoke_Red`, `SNAFU_Shotgunchoke_Tur`, `SNAFU_Shotgunchoke_Yellow` |
| Vanilla-only slots | `weaponWrap` |

#### Spas12_Gun

**Spas12**

| Type | Attachments |
|---|---|
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Shotgun Chokes | `SNAFU_Shotgunchoke_Black`, `SNAFU_Shotgunchoke_Blue`, `SNAFU_Shotgunchoke_Brown`, `SNAFU_Shotgunchoke_Green`, `SNAFU_Shotgunchoke_Purple`, `SNAFU_Shotgunchoke_Red`, `SNAFU_Shotgunchoke_Tur`, `SNAFU_Shotgunchoke_Yellow` |
| Vanilla-only slots | `weaponWrap` |

#### SNAFU_TP82S

**TP-82 Shotgun**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Docter` |

#### VR80_Gun

**VR80 Shotgun**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` |
| Suppressors & Muzzle Devices | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` |
| Lights & Lasers | `SNAFUUniversalLight` |
| Shotgun Chokes | `SNAFU_Shotgunchoke_Black`, `SNAFU_Shotgunchoke_Blue`, `SNAFU_Shotgunchoke_Brown`, `SNAFU_Shotgunchoke_Green`, `SNAFU_Shotgunchoke_Purple`, `SNAFU_Shotgunchoke_Red`, `SNAFU_Shotgunchoke_Tur`, `SNAFU_Shotgunchoke_Yellow` |
| Vanilla-only slots | `weaponWrap` |

### Pistols & Revolvers

#### SNAFUChiappaRhino

**Chiappa Rhino**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `RevolverCylinderSNAFUChiappaRhino`, `RevolverEjectorSNAFUChiappaRhino` |

#### SNAFUAPS

**APS**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `pistolMuzzle` |

#### SNAFUSWM629

**Smith & Wesson Model 629**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `RevolverCylinderSNAFUSWM629`, `RevolverEjectorSNAFUSWM629` |

#### SN_USP

**SN USP**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Docter` |
| Vanilla-only slots | `pistolMuzzle`, `pistolFlashlight` |

#### SNAFUMagnum500

**Model 500 Competitor**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `RevolverCylinderSNAFUMagnum500`, `RevolverEjectorSNAFUMagnum500` |

#### SNAFU_Fort12_GUN

**Fort12**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Docter` |
| Vanilla-only slots | `pistolMuzzle` |

#### SNAFU_PL14HQP

**Lebedev-PL14 Pistol**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Docter` |
| Vanilla-only slots | `pistolFlashlight`, `pistolMuzzle` |

#### SN_Glock19

**SN Glock19**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Docter` |
| Vanilla-only slots | `pistolFlashlight`, `pistolMuzzle` |

#### SN_M9

**SN M9**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `pistolMuzzle` |

#### SN_Mp443

**SN Mp443**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_Docter` |
| Vanilla-only slots | `pistolFlashlight`, `pistolMuzzle` |

#### SN_Springfield

**XD Sub-Compact**

| Type | Attachments |
|---|---|
| Vanilla-only slots | `pistolFlashlight`, `pistolMuzzle` |

### Test / Duplicate Classes

#### SN_AKM

**$STR_cfgWeapons_AKM0**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_M14Optic` |
| Suppressors & Muzzle Devices | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W`, `SNAFU_SR25_Supp`, `SNAFU_SR3Vikhr_Supp`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SR3_Vikhr_Supp` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Other | `SNAFU_SKS_Bayonet` |
| Vanilla-only slots | `sr25bipod` |

#### SN_AKM_TESTBED

**testing AKM**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_M14Optic` |
| Suppressors & Muzzle Devices | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W`, `SNAFU_SR25_Supp`, `SNAFU_SR3Vikhr_Supp`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SR3_Vikhr_Supp` |
| Grips & Foregrips | `SA58_FGrip`, `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` |
| Other | `SNAFU_SKS_Bayonet` |
| Vanilla-only slots | `sr25bipod` |

#### SR3_Vikhr_Gun

**REPLACE SR-3 Assault Rifle**

| Type | Attachments |
|---|---|
| Optics | `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther` |
| Suppressors & Muzzle Devices | `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_MK47Muzzel`, `SNAFU_MuzzelFF`, `SNAFU_SR3Vikhr_Supp`, `SR3_Vikhr_Supp`, `Test_SNAFU_MuzzelF` |
| Handguards | `SNAFU_SR3HG` |
| Stocks | `SNAFU_WSR3Stock` |
| Grips & Foregrips | `SNAFU_SR3Grip` |
| Vanilla-only slots | `weaponWrap` |

## Attachment slots

Every slot used by the SNAFU weapons, which SNAFU items fit it and how many SNAFU weapons have it.
Vanilla slots (for example `weaponOptics`, `weaponMuzzleM4`, `weaponFlashlight`, `weaponWrap`, `pistolOptics`) also accept vanilla DayZ items.

| Slot | SNAFU items that fit | Weapons with this slot |
|---|---|---|
| `FGRIP` | `SA58_FGrip` | 66 |
| `GCGN_M1Garand_Bayonet` | `GCGN_M1Garand_Bayonet` | 1 |
| `GCGN_M1Garand_FH` | `GCGN_M1Garand_FlashHider` | 1 |
| `GCGN_M1Garand_Muzzle` | `GCGN_M1Garand_Supp` | 1 |
| `GCGN_M84_Optic` | `GCGN_M84_Optic` | 1 |
| `helmetFlashlight` | `SNAFUUniversalLight` | 0 |
| `Knife` | `SNAFU_Kabar` | 0 |
| `pistolFlashlight` | (vanilla items only) | 5 |
| `pistolMuzzle` | (vanilla items only) | 20 |
| `pistolOptics` | `SNAFU_Docter` | 6 |
| `PKPBIPOD` | `SNAFU_NPKPBIPOD`, `SNAFU_PKPBIPOD` | 2 |
| `RevolverCylinderSNAFUChiappaRhino` | `SNAFUChiappaRhino_Cylinder` | 1 |
| `RevolverCylinderSNAFUMagnum500` | `SNAFUMagnum500_Cylinder` | 1 |
| `RevolverCylinderSNAFUSWM629` | `SNAFUSWM629_Cylinder` | 1 |
| `RevolverEjectorSNAFUChiappaRhino` | `SNAFUChiappaRhino_Ejector` | 1 |
| `RevolverEjectorSNAFUMagnum500` | `SNAFUMagnum500_Ejector` | 1 |
| `RevolverEjectorSNAFUSWM629` | `SNAFUSWM629_Ejector` | 1 |
| `snafu300acsupp` | `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL` | 2 |
| `SNAFU338_Suppressor` | `SNAFUKivaari_338_Supp` | 22 |
| `snafu50bmg` | `SNAFU_408_Suppressor_T`, `SNAFU_50bmg_Suppressor_B`, `SNAFU_50bmg_Suppressor_M`, `SNAFU_50bmg_Suppressor_S`, `SNAFU_50bmg_Suppressor_U`, `SNAFU_50bmg_Suppressor_W` | 12 |
| `SNAFU_M14Optic` | `SNAFU_M14Optic` | 3 |
| `SNAFU_SKS_Bayonet` | `SNAFU_SKS_Bayonet` | 3 |
| `snafuar15afg` | `SNAFU_AFG_02_Black`, `SNAFU_AFG_02_OD`, `SNAFU_AFG_02_Tan`, `SNAFUAR15_AFG`, `SNAFUMPX_Grip`, `SNAFUScar_AFG_BK`, `SNAFUScar_AFG_Tan` | 68 |
| `SNAFUDSASA58` | `SNAFU_DSAHG1`, `SNAFU_DSAHG2` | 1 |
| `SNAFUM200Bipod` | `SNAFU_M200B_BK` | 4 |
| `SNAFUM200Stock` | `SNAFU_M200S_BK`, `SNAFU_M200S_Green`, `SNAFU_M200S_Snow`, `SNAFU_M200S_Tan` | 4 |
| `SNAFUM249Bipod` | `SNAFU_M249Bipod` | 1 |
| `SNAFUM249Grip` | `SNAFU_M249Grip` | 1 |
| `SNAFUM249HG` | `SNAFU_M249HG` | 1 |
| `SNAFUM249Stock` | `SNAFU_M249Stock` | 1 |
| `SNAFUM60Handguard` | `SNAFU_M60_Handguard_E3`, `SNAFU_M60_Handguard_E4` | 1 |
| `SNAFUM60ScopeMount` | `SNAFU_M60_ScopeMount` | 1 |
| `SNAFUPEQLASER` | `SNAFU_PEQ1_Laser` | 31 |
| `SNAFUShotgunchoke` | `SNAFU_Shotgunchoke_Black`, `SNAFU_Shotgunchoke_Blue`, `SNAFU_Shotgunchoke_Brown`, `SNAFU_Shotgunchoke_Green`, `SNAFU_Shotgunchoke_Purple`, `SNAFU_Shotgunchoke_Red`, `SNAFU_Shotgunchoke_Tur`, `SNAFU_Shotgunchoke_Yellow` | 6 |
| `SNAFUSR3Grip` | `SNAFU_SR3Grip` | 2 |
| `SNAFUSR3HG` | `SNAFU_SR3HG` | 2 |
| `snafuvsskBipod` | `SNAFU_VSSKbipod` | 1 |
| `snafuweaponBipod` | `SNAFU_AtlasBipod`, `SNAFU_Bipod`, `SNAFU_ModBipod` | 46 |
| `SNAFUWeaponHandguardAK` | `SNAFU_AK_HG` | 3 |
| `SNAFUWSR3Stock` | `SNAFU_WSR3Stock` | 2 |
| `sr25bipod` | (vanilla items only) | 2 |
| `sr25Muzzle` | `SNAFU_SR25_Supp` | 6 |
| `SR3S` | `SNAFU_SR3Vikhr_Supp`, `SR3_Vikhr_Supp` | 4 |
| `suppressorImpro` | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_SR25_Supp`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUAR15_SPR_SIL`, `SNAFUAR15_SPR_SQSIL`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan` | 103 |
| `weaponButtstockADAR` | `SNAFU_SADAR_Stock` | 19 |
| `weaponButtstockAK` | `SNAFU_AK19_Stock`, `SNAFU_AK_AR_Stock` | 4 |
| `weaponButtstockCQR` | `SNAFU_SCQR_Stock` | 19 |
| `weaponButtstockFal` | `SA58_Stock`, `SNAFUDSASA58_Stock` | 2 |
| `weaponButtstockM4` | `SNAFU_M4SS_Stock`, `SNAFU_MK47_Stock`, `SNAFU_MOE_Stock`, `SNAFU_PRSGen3_Stock`, `SNAFU_SBA_Stock`, `SNAFU_UBR_Stock` | 21 |
| `weaponFlashlight` | `SNAFUUniversalLight` | 102 |
| `weaponGripCQR` | `SNAFU_FGCR_Grip` | 43 |
| `weaponGripKAAR` | `SNAFU_FGKAC_Grip` | 65 |
| `WeaponHandguardAK` | (vanilla items only) | 1 |
| `WeaponHandguardM4` | (vanilla items only) | 5 |
| `weaponHGAdarNA` | `SNAFU_GADAR` | 6 |
| `weaponHGSNAFU10` | `SNAFU_HG625`, `SNAFU_MK10`, `SNAFU_MK7`, `SNAFU_MK9` | 13 |
| `weaponHGSNAFU10NA` | `SNAFU_HGGS`, `SNAFU_MCMR07`, `SNAFU_MCMR08`, `SNAFU_MCMR09`, `SNAFU_MCMR10`, `SNAFU_MK47HG`, `SNAFU_MOEFS`, `SNAFU_MOEFS_Grey`, `SNAFU_MOEFS_OD`, `SNAFU_MOEFS_Tan`, `SNAFU_MOELS`, `SNAFU_MOELS_Grey`, `SNAFU_MOELS_OD`, `SNAFU_MOELS_Tan` | 13 |
| `weaponHGSNAFU14` | `SNAFU_MK13` | 7 |
| `weaponHGSNAFU14NA` | `SNAFU_MCMR13` | 7 |
| `weaponHGSNAFU16` | `SNAFU_HGMlok`, `SNAFU_HGMlok_Tan`, `SNAFU_MK15` | 10 |
| `weaponHGSNAFU16NA` | `SNAFU_LVOAHG`, `SNAFU_MCMR15` | 10 |
| `weaponMuzzelSNAFU` | `SNAFU_AK19Muzzel`, `SNAFU_AK308Muzzel`, `SNAFU_HeramuzzelF`, `SNAFU_MK47Muzzel`, `SNAFU_MuzzelFF`, `Test_SNAFU_MuzzelF` | 26 |
| `weaponMuzzleAK` | `SNAFU_LNormalized_Suppressor_Black`, `SNAFU_LNormalized_Suppressor_Green`, `SNAFU_Normalized_Suppressor_Black`, `SNAFU_Normalized_Suppressor_Green` | 13 |
| `weaponMuzzleM4` | `SNAFU_Agram_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Black`, `SNAFU_LStandardized_Suppressor_Green`, `SNAFU_MPX_Suppressor_Black`, `Snafu_ScarH_SIL_Black`, `Snafu_ScarH_SIL_Tan`, `SNAFU_SPMOD`, `SNAFU_Standardized_Suppressor_Black`, `SNAFU_Standardized_Suppressor_Green`, `SNAFUGevar_Suppressor_Black`, `SNAFUGevar_Suppressor_Green`, `SNAFUGevar_Suppressor_Tan`, `SNAFUMDAR_Supp_Black`, `SNAFUMDAR_Supp_Tan` | 71 |
| `weaponOptics` | `SNAFU_Aimpoint_ACO`, `SNAFU_Aimpoint_M5`, `SNAFU_Elcan`, `SNAFU_EOTech_EXPS3`, `SNAFU_HuntingOptic`, `SNAFU_IRONMODOptic`, `SNAFU_Kahles`, `SNAFU_Kobra`, `SNAFU_Leupold_Mark8`, `SNAFU_Nightforce`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood`, `SNAFU_Trijicon`, `SNAFU_Trijicon_Docter`, `SNAFU_Walther` | 138 |
| `weaponOpticsAK` | `SNAFU_AKAimpoint_ACO`, `SNAFU_AKAimpoint_M5`, `SNAFU_AKElcan`, `SNAFU_AKEOTech_EXPS3`, `SNAFU_AKHuntingOptic`, `SNAFU_AKKahles`, `SNAFU_AKLeupold_Mark8`, `SNAFU_AKNightforce`, `SNAFU_AKTango6T_Black`, `SNAFU_AKTango6T_Snow`, `SNAFU_AKTango6T_Tan`, `SNAFU_AKTango6T_Wood`, `SNAFU_AKTrijicon`, `SNAFU_AKTrijicon_Docter`, `SNAFU_AKWalther` | 8 |
| `weaponOpticsCrossbow` | `SNAFU_Docter` | 0 |
| `weaponOpticsHunting` | `SNAFU_HAimpoint_ACO`, `SNAFU_HAimpoint_M5`, `SNAFU_HElcan`, `SNAFU_HEOTech_EXPS3`, `SNAFU_HHuntingOptic`, `SNAFU_HKahles`, `SNAFU_HLeupold_Mark8`, `SNAFU_HNightforce`, `SNAFU_HTrijicon`, `SNAFU_HTrijicon_Docter`, `SNAFU_HWalther`, `SNAFU_Tango6T_Black`, `SNAFU_Tango6T_Snow`, `SNAFU_Tango6T_Tan`, `SNAFU_Tango6T_Wood` | 56 |
| `weaponOpticsMosin` | `SNAFU_MAimpoint_ACO`, `SNAFU_MAimpoint_M5`, `SNAFU_MElcan`, `SNAFU_MEOTech_EXPS3`, `SNAFU_MHuntingOptic`, `SNAFU_MKahles`, `SNAFU_MLeupold_Mark8`, `SNAFU_MNightforce`, `SNAFU_MTango6T_Black`, `SNAFU_MTango6T_Snow`, `SNAFU_MTango6T_Tan`, `SNAFU_MTango6T_Wood`, `SNAFU_MTrijicon`, `SNAFU_MTrijicon_Docter`, `SNAFU_MWalther` | 2 |
| `weaponrgripSNAFU` | `SNAFU_GIGripColtA2`, `SNAFU_PistolGripColtA2`, `SNAFU_TACGripColtA2_BK`, `SNAFU_TACGripColtA2_Grey`, `SNAFU_TACGripColtA2_OD`, `SNAFU_TACGripColtA2_Tan` | 19 |
| `weaponWrap` | (vanilla items only) | 148 |

## Magazines

129 magazines, sorted by caliber.

| Class name | Name | Rounds | Caliber | Used by | Mod |
|---|---|---|---|---|---|
| `SNAFU_M1918A2_Mag` | M1918A2 Magazine | 20 | .30-06 Springfield | `SNAFU_M1918A2` | SNAFU_WW2 |
| `SNAFU_BMAG300_Black` | 300AC 100RND BMag BK | 100 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_BMAG300_Tan` | 300AC 100RND BMag Tan | 100 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_CMAG30300_Black` | 300AC 30RND C-Mag BK | 30 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_CMAG30300_Tan` | 300AC 30RND C-Mag Tan | 30 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_CMAG40300_Black` | 300AC 40RND C-Mag BK | 40 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_CMAG40300_Tan` | 300AC 40RND C-Mag Tan | 40 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_CMAG60300_Black` | 300AC 60RND C-Mag BK | 60 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_CMAG60300_Tan` | 300AC 60RND C-Mag Tan | 60 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFU_KAC_Mag` | KAC Mag | 30 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +3 more | SNAFU_Guns_01 |
| `SNAFUAR15_SPR_100RND_Mag` | AR15 SPR 100RND Mag | 100 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFUAR15_SPR_30RND_Mag` | AR15 SPR 30RND Mag | 30 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFUAR15_SPR_40RND_Mag` | AR15 SPR 40RND Mag | 40 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFUAR15_SPR_60RND_Mag` | AR15 SPR 60RND Mag | 60 | .300 AAC Blackout | `SNAFU_KAC_Gun`, `SNAFU_M4300AC_10_GUN`, `SNAFU_M4300AC_14_GUN`, `SNAFU_M4300AC_16_GUN`, `SNAFU_M4300AC_14DV_GUN`, `SNAFU_AR15SPRBK` +5 more | SNAFU_Guns_02 |
| `SNAFUHoneyBadger_30rdMag_Black` | Honey Badger 30rnd Mag | 30 | .300 AAC Blackout | `SNAFUHoneyBadger_Black`, `SNAFUHoneyBadger_Tan` | SNAFU_Guns_06 |
| `SNAFUHoneyBadger_30rdMag_Tan` | Honey Badger 30rnd Mag | 30 | .300 AAC Blackout | `SNAFUHoneyBadger_Black`, `SNAFUHoneyBadger_Tan` | SNAFU_Guns_06 |
| `GCGN_M110_Mag` | 20 Round M110 Semi-Automatic Magazine | 20 | .308 Win / 7.62x51mm | `GCGN_M110_Black`, `GCGN_M110_Green`, `GCGN_M110_Tan`, `SNHK417_Gun`, `SNAFURSASS_Wood_GUN`, `SNAFURSASS_od_GUN` +2 more | GCGN_Guns |
| `GCGN_M700_Mag` | M700 Mag | 5 | .308 Win / 7.62x51mm | `GCGN_M700` | GCGN_Guns |
| `GCGN_Mag_FAL_50Rnd` | FN FAL 50rnd | 50 | .308 Win / 7.62x51mm | `SNSA58_Gun`, `SNAFUDSASA58_Gun` | GCGN_Guns |
| `Modified_SA58_30RND_BK` | Modified SA58 30Rnd BK | 30 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `Modified_SA58_30RND_DT` | Modified SA58 30Rnd Dirt | 30 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `Modified_SA58_30RND_WBK` | Modified SA58 30Rnd Worn | 30 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `SA58_30RND_BK` | SA58 30Rnd BK | 30 | .308 Win / 7.62x51mm | `SNSA58_Gun`, `SNAFUDSASA58_Gun` | Guns_01 |
| `SA58_30RND_DT` | SA58 30Rnd Dirt | 30 | .308 Win / 7.62x51mm | `SNSA58_Gun`, `SNAFUDSASA58_Gun` | Guns_01 |
| `SA58_30RND_WBK` | SA58 30Rnd Worn | 30 | .308 Win / 7.62x51mm | `SNSA58_Gun`, `SNAFUDSASA58_Gun` | Guns_01 |
| `SA58_DrumMag` | SA58 DrumMag | 50 | .308 Win / 7.62x51mm | `SNSA58_Gun`, `SNAFUDSASA58_Gun` | Guns_01 |
| `SNAFU_AK308_Mag` | AK308 Magazine | 20 | .308 Win / 7.62x51mm | `SNAFU_AK308` | SNAFU_Guns |
| `SNAFU_FRF2_Mag` | SNAFU FRF2 Mag | 10 | .308 Win / 7.62x51mm | `SNAFU_FRF2` | SNAFU_WW2 |
| `SNAFU_G3A3_20rdMag` | 20rd G3A3 Mag | 20 | .308 Win / 7.62x51mm | `SNAFU_G3A3` | SNAFU_Guns_05 |
| `SNAFU_M14_Mag` | M14 Battle Rifle Magazine | 20 | .308 Win / 7.62x51mm | `SNAFUM1A_Black`, `SNAFUM1A_Green`, `SNAFUM1A_Tan`, `SNAFU_M14` | SNAFU_WW2 |
| `SNAFU_M60_100rdMag` | 100rd M60 Ammo Belt | 100 | .308 Win / 7.62x51mm | `SNAFU_M60` | SNAFU_Guns_05 |
| `SNAFU_M76_Mag` | Zastava M76 10 Round Magazine | 10 | .308 Win / 7.62x51mm | `SNAFU_M76` | SNAFU_WW2 |
| `SNAFU_Saint_Mag` | 20 Round Magazine | 20 | .308 Win / 7.62x51mm | `GCGN_M110_Black`, `GCGN_M110_Green`, `GCGN_M110_Tan`, `SNHK417_Gun`, `SNAFURSASS_Wood_GUN`, `SNAFURSASS_od_GUN` +3 more | SNAFU_Guns_02 |
| `SNAFU_ScarH_100RND_Mag_Black` | Snafu Scar-H 100rnd drum mag Black | 100 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `SNAFU_ScarH_100RND_Mag_Tan` | Snafu Scar-H 100rnd drum mag Tan | 100 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `Snafu_ScarH_25RND_Mag_BK` | ScarH 25rnd Mag Black | 25 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `Snafu_ScarH_25RND_Mag_DKMC` | ScarH 25rnd Mag DKMC | 25 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `Snafu_ScarH_25RND_Mag_OD` | ScarH 25rnd Mag OD | 25 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `Snafu_ScarH_25RND_Mag_Snow` | ScarH 25rnd Mag Snow | 25 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `Snafu_ScarH_25RND_Mag_Tan` | ScarH 25rnd Mag Tan | 25 | .308 Win / 7.62x51mm | `Snafu_ScarH_Black_GUN`, `Snafu_ScarH_DKMC_GUN`, `Snafu_ScarH_OD_GUN`, `Snafu_ScarH_Snow_GUN`, `Snafu_ScarH_Tan_GUN` | SNAFU_Guns_03 |
| `SNAFU_SR25_Mag` | 20 Round SR25 Semi-Automatic Magazine | 20 | .308 Win / 7.62x51mm | `GCGN_M110_Black`, `GCGN_M110_Green`, `GCGN_M110_Tan`, `SNHK417_Gun`, `SNAFURSASS_Wood_GUN`, `SNAFURSASS_od_GUN` +2 more | SNAFU_Guns_01 |
| `SNAFUM1A_20rdMag` | M1A Mag | 20 | .308 Win / 7.62x51mm | `SNAFUM1A_Black`, `SNAFUM1A_Green`, `SNAFUM1A_Tan`, `SNAFU_M14` | SNAFU_Guns_06 |
| `SNAFURSASS_Mag` | SNAFU RSASS Mag | 20 | .308 Win / 7.62x51mm | `SNAFURSASS_Wood_GUN`, `SNAFURSASS_od_GUN`, `SNAFURSASS_dkmc_GUN`, `SNAFU_SR25_Gun` | SNAFU_Guns_01 |
| `SNHK417_Mag` | 20 Round HK417 Semi-Automatic Magazine | 20 | .308 Win / 7.62x51mm | `GCGN_M110_Black`, `GCGN_M110_Green`, `GCGN_M110_Tan`, `SNHK417_Gun`, `SNAFURSASS_Wood_GUN`, `SNAFURSASS_od_GUN` +2 more | Guns_01 |
| `SNAFU_AWM_Mag` | AWM Mag | 10 | .338 Lapua Magnum | `SNAFU_AWM_GUN` | SNAFU_Guns_01 |
| `SNAFU_Mar10_15rnd_Mag` | Mar10 15rd Mag | 15 | .338 Lapua Magnum | `SNAFU_MAR10_Black_GUN` | SNAFU_Guns_03 |
| `SNAFUDVL10M2_5rdMag` | DVL-10 M2 5rnd Mag | 5 | .338 Lapua Magnum | `SNAFUDVL10M2` | SNAFU_Guns_06 |
| `SNAFUGevar_10rdMag` | Gevar Mk-3 10rnd Mag | 10 | .338 Lapua Magnum | `SNAFUGevar_Grey`, `SNAFUGevar_Black`, `SNAFUGevar_Green`, `SNAFUGevar_Tan` | SNAFU_Guns_06 |
| `SNAFUKivaari_10rdMag` | Kivaari 10rd Mag | 10 | .338 Lapua Magnum | `SNAFUKivaari_Black_GUN`, `SNAFUKivaari_Tan_GUN`, `SNAFUKivaari_Grey_GUN`, `SNAFUKivaari_Snow_GUN` | SNAFU_Guns_03 |
| `SNAFUKivaari_25rdMag` | Kivaari 25rd Mag | 25 | .338 Lapua Magnum | `SNAFUKivaari_Black_GUN`, `SNAFUKivaari_Tan_GUN`, `SNAFUKivaari_Grey_GUN`, `SNAFUKivaari_Snow_GUN` | SNAFU_Guns_03 |
| `SNAFUM24_Mag` | SNAFU M24A3 Mag | 5 | .338 Lapua Magnum | `SNAFUM24_GUN` | SNAFU_Guns_01 |
| `SNAFUM98B_Mag` | SNAFU M98B Mag | 10 | .338 Lapua Magnum | `SNAFUM98B_Atac_GUN`, `SNAFUM98B_Digi_GUN`, `SNAFUM98B_Ger_GUN`, `SNAFUM98B_Mc_GUN`, `SNAFUM98B_Snow_GUN`, `SNAFUM98B_Wood_GUN` | SNAFU_Guns_01 |
| `SNAFUSRSA2_10rdMag` | SRS A2 10rnd Mag | 10 | .338 Lapua Magnum | `SNAFUSRSA2` | SNAFU_Guns_06 |
| `SNAFUT5000_Mag` | SNAFU T5000 Mag | 5 | .338 Lapua Magnum | `SNAFUT5000_Dkmcc_GUN`, `SNAFUT5000_Snow_GUN`, `SNAFUT5000_Wood_GUN` | SNAFU_Guns_01 |
| `SNAFUTac21_5rdMag` | Tac-21 5rnd Mag | 5 | .338 Lapua Magnum | `SNAFUTac21` | SNAFU_Guns_06 |
| `SNAFUAPS_20rdMag` | APS Mag | 20 | .380 ACP | `SNAFUAPS` | SNAFU_Guns_06 |
| `GCGN_M200_Mag` | CheyTac 7 Round Mag | 7 | .408 CheyTac | `GCGN_M200`, `GCGN_M200_Tan`, `SNAFU_M200Green`, `SNAFU_M200SNOW`, `SNAFU_M300BK`, `SNAFU_M300TAN` +1 more | GCGN_Guns |
| `SNAFU_M300Mag` | M300 Mag | 7 | .408 CheyTac | `GCGN_M200`, `GCGN_M200_Tan`, `SNAFU_M200Green`, `SNAFU_M200SNOW`, `SNAFU_M300BK`, `SNAFU_M300TAN` +1 more | SNAFU_Guns_02 |
| `SNAFUM96_5rdMag` | M96 5rnd Mag | 5 | .408 CheyTac | `SNAFUM96` | SNAFU_Guns_06 |
| `SN_USP_Mag` | USP Mag | 12 | .45 ACP | `SN_USP` | SNAFU_Guns |
| `SNAFU_PDW_45ACP_Mag` | PDW Magazine 45ACP | 26 | .45 ACP | `SNAFU_PDW_45ACP` | SNAFU_Guns |
| `SNAFUThompsonMk2_30rdMag` | Thompson Mk2 30rnd Mag | 30 | .45 ACP | `SNAFUThompsonMk2` | SNAFU_Guns_06 |
| `SNAFUVECTOR_45acp_Mag` | KRISS Vector 45ACP Mag | 37 | .45 ACP | `SNAFUVECTOR_45acp_GUN` | SNAFU_Guns_01 |
| `GCGN_M82_Mag` | Barret M82 Magazine | 10 | .50 BMG | `GCGN_M82_Barret` | GCGN_Guns |
| `SNAFU_AS50_Mag` | AS50 10rnd Mag | 10 | .50 BMG | `SNAFU_AS50_GUN` | SNAFU_Guns_01 |
| `SNAFUAX50_Mag` | SNAFUAX50 Mag | 5 | .50 BMG | `SNAFUAX50_GUN` | SNAFU_Guns_01 |
| `SNAFUGM6Lynx_5rdMag` | GM6 Lynx 5rnd Mag | 5 | .50 BMG | `SNAFUGM6Lynx` | SNAFU_Guns_06 |
| `AA12_Mag` | AA12 Mag | 32 | 12 Gauge | `AA12_Gun` | Guns_01 |
| `SN_Auto_Shotgun_Mag` | SN Auto Shotgun Mag | 20 | 12 Gauge | `SN_Auto_Shotgun` | SNAFU_Guns |
| `VR80_Magazine_10rd` | VR80 Magazine 10rd | 10 | 12 Gauge | `VR80_Gun` | Guns_01 |
| `VR80_Magazine_5rd` | VR80 Magazine 5rd | 5 | 12 Gauge | `VR80_Gun` | Guns_01 |
| `SNAFUASh12_20rdMag` | ASh-12 Mag | 20 | 12.7x55mm | `SNAFUASh12` | SNAFU_Guns_06 |
| `SNAFUVSSK_5rdMag` | Vssk Mag | 5 | 12.7x55mm | `SNAFUVSSK` | SNAFU_Guns_02 |
| `SNAFUAlligator_5rdMag` | Alligator 5rnd Mag | 5 | 14.5x114mm | `SNAFUAlligator` | SNAFU_Guns_06 |
| `GCGN_MP7_40Rnd` | 40 Round MP7 Mag | 40 | 4.6x30mm | `GCGN_MP7` | GCGN_Guns |
| `SNAFU_AK12_Mag` | AK12 Magazine | 30 | 5.45x39mm | `SNAFU_AK12A`, `SNAFU_AEK545_Gun` | SNAFU_Guns |
| `SNAFU_RPK16_Black_Mag` | RPK16 Magazine | 75 | 5.45x39mm | `SNAFU_AK12A`, `SNAFU_RPK16_Black`, `SNAFU_RPK16_Green`, `SNAFU_RPK16_Tan`, `SNAFU_AEK545_Gun` | SNAFU_Guns |
| `SNAFU_RPK16_Green_Mag` | RPK16 Magazine | 75 | 5.45x39mm | `SNAFU_AK12A`, `SNAFU_RPK16_Black`, `SNAFU_RPK16_Green`, `SNAFU_RPK16_Tan`, `SNAFU_AEK545_Gun` | SNAFU_Guns |
| `SNAFU_RPK16_Tan_Mag` | RPK16 Magazine | 75 | 5.45x39mm | `SNAFU_AK12A`, `SNAFU_RPK16_Black`, `SNAFU_RPK16_Green`, `SNAFU_RPK16_Tan`, `SNAFU_AEK545_Gun` | SNAFU_Guns |
| `GCGN_HK416_Mag` | HK416 Drum Mag | 60 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +30 more | GCGN_Guns |
| `GCGN_M249_Mag` | M249 Magazine | 200 | 5.56x45mm | `GCGN_M249` | GCGN_Guns |
| `SG550_Mag` | Sig Sauer 550 30 Round Magazine | 30 | 5.56x45mm | `SG550_Gun`, `SG552_Gun` | Guns_01 |
| `SNAFU_BMAG556_Black` | 5.56 100RND BMag BK | 100 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_BMAG556_Tan` | 5.56 100RND BMag Tan | 100 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_CMAG30556_Black` | 5.56 30RND C-Mag BK | 30 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_CMAG30556_Tan` | 5.56 30RND C-Mag Tan | 30 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_CMAG40556_Black` | 5.56 40RND C-Mag BK | 40 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_CMAG40556_Tan` | 5.56 40RND C-Mag Tan | 40 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_CMAG60556_Black` | 5.56 60RND C-Mag BK | 60 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_CMAG60556_Tan` | 5.56 60RND C-Mag Tan | 60 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_PMAG556_Black` | 5.56 30RND PMag BK | 30 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_PMAG556_Grey` | 5.56 30RND PMag Grey | 30 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_PMAG556_OD` | 5.56 30RND PMag OD | 30 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_PMAG556_Tan` | 5.56 30RND PMag Tan | 30 | 5.56x45mm | `GCGN_HK416`, `ACR_Gun`, `HK416_Gun`, `IA2_Gun`, `MK18_Gun`, `SCAR_Gun` +29 more | SNAFU_Guns_02 |
| `SNAFU_U100_Mag` | U100 Magazine | 100 | 5.56x45mm | `SNAFU_U100` | SNAFU_WW2 |
| `SNAFUAUG_30rdMag` | AUG Mag | 30 | 5.56x45mm | `SNAFUMDARSBR_Black`, `SNAFUMDARSBR_Green`, `SNAFUMDARSBR_Tan`, `SNAFUMDARCAR_Black`, `SNAFUMDARCAR_Green`, `SNAFUMDARCAR_Tan` +5 more | SNAFU_Guns_06 |
| `SNAFUMDAR_30rndMagB` | MDAR 30Rnd Black | 30 | 5.56x45mm | `SNAFUMDARSBR_Black`, `SNAFUMDARSBR_Green`, `SNAFUMDARSBR_Tan`, `SNAFUMDARCAR_Black`, `SNAFUMDARCAR_Green`, `SNAFUMDARCAR_Tan` +3 more | SNAFU_Guns_02 |
| `SNAFUMDAR_30rndMagT` | MDAR 30Rnd Tan | 30 | 5.56x45mm | `SNAFUMDARSBR_Black`, `SNAFUMDARSBR_Green`, `SNAFUMDARSBR_Tan`, `SNAFUMDARCAR_Black`, `SNAFUMDARCAR_Green`, `SNAFUMDARCAR_Tan` +3 more | SNAFU_Guns_02 |
| `SNAFUMDAR_60rndMagB` | MDAR 60Rnd Black | 60 | 5.56x45mm | `SNAFUMDARSBR_Black`, `SNAFUMDARSBR_Green`, `SNAFUMDARSBR_Tan`, `SNAFUMDARCAR_Black`, `SNAFUMDARCAR_Green`, `SNAFUMDARCAR_Tan` +3 more | SNAFU_Guns_02 |
| `SNAFUMDAR_60rndMagT` | MDAR 60Rnd Tan | 60 | 5.56x45mm | `SNAFUMDARSBR_Black`, `SNAFUMDARSBR_Green`, `SNAFUMDARSBR_Tan`, `SNAFUMDARCAR_Black`, `SNAFUMDARCAR_Green`, `SNAFUMDARCAR_Tan` +3 more | SNAFU_Guns_02 |
| `SNAFUMk12_20rdMag` | Mk12 20rnd Mag | 20 | 5.56x45mm | `SNAFUMk12` | SNAFU_Guns_06 |
| `SNAFUP90_50rdMag` | P90 Mag | 50 | 5.7x28mm | `SNAFUP90` | SNAFU_Guns_06 |
| `SNAFUPPSh_71rdMag` | 71rd PPSh-41 Drum Magazine | 71 | 7.62x25mm Tokarev | `SNAFUPPSh` | SNAFU_Guns_05 |
| `GCGN_VEPR_10rnd` | VEPR 10rnd 7.62x39 | 10 | 7.62x39mm | `GCGN_Vepr` | GCGN_Guns |
| `SNAFU_AK103_Mag` | AK103 Magazine | 30 | 7.62x39mm | `SNAFU_AK103A`, `SNAFU_MK4710Gun`, `SNAFU_MK4716Gun`, `SNAFU_M70` | SNAFU_Guns |
| `SNAFU_Bren_30rdMag` | 30rd Bren Mag | 30 | 7.62x39mm | `SNAFU_Bren` | SNAFU_Guns_05 |
| `SNAFU_SKS_10Rnd_Mag` | Zastava M59/66 PAP 10 Round Magazine | 10 | 7.62x39mm | `SNAFU_SKS` | SNAFU_WW2 |
| `SNAFU_SKS_30Rnd_Mag` | Zastava M59/66 PAP 30 Round Magazine | 30 | 7.62x39mm | `SNAFU_SKS` | SNAFU_WW2 |
| `SNAFUPPSKN_30rdMag` | PPSKN-42 30rnd Mag | 30 | 7.62x39mm | `SNAFUPPSKN` | SNAFU_Guns_06 |
| `SNAFURPD_100rdMag` | 100rd RPD Mag | 100 | 7.62x39mm | `SNAFURPD` | SNAFU_Guns_05 |
| `Snafu_PKP_250RND_Mag` | PKP 250rnd Mag | 250 | 7.62x54mmR | `Snafu_PKP_Black_GUN`, `Snafu_PKP_NBlack_GUN` | SNAFU_Guns_01 |
| `GCGN_Vityaz_Mag` | Vityaz-SN 30 Rnd. Mag | 30 | 9x19mm | `GCGN_Vityaz` | GCGN_Guns |
| `SN_M9_Mag` | M9 Mag | 15 | 9x19mm | `SN_M9` | SNAFU_Guns |
| `SN_Mp443_Mag` | Mp443 Mag | 17 | 9x19mm | `SN_Mp443` | SNAFU_Guns |
| `SN_Springfield_Mag` | Springfield Magazine | 10 | 9x19mm | `SN_Springfield` | SNAFU_Guns |
| `SNAFU_Agram_32rnd_Mag` | Agram 32Rnd Mag | 32 | 9x19mm | `SNAFU_Agram_GUN` | SNAFU_Guns_01 |
| `SNAFU_Fort12_12rnd_Mag` | Fort12 12Rnd Mag | 12 | 9x19mm | `SNAFU_Fort12_GUN` | SNAFU_Guns_01 |
| `SNAFU_MP9_30rnd_Mag` | MP9 30Rnd Mag | 30 | 9x19mm | `SNAFU_MP9_GUN` | SNAFU_Guns_01 |
| `SNAFU_MPX_30rnd_Mag` | MPX 30Rnd Mag | 30 | 9x19mm | `SNAFU_MPX_GUN` | SNAFU_Guns_01 |
| `SNAFU_PDW_9mm_Mag` | PDW Magazine 9mm | 33 | 9x19mm | `SNAFU_PDW_9mm` | SNAFU_Guns |
| `SNAFU_PL14HQP_Mag` | Lebedev-PL14 Magazine | 16 | 9x19mm | `SNAFU_PL14HQP` | SNAFU_Guns |
| `SNAFUKH9_30rdMag` | KH9 30rnd Mag | 30 | 9x19mm | `SNAFUKH9` | SNAFU_Guns_06 |
| `SNAFUSten_32rdMag` | 32rd STEN Magazine | 32 | 9x19mm | `SNAFUSten` | SNAFU_Guns_05 |
| `SNAFUUzi_32rdMag` | UZI 32rnd Mag | 32 | 9x19mm | `SNAFUUzi` | SNAFU_Guns_06 |
| `SNAFUUzi_72rdMag` | UZI 72rnd Mag | 72 | 9x19mm | `SNAFUUzi` | SNAFU_Guns_06 |
| `SNAFUVECTOR_9mm_Mag` | KRISS Vector 9mm Mag | 50 | 9x19mm | `SNAFUVECTOR_9mm_GUN` | SNAFU_Guns_01 |
| `Tec9_Mag` | Tec9 Mag | 32 | 9x19mm | `Tec9_Gun` | Guns_01 |
| `SNAFU_SR3Vikhr_Mag` | SR3 Vikhr Mag | 20 | 9x39mm | `SNAFUSR3_Vikhr`, `SR3_Vikhr_Gun` | SNAFU_Guns_03 |
| `SR3_Vikhr_Mag` | REPLACE MAG | 20 | 9x39mm | `SNAFUSR3_Vikhr`, `SR3_Vikhr_Gun` | SNAFU_Guns_03 |

## Ammunition

Ammo boxes and loose rounds added by the mod. Weapons that use vanilla ammo (5.56, .308, 7.62x39, 9mm, 12 gauge, ...) take the normal DayZ `Ammo_*` classes.

| Class name | Name | Caliber | Stack size | Used by (weapons) | Mod |
|---|---|---|---|---|---|
| `GCGN_Ammo_3006` | .30-06 Springfield | .30-06 Springfield | 20 | 2 | SNAFU_Guns_01 |
| `SNAFU_Ammo_300ACC` | 300ACC | .300 AAC Blackout | 40 | 11 | SNAFU_Guns_01 |
| `SNAFU_Ammo_338` | 338 | .338 Lapua Magnum | 40 | 23 | SNAFU_Guns_01 |
| `GCGN_Ammo_408Chey` | .408 CheyTac | .408 CheyTac | 10 | 8 | SNAFU_Guns_01 |
| `SNAFU_Ammo_44` | .44 Magnum | .44 Magnum | 40 | 1 | SNAFU_Guns_01 |
| `SNAFU_Ammo_45_70mm` | 45.70 | .45-70 Government | 40 | 1 | SNAFU_Guns_01 |
| `GCGN_Ammo_50Cal` | .50cal BMG | .50 BMG | 10 | 4 | SNAFU_Guns_01 |
| `SNAFU_Ammo_500_SW` | 500 SW Ammo | .500 S&W Magnum | 40 | 1 | SNAFU_Guns_01 |
| `SNAFU_Ammo_127x55mm` | 127x55mm STs-130PT | 12.7x55mm | 40 | 2 | SNAFU_Guns_01 |
| `SNAFU_Ammo_127x55mmAP` | 12.7×55mm STs-130VPS AP | 12.7x55mm AP | 40 | 1 | SNAFU_Guns_01 |
| `SNAFU_Ammo_145Cal` | 14.5 × 114mm | 14.5x114mm | 20 | 1 | SNAFU_Guns_01 |
| `SNAFU_Ammo_46x30` | 46x30 | 4.6x30mm | 40 | 1 | SNAFU_Guns_01 |
| `SNAFU_MD_Ammo_556x45mm_M855A1` | 5.56 M855A1 | 5.56x45mm M855A1 | 40 | 0 | SNAFU_Guns_01 |
| `SNAFU_Ammo_5_7x28mm` | 5.7x28mm | 5.7x28mm | 40 | 1 | SNAFU_Guns_01 |
| `SNAFU_Ammo_762x25` | 7.62×25mm Tokarev | 7.62x25mm Tokarev | 40 | 1 | SNAFU_Guns_01 |
| `GCGN_Ammo_762x51` | 762x51mm | 7.62x51mm | 40 | 0 | SNAFU_Guns_01 |
| `SNAFU_Ammo_762x51` | 762x51mm | 7.62x51mm | 20 | 0 | SNAFU_WW2 |

### Vanilla ammo used by SNAFU weapons

| Ammo class | Caliber | Weapons |
|---|---|---|
| `Ammo_12gaBeanbag` | 12 Gauge | 7 |
| `Ammo_12gaPellets` | 12 Gauge | 8 |
| `Ammo_12gaRubberSlug` | 12 Gauge | 8 |
| `Ammo_12gaSlug` | 12 Gauge | 8 |
| `Ammo_308Win` | .308 Win / 7.62x51mm | 27 |
| `Ammo_308WinTracer` | .308 Win / 7.62x51mm | 27 |
| `Ammo_357` | .357 Magnum | 1 |
| `Ammo_380` | .380 ACP | 1 |
| `Ammo_45ACP` | .45 ACP | 4 |
| `Ammo_545x39` | 5.45x39mm | 5 |
| `Ammo_545x39Tracer` | 5.45x39mm | 5 |
| `Ammo_556x45` | 5.56x45mm | 43 |
| `Ammo_556x45Tracer` | 5.56x45mm | 43 |
| `Ammo_762x39` | 7.62x39mm | 9 |
| `Ammo_762x39Tracer` | 7.62x39mm | 9 |
| `Ammo_762x54` | 7.62x54mmR | 2 |
| `Ammo_762x54Tracer` | 7.62x54mmR | 2 |
| `Ammo_9x19` | 9x19mm | 16 |
| `Ammo_9x39` | 9x39mm | 2 |
| `Ammo_9x39AP` | 9x39mm AP | 2 |

## Mod folders

| Folder | Weapons | Attachments | Magazines | Ammo |
|---|---|---|---|---|
| `GCGN_Guns` | 16 | 13 | 10 | 0 |
| `Guns_01` | 13 | 2 | 10 | 0 |
| `SNAFU_Guns` | 18 | 6 | 14 | 0 |
| `SNAFU_Guns_01` | 31 | 3 | 16 | 16 |
| `SNAFU_Guns_02` | 35 | 100 | 31 | 0 |
| `SNAFU_Guns_03` | 12 | 3 | 15 | 0 |
| `SNAFU_Guns_05` | 11 | 7 | 6 | 0 |
| `SNAFU_Guns_06` | 32 | 2 | 20 | 0 |
| `SNAFU_Scopes` | 0 | 61 | 0 | 0 |
| `SNAFU_WW2` | 9 | 2 | 7 | 1 |
