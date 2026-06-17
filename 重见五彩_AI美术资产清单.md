# 《重见五彩》AI 美术资产清单

> 版本：v0.1  
> 日期：2026-06-16  
> 用途：规划第一版灰盒之后需要逐步生成和接入的 AI 美术资产。  
> 原则：先生成关键流程图，不批量生成无用途图片。

## 1. 美术策略

第一版开发顺序：

1. 先做纯文字灰盒。
2. 灰盒跑通后，加关键背景。
3. 再加成功和失败作品图。
4. 最后加角色立绘和 UI 装饰。

不要一开始生成大量图片。每张图都必须有明确用途。

## 2. 风格方向

建议统一为：

> 半写实 2D，温和克制，工艺记录感，1950 年代研究工坊气质，陶瓷釉面细腻，避免夸张卡通和过度古风。

视觉关键词：

- 醴陵釉下五彩
- 白釉
- 透明釉层
- 试片墙
- 陶瓷研究工坊
- 窑火
- 手写记录
- 展柜光
- 1950 年代
- 克制、真实、温暖

避免：

- 仙侠风
- 过度国潮
- 过度卡通
- 赛博风
- 明显现代奢侈品广告感
- 直接复刻真实文物

## 3. 第一批必需资产

| 编号 | 资产名 | 用途 | 优先级 | 尺寸建议 | 状态 |
| --- | --- | --- | --- | --- | --- |
| A001 | 工坊背景 | 工坊主界面 | P0 | 1920x1080 | 未生成 |
| A002 | 窑炉间背景 | 开窑与烧成界面 | P0 | 1920x1080 | 未生成 |
| A003 | 制作台背景 | 参数选择或制作界面 | P0 | 1920x1080 | 未生成 |
| A004 | 颜色发灰作品图 | 第一次失败结果 | P0 | 1024x1024 | 未生成 |
| A005 | 针孔气泡作品图 | 二烧失败结果 | P0 | 1024x1024 | 未生成 |
| A006 | 黑壳发乌作品图 | 二烧失败结果 | P0 | 1024x1024 | 未生成 |
| A007 | 成功五彩瓶 | 成功结果与展柜 | P0 | 1024x1024 | 未生成 |
| A008 | 展柜背景 | 结尾界面 | P1 | 1920x1080 | 未生成 |

## 4. 第二批资产

| 编号 | 资产名 | 用途 | 优先级 | 尺寸建议 | 状态 |
| --- | --- | --- | --- | --- | --- |
| A009 | 老艺人立绘 | 剧情对白 | P1 | 768x1024 | 未生成 |
| A010 | 青年技术员立绘 | 剧情对白 | P1 | 768x1024 | 未生成 |
| A011 | 残片插图 | 开场与档案 | P1 | 1024x1024 | 未生成 |
| A012 | 试片墙插图 | 长石釉试验 | P1 | 1920x1080 | 未生成 |
| A013 | 档案纸张背景 | 档案界面 | P2 | 1920x1080 | 未生成 |
| A014 | UI 标签与印章元素 | UI 装饰 | P2 | 1024x1024 | 未生成 |

## 5. 单张资产记录模板

每生成一张图，都补充以下记录：

```text
资产编号：
资产名称：
用途：
使用界面：
尺寸：
风格关键词：
生成提示词：
负面提示词：
生成日期：
文件路径：
是否已接入游戏：
是否需要重做：
问题记录：
```

## 6. 提示词模板

### 6.1 工坊背景

用途：工坊主界面。

提示词：

```text
1950s Chinese ceramic research workshop interior, Liling underglaze porcelain restoration studio, wooden tables, ceramic shards, handwritten notes, glaze test tiles, old tools, warm natural light, restrained realistic 2D illustration, semi realistic, calm documentary atmosphere, detailed but not cluttered, no people, game background, 16:9
```

中文辅助描述：

```text
1950 年代中国陶瓷研究工坊，桌上有瓷片、旧谱、试片、手写记录和磨损工具，氛围克制温暖，半写实 2D 游戏背景，无人物。
```

负面提示：

```text
fantasy, cyberpunk, luxury showroom, modern factory, exaggerated cartoon, overdecorated ancient palace, text, watermark, logo
```

### 6.2 窑炉间背景

用途：烧成与开窑界面。

提示词：

```text
traditional ceramic kiln room in 1950s China, kiln door, warm fire light, ceramic workshop tools, ash and brick texture, restrained semi realistic 2D game background, quiet tense atmosphere before opening the kiln, no people, 16:9
```

中文辅助描述：

```text
1950 年代陶瓷窑炉间，窑门、砖墙、工具和温暖火光，开窑前的紧张感，半写实 2D 背景，无人物。
```

负面提示：

```text
lava cave, fantasy forge, sci fi, modern industrial plant, cartoon, text, watermark
```

### 6.3 制作台背景

用途：工艺参数和制作界面。

提示词：

```text
ceramic painting and glazing workbench, porcelain blank, glaze bowls, brushes, color samples, handwritten process notes, Liling underglaze porcelain craft, semi realistic 2D game background, top down slight angle, clean readable composition, no people, 16:9
```

中文辅助描述：

```text
陶瓷彩绘和施釉工作台，有瓷坯、釉碗、毛笔、色样和工艺记录，构图清楚，适合放 UI。
```

负面提示：

```text
messy, fantasy, modern luxury, excessive decoration, text, watermark, logo
```

### 6.4 颜色发灰作品图

用途：第一次试烧结果。

提示词：

```text
underglaze porcelain vase test piece, colors appear gray and muted, old bluish glaze base, visible but not vibrant floral pattern, ceramic defect study image, semi realistic 2D illustration, neutral background, detailed glaze texture
```

中文辅助描述：

```text
釉下五彩试烧瓶，颜色偏灰偏暗，底釉略青，花鸟纹样可见但不明亮，像失败复盘用的作品图。
```

负面提示：

```text
perfect porcelain, bright luxury product, museum masterpiece, text, watermark
```

### 6.5 针孔气泡作品图

用途：二烧失败结果。

提示词：

```text
underglaze porcelain test vase with small pinholes and glaze bubbles, flawed ceramic surface, restoration experiment failure, semi realistic 2D illustration, neutral background, detailed close view of glaze defects
```

中文辅助描述：

```text
釉下五彩试烧瓶，釉面有细小针孔和局部气泡，适合作为失败结果图。
```

负面提示：

```text
perfect surface, broken into pieces, extreme damage, text, watermark
```

### 6.6 黑壳发乌作品图

用途：二烧失败结果。

提示词：

```text
underglaze porcelain test vase with darkened blackened areas under glaze, firing defect, uneven dark marks, restoration experiment failure, semi realistic 2D illustration, neutral background, detailed ceramic glaze texture
```

中文辅助描述：

```text
釉下五彩试烧瓶，局部发乌、黑壳、暗色痕迹，表现烧成失败，但器物整体仍完整。
```

负面提示：

```text
charred wood, fantasy curse, broken shards only, text, watermark
```

### 6.7 成功五彩瓶

用途：成功结果和展柜。

提示词：

```text
fictional Liling underglaze five color porcelain vase, clean white feldspathic glaze, bright but restrained underglaze colors, clear negative white lines, floral and bird inspired pattern, not a replica of real artifact, semi realistic 2D illustration, museum display quality, neutral background
```

中文辅助描述：

```text
虚构醴陵釉下五彩瓶，洁净白釉，釉下色明亮克制，负形留白清晰，花鸟枝叶纹样，不复刻真实文物。
```

负面提示：

```text
copy of famous artifact, over ornate, gold luxury, fantasy, text, watermark, logo
```

## 7. 接入顺序

灰盒跑通后按这个顺序接图：

1. 工坊背景
2. 开窑结果占位图替换为失败/成功作品图
3. 窑炉间背景
4. 展柜背景
5. 角色立绘
6. UI 装饰

每接入一张图，都要重新从头玩一遍，确认：

- 图片加载正常。
- 文字没有看不清。
- 按钮没有被遮挡。
- 成功和失败状态能区分。

## 8. 文件命名建议

```text
assets/images/bg_workshop.png
assets/images/bg_kiln_room.png
assets/images/bg_workbench.png
assets/images/result_gray_color.png
assets/images/result_pinholes.png
assets/images/result_black_shell.png
assets/images/result_success_vase.png
assets/images/bg_exhibition.png
assets/images/character_old_craftsman.png
assets/images/character_young_technician.png
```

## 9. 验收标准

- P0 资产都有明确用途。
- 成功、失败和工坊场景都有图。
- 图片风格统一。
- 没有直接复刻真实文物。
- 接入后不影响界面可读性。

## 10. 当前不建议生成的资产

- 大量 NPC 立绘
- 多套服装
- 大地图
- 复杂动画序列
- 过多瓷器变体
- 商店图标
- 成就图标

这些资产只有在核心切片跑通后才值得投入。
