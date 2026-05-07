# 2026 — works

[dorawolf.com](https://dorawolf.com) 的「档案」页从这里读图。
**按下面的规则整理文件，整理完 push 上来即可**——网站会自动显示。

---

## 1. 一个项目长什么样

每个项目是仓库根目录下的一个文件夹，文件夹名按这个规则：

```
日期_类型_英文名
```

举例：

```
2026-04-29_thesis_fallout-shelter
2026-04-20_project_rotational-architecture
2026-01-01_coursework_perforation-interference
```

| 段位 | 怎么写 | 举例 |
|------|--------|------|
| **日期** | `年-月-日`，每段两位数 (4 月写 `04`) | `2026-04-29` |
| **类型** | 三选一：`thesis` / `project` / `coursework` | `thesis` |
| **英文名** | 全小写英文 + `-`。**不要拼音首字母**，让人看得懂 | `fallout-shelter` |

**类型怎么选**：
- `thesis` = 长期 (一学期以上) 的深度研究
- `project` = 项目方案 / 合作设计
- `coursework` = 短期研究 / 单次研究 / 习作

---

## 2. 项目里面文件怎么放

```
2026-04-29_thesis_fallout-shelter/
│
├─ images/                ← 想展示在网站上的图
│   ├─ 1.png  2.png  3.png       ← 命名成 1、2、3，1 自动当封面
│   └─ _raw/                      ← 微信截图 / 临时图，存着但不展示
│
├─ models/
│   ├─ rhino/        ← *.3dm
│   ├─ sketchup/     ← *.skp 和 *.skb
│   ├─ grasshopper/  ← *.gh 和 *.ghx
│   └─ cad/          ← *.dwg 和 *.dxf
│
├─ docs/               ← *.pdf  *.docx  *.pptx
├─ data/               ← *.xlsx *.csv
├─ simulation/         ← Ladybug / EnergyPlus / Octopus 输出
└─ archives/           ← *.rar *.zip 大压缩包
```

**重点**：
- 网站封面 = `images/` 根目录下数字最小的图 (例如 `1.png`)
- 微信截图 / 过程草图 → `images/_raw/`，存着但不上网站
- 不需要的桶不用建

---

## 3. 想给作品加中英文标题 / 简介？

不用你写文字——告诉 crabsatellite 你想要的中文标题、英文标题、简介就行，
他在网站那边加上。

---

## 4. 几个小提醒

- **日期定了就别改**——日期是网站链接的一部分，改了原链接会失效。
- **英文名 (slug) 也别轻易改**——同上。要改先 ping crabsatellite。
- **同一天两件同名**？英文名后面加变体 (`-v2` / `-baicao-variant` 之类)。
- **想删 / 重命名一个项目**？先 ping crabsatellite，他在网站端同步更新后你再动。

---

## 5. 流程

你按规则整理 + push → crabsatellite 定期同步 → dorawolf.com 自动更新。

不确定就 ping crabsatellite。
