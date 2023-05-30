# Comparing `tmp/fgo_api_types-2023.5.3.17.28.2.tar.gz` & `tmp/fgo_api_types-2023.5.30.4.51.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.5.3.17.28.2.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.5.30.4.51.47.tar", max compression
```

## Comparing `fgo_api_types-2023.5.3.17.28.2.tar` & `fgo_api_types-2023.5.30.4.51.47.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-05-03 17:27:27.774556 fgo_api_types-2023.5.3.17.28.2/LICENSE
--rw-r--r--   0        0        0      449 2023-05-03 17:27:27.774556 fgo_api_types-2023.5.3.17.28.2/README.md
--rw-r--r--   0        0        0        0 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/common.py
--rw-r--r--   0        0        0    37946 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/enums.py
--rw-r--r--   0        0        0   157289 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    74966 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50178 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-05-03 17:28:02.274895 fgo_api_types-2023.5.3.17.28.2/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-05-03 17:28:02.758900 fgo_api_types-2023.5.3.17.28.2/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.5.3.17.28.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-30 04:51:21.811189 fgo_api_types-2023.5.30.4.51.47/LICENSE
+-rw-r--r--   0        0        0      449 2023-05-30 04:51:21.811189 fgo_api_types-2023.5.30.4.51.47/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   157892 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    75643 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    50619 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18670 2023-05-30 04:51:47.916121 fgo_api_types-2023.5.30.4.51.47/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-05-30 04:51:48.348135 fgo_api_types-2023.5.30.4.51.47/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.5.30.4.51.47/PKG-INFO
```

### Comparing `fgo_api_types-2023.5.3.17.28.2/LICENSE` & `fgo_api_types-2023.5.30.4.51.47/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/basic.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/common.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/enums.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 ### Function Type ###
 
 # The vals attribute of these func types are not buff IDs.
 FUNC_VALS_NOT_BUFF = {
     FuncType.SUB_STATE,
     FuncType.EVENT_DROP_UP,
     FuncType.GAIN_NP_BUFF_INDIVIDUAL_SUM,
+    FuncType.GAIN_NP_INDIVIDUAL_SUM,
 }
 
 
 FUNC_TYPE_NAME_REVERSE: dict[NiceFuncType, int] = {
     v: k for k, v in FUNC_TYPE_NAME.items()
 }
 
@@ -956,14 +957,15 @@
     gutsBlock = "gutsBlock"
     classBeastILost = "classBeastILost"
     holdingHolyGrail = "holdingHolyGrail"
     standardClassServant = "standardClassServant"
     classBeast = "classBeast"
     classBeastVI = "classBeastVI"
     classBeastVIBoss = "classBeastVIBoss"
+    buffBound = "buffBound"
 
 
 TRAIT_NAME: dict[int, Trait] = {
     1: Trait.genderMale,
     2: Trait.genderFemale,
     3: Trait.genderUnknown,
     100: Trait.classSaber,
@@ -1199,14 +1201,15 @@
     3064: Trait.buffSpecialInvincible,
     3065: Trait.buffSkillRankUp,
     3066: Trait.buffSleep,
     3068: Trait.chenGongNp,
     3070: Trait.buffNullifyBuff,
     3076: Trait.cantBeSacrificed,
     3086: Trait.gutsBlock,
+    3087: Trait.buffBound,
     # 6016: No detail
     # 6021: No detail
     # 6022: No detail
     # 10xxx: CCC Kiara buff
     4001: Trait.cardArts,
     4002: Trait.cardBuster,
     4003: Trait.cardQuick,
```

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/gameenums.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/gameenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,16 @@
     DAMAGE_NP_AND_CHECK_INDIVIDUALITY = 55
     ABSORB_NPTURN = 56
     OVERWRITE_DEAD_TYPE = 57
     FORCE_ALL_BUFF_NOACT = 58
     BREAK_GAUGE_UP = 59
     BREAK_GAUGE_DOWN = 60
     MOVE_TO_LAST_SUBMEMBER = 61
+    EXTEND_USER_EQUIP_SKILL = 62
+    UPDATE_ENEMY_ENTRY_MAX_COUNT_EACH_TURN = 63
     EXP_UP = 101
     QP_UP = 102
     DROP_UP = 103
     FRIEND_POINT_UP = 104
     EVENT_DROP_UP = 105
     EVENT_DROP_RATE_UP = 106
     EVENT_POINT_UP = 107
@@ -268,14 +270,16 @@
     damageNpAndCheckIndividuality = "damageNpAndCheckIndividuality"
     absorbNpturn = "absorbNpturn"
     overwriteDeadType = "overwriteDeadType"
     forceAllBuffNoact = "forceAllBuffNoact"
     breakGaugeUp = "breakGaugeUp"
     breakGaugeDown = "breakGaugeDown"
     moveToLastSubmember = "moveToLastSubmember"
+    extendUserEquipSkill = "extendUserEquipSkill"
+    updateEnemyEntryMaxCountEachTurn = "updateEnemyEntryMaxCountEachTurn"
     expUp = "expUp"
     qpUp = "qpUp"
     dropUp = "dropUp"
     friendPointUp = "friendPointUp"
     eventDropUp = "eventDropUp"
     eventDropRateUp = "eventDropRateUp"
     eventPointUp = "eventPointUp"
@@ -368,14 +372,16 @@
     55: NiceFuncType.damageNpAndCheckIndividuality,
     56: NiceFuncType.absorbNpturn,
     57: NiceFuncType.overwriteDeadType,
     58: NiceFuncType.forceAllBuffNoact,
     59: NiceFuncType.breakGaugeUp,
     60: NiceFuncType.breakGaugeDown,
     61: NiceFuncType.moveToLastSubmember,
+    62: NiceFuncType.extendUserEquipSkill,
+    63: NiceFuncType.updateEnemyEntryMaxCountEachTurn,
     101: NiceFuncType.expUp,
     102: NiceFuncType.qpUp,
     103: NiceFuncType.dropUp,
     104: NiceFuncType.friendPointUp,
     105: NiceFuncType.eventDropUp,
     106: NiceFuncType.eventDropRateUp,
     107: NiceFuncType.eventPointUp,
@@ -437,14 +443,15 @@
     PT_SELF_AFTER = 23
     PT_SELF_ANOTHER_LAST = 24
     COMMAND_TYPE_SELF_TREASURE_DEVICE = 25
     FIELD_OTHER = 26
     ENEMY_ONE_NO_TARGET_NO_ACTION = 27
     PT_ONE_HP_LOWEST_VALUE = 28
     PT_ONE_HP_LOWEST_RATE = 29
+    ENEMY_RANGE = 30
 
 
 class NiceFuncTargetType(StrEnum):
     """Function Target Type Enum"""
 
     self_ = "self"
     ptOne = "ptOne"
@@ -472,14 +479,15 @@
     ptSelfAfter = "ptSelfAfter"
     ptSelfAnotherLast = "ptSelfAnotherLast"
     commandTypeSelfTreasureDevice = "commandTypeSelfTreasureDevice"
     fieldOther = "fieldOther"
     enemyOneNoTargetNoAction = "enemyOneNoTargetNoAction"
     ptOneHpLowestValue = "ptOneHpLowestValue"
     ptOneHpLowestRate = "ptOneHpLowestRate"
+    enemyRange = "enemyRange"
 
 
 FUNC_TARGETTYPE_NAME: dict[int, NiceFuncTargetType] = {
     0: NiceFuncTargetType.self_,
     1: NiceFuncTargetType.ptOne,
     2: NiceFuncTargetType.ptAnother,
     3: NiceFuncTargetType.ptAll,
@@ -505,14 +513,15 @@
     23: NiceFuncTargetType.ptSelfAfter,
     24: NiceFuncTargetType.ptSelfAnotherLast,
     25: NiceFuncTargetType.commandTypeSelfTreasureDevice,
     26: NiceFuncTargetType.fieldOther,
     27: NiceFuncTargetType.enemyOneNoTargetNoAction,
     28: NiceFuncTargetType.ptOneHpLowestValue,
     29: NiceFuncTargetType.ptOneHpLowestRate,
+    30: NiceFuncTargetType.enemyRange,
 }
 
 
 class BuffType(IntEnum):
     NONE = 0
     UP_COMMANDATK = 1
     UP_STARWEIGHT = 2
@@ -1562,14 +1571,17 @@
     IgnoreValueUp = 122
     ApplyValueUp = 123
     ActNoDamageBuff = 124
     ActSelectIndex = 125
     CopyTargetBuffType = 126
     NotSkillCopyTargetFuncIds = 127
     NotSkillCopyTargetIndividualities = 128
+    IntervalTurn = 129
+    IntervalCount = 130
+    TargetEnemyRange = 131
 
 
 class ClassRelationOverwriteType(IntEnum):
     OVERWRITE_FORCE = 0
     OVERWRITE_MORE_THAN_TARGET = 1
     OVERWRITE_LESS_THAN_TARGET = 2
 
@@ -3985,14 +3997,15 @@
     USENP_TARGET = -11
     REACTION_TURNSTART = -12
     REACTION_PLAYERACTIONSTART = -13
     REACTION_ENTRY_UNIT = -14
     REACTION_BEFORE_RESURRECTION = -15
     REACTION_BEFORE_DEAD = -16
     SHIFT_SERVANT_AFTER = -17
+    REACTION_BEFORE_MOVE_WAVE = -18
     REACTION_ENEMY_TURN_START_PRIORITY = -401
     REACTION_ENEMY_TURN_END_PRIORITY = -501
 
 
 class NiceAiActNum(StrEnum):
     """AI Act Num Enum"""
 
@@ -4009,14 +4022,15 @@
     usenpTarget = "usenpTarget"
     reactionTurnstart = "reactionTurnstart"
     reactionPlayeractionstart = "reactionPlayeractionstart"
     reactionEntryUnit = "reactionEntryUnit"
     reactionBeforeResurrection = "reactionBeforeResurrection"
     reactionBeforeDead = "reactionBeforeDead"
     shiftServantAfter = "shiftServantAfter"
+    reactionBeforeMoveWave = "reactionBeforeMoveWave"
     reactionEnemyTurnStartPriority = "reactionEnemyTurnStartPriority"
     reactionEnemyTurnEndPriority = "reactionEnemyTurnEndPriority"
     unknown = "unknown"
 
 
 AI_ACT_NUM_NAME: dict[int, NiceAiActNum] = {
     0: NiceAiActNum.nomal,
@@ -4032,14 +4046,15 @@
     -11: NiceAiActNum.usenpTarget,
     -12: NiceAiActNum.reactionTurnstart,
     -13: NiceAiActNum.reactionPlayeractionstart,
     -14: NiceAiActNum.reactionEntryUnit,
     -15: NiceAiActNum.reactionBeforeResurrection,
     -16: NiceAiActNum.reactionBeforeDead,
     -17: NiceAiActNum.shiftServantAfter,
+    -18: NiceAiActNum.reactionBeforeMoveWave,
     -401: NiceAiActNum.reactionEnemyTurnStartPriority,
     -501: NiceAiActNum.reactionEnemyTurnEndPriority,
     -9999: NiceAiActNum.unknown,
 }
 
 
 class MissionType(IntEnum):
```

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/nice.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,17 @@
     IgnoreValueUp: int | None = None
     ApplyValueUp: list[str] | None = None
     ActNoDamageBuff: int | None = None
     ActSelectIndex: int | None = None
     CopyTargetBuffType: list[int] | None = None
     NotSkillCopyTargetFuncIds: list[int] | None = None
     NotSkillCopyTargetIndividualities: list[int] | None = None
+    IntervalTurn: int | None = None
+    IntervalCount: int | None = None
+    TargetEnemyRange: list[int] | None = None
     # Extra dataval from SkillLvEntty.DIC_KEY_APPLY_SUPPORT_SVT
     ApplySupportSvt: Optional[int] = None
     # These are not DataVals but guesses from SkillLvEntity and EventDropUpValInfo
     Individuality: Optional[int] = None
     EventId: Optional[int] = None
     AddCount: Optional[int] = None
     RateCount: Optional[int] = None
@@ -605,14 +608,25 @@
     unmodifiedDetail: str
     functions: list[NiceFunction] = Field(
         ...,
         description="Since each skill level has their own group overwrite, the svals field only contains data for 1 level.",
     )
 
 
+class NiceSvtSkillRelease(BaseModelORJson):
+    # svtId: int
+    # num: int
+    # priority: int
+    idx: int
+    condType: NiceCondType
+    condTargetId: int
+    condNum: int
+    condGroup: int
+
+
 class NiceSkill(BaseModelORJson):
     id: int
     num: int = -1
     name: str
     originalName: str
     ruby: str
     detail: Optional[str] = None
@@ -626,14 +640,15 @@
     condLimitCount: int = -1
     icon: Optional[HttpUrl] = None
     coolDown: list[int]
     actIndividuality: list[NiceTrait]
     script: NiceSkillScript
     extraPassive: list[ExtraPassive]
     skillAdd: list[NiceSkillAdd]
+    releaseConditions: list[NiceSvtSkillRelease] = []
     aiIds: Optional[dict[AiType, list[int]]] = None
     groupOverwrites: list[NiceSkillGroupOverwrite] | None = None
     functions: list[NiceFunction]
 
 
 class NpGain(BaseModel):
     buster: list[int]
@@ -654,14 +669,15 @@
     imageIndex: int
     condQuestId: int
     condQuestPhase: int
     condLv: int = 0
     condFriendshipRank: int = 0
     motion: int
     card: NiceCardType
+    releaseConditions: list[NiceSvtSkillRelease] = []
 
 
 class NiceTd(BaseModelORJson):
     id: int
     num: int
     card: NiceCardType
     name: str
@@ -675,14 +691,15 @@
     unmodifiedDetail: Optional[str] = None
     npGain: NpGain
     npDistribution: list[int]
     strengthStatus: int
     priority: int
     condQuestId: int
     condQuestPhase: int
+    releaseConditions: list[NiceSvtSkillRelease] = []
     individuality: list[NiceTrait]
     npSvts: list[NiceTdSvt]
     script: NiceSkillScript
     functions: list[NiceFunction]
 
 
 class ExtraMCAssets(BaseModel):
@@ -1779,19 +1796,26 @@
 class NiceEventBulletinBoardRelease(BaseModelORJson):
     condGroup: int
     condType: NiceCondType
     condTargetId: int
     condNum: int
 
 
+class NiceEventBulletinBoardScript(BaseModelORJson):
+    icon: HttpUrl | None = None
+    name: str | None = None
+
+
 class NiceEventBulletinBoard(BaseModelORJson):
     bulletinBoardId: int
     message: str
     probability: int | None = None
+    dispOrder: int | None = None
     releaseConditions: list[NiceEventBulletinBoardRelease]
+    script: list[NiceEventBulletinBoardScript] = []
 
 
 class NiceEventRecipeGift(BaseModelORJson):
     idx: int
     displayOrder: int
     topIconId: int
     gifts: list[NiceGift]
```

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/raw.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,14 +115,29 @@
     condQuestPhase: int  # 0,
     condLv: int = 0  # 0,
     condLimitCount: int  # 0,
     eventId: int  # 0,
     flag: int  # 0
 
 
+class MstSvtSkillRelease(BaseModelORJson):
+    svtId: int
+    num: int
+    priority: int
+    idx: int
+    condType: int
+    condTargetId: int
+    condNum: int
+    condGroup: int
+
+
+class MstSvtTreasureDeviceRelease(MstSvtSkillRelease):
+    ...
+
+
 class MstSvtPassiveSkill(BaseModelORJson):
     svtId: int
     num: int
     priority: int
     skillId: int
     condQuestId: int
     condQuestPhase: int
@@ -193,14 +208,15 @@
 
 
 class SkillEntityNoReverse(BaseModelORJson):
     mstSkill: MstSkill
     mstSkillDetail: list[MstSkillDetail]
     mstSvtSkill: list[MstSvtSkill]
     mstSkillAdd: list[MstSkillAdd]
+    mstSvtSkillRelease: list[MstSvtSkillRelease]
     mstCommonRelease: list[MstCommonRelease]
     mstSkillLv: list[MstSkillLv]
     mstSkillGroup: list[MstSkillGroup]
     mstSkillGroupOverwrite: list[MstSkillGroupOverwrite]
     aiIds: Optional[dict[AiType, list[int]]] = None
 
 
@@ -302,14 +318,15 @@
 
 
 class TdEntityNoReverse(BaseModelORJson):
     mstTreasureDevice: MstTreasureDevice
     mstTreasureDeviceDetail: list[MstTreasureDeviceDetail]
     mstSvtTreasureDevice: list[MstSvtTreasureDevice]
     mstTreasureDeviceLv: list[MstTreasureDeviceLv]
+    mstSvtTreasureDeviceRelease: list[MstSvtTreasureDeviceRelease]
 
 
 class MstSvt(BaseModelORJson):
     relateQuestIds: list[int]  # [91500701, 94004103, 94014414],
     individuality: list[int]  # [5000, 500800],
     classPassive: list[int]  # [83350, 80350, 320650],
     expandedClassPassive: list[SkillEntityNoReverse] = []
@@ -1256,14 +1273,16 @@
 
 
 class MstEventBulletinBoard(BaseModelORJson):
     id: int
     eventId: int
     message: str
     probability: int | None = None
+    dispOrder: int | None = None
+    script: list[dict[str, Any]] | None = None
 
 
 class MstEventBulletinBoardRelease(BaseModelORJson):
     bulletinBoardId: int
     condType: int
     condTargetId: int
     condNum: int
```

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/rayshift.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.3.17.28.2/fgo_api_types/search.py` & `fgo_api_types-2023.5.30.4.51.47/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.5.3.17.28.2/pyproject.toml` & `fgo_api_types-2023.5.30.4.51.47/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.05.03.17.28.02"
+version = "2023.05.30.04.51.47"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.5.3.17.28.2/PKG-INFO` & `fgo_api_types-2023.5.30.4.51.47/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.5.3.17.28.2
+Version: 2023.5.30.4.51.47
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

