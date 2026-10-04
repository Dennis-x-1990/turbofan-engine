# 航空发动机 & 活塞发动机 · 交互式 3D 解剖系列

用 Three.js **纯代码程序化建模**的三台发动机,零外部模型资源,单文件实现。
支持 360° 旋转、剖面切视、透视外壳、爆炸视图、气流流线演示、P-V / 布雷顿循环原理图表,
以及每个部件的中文讲解。

## 预览

### 01 · 涡扇发动机 Turbofan —— `main` 分支(本分支)
高涵道比双转子:22 片宽弦风扇 + 增压级 + 高压压气机 + 环形燃烧室 + 双级涡轮 + 大短舱。
透视外壳下的内外涵气流演示 👇

![涡扇发动机透视+气流](docs/preview-turbofan.png)

👉 分支:[`main`](https://github.com/Dennis-x-1990/turbofan-engine/tree/main)(本页)

### 02 · 涡喷发动机 Turbojet —— `turbojet-engine` 分支
带**加力燃烧室**的单转子涡喷:8 级轴流压气机、两级涡轮、V 形火焰稳定器、
16 组可调尾喷口,开加力后喷口张开、尾焰出现激波菱形 👇

![涡喷发动机透视+气流](docs/preview-turbojet.png)

👉 分支:[`turbojet-engine`](https://github.com/Dennis-x-1990/turbofan-engine/tree/turbojet-engine)

### 03 · 单缸汽油发动机 Single-Cylinder —— `single-cylinder` 分支
四冲程 OHC 单缸机:真实曲柄连杆运动学、气门升程曲线、点火提前角、
P-V 示功图与慢放观察 👇

![单缸发动机透视+气流](docs/preview-single-cylinder.png)

👉 分支:[`single-cylinder`](https://github.com/Dennis-x-1990/turbofan-engine/tree/single-cylinder)

### 04 · 直列四缸汽油发动机 Inline-4 —— `four-cylinder-engine` 分支
2.0L DOHC 16V:平面曲轴 0°-180°-180°-0°,发火顺序 1-3-4-2,正时皮带 2:1,
纵剖视角同时看到四套活塞连杆的不同冲程 👇

![四缸发动机纵剖](docs/preview-inline4.png)

👉 分支:[`four-cylinder-engine`](https://github.com/Dennis-x-1990/turbofan-engine/tree/four-cylinder-engine)

### 05 · F-35 战斗机 Lightning II —— `f35` 分支
F-35A 隐身战斗机:锯齿状蒙皮分缝线、DSI 进气道、内置弹舱(4× AIM-120)、
可开启座舱盖与弹射座椅、棕钛锯齿喷口、加力尾焰 👇

![F-35 战斗机](docs/preview-f35.png)

👉 分支:[`f35`](https://github.com/Dennis-x-1990/turbofan-engine/tree/f35)

### 06 · B-2 幽灵 隐身轰炸机 —— `b2` 分支
诺斯罗普·格鲁曼 B-2A:飞翼布局、前缘 33° 后掠、双 W 锯齿尾缘、
背部 S 弯进气、二维窄缝排气、内置旋转弹舱、开裂式阻力方向舵 👇

![B-2 隐身轰炸机](docs/preview-b2.png)

👉 分支:[`b2`](https://github.com/Dennis-x-1990/turbofan-engine/tree/b2)

### 07 · UH-60 黑鹰直升机 —— `uh60` 分支
西科斯基 UH-60L:4 叶全铰接旋翼(弹性轴承,启动时桨叶从下垂到锥角)、
倾斜 20° 无轴承尾桨、全动平尾、ESSS 短翼副油箱、滑动舱门与后货桥 👇

![UH-60 黑鹰直升机](docs/preview-uh60.png)

👉 分支:[`uh60`](https://github.com/Dennis-x-1990/turbofan-engine/tree/uh60)

## 如何运行

每个分支 / 目录里只有一个 `index.html`:

- 直接**双击打开**(需联网加载 Three.js CDN),或
- 任意静态服务器托管后访问(如 `python -m http.server 8000`)。

操作:拖动旋转 · 滚轮缩放 · 右键平移 · 点击部件查看中文讲解;
快捷键:`空格` 起动/停车 · `C` 剖面 · `L` 标注。

## 分支导航

| 分支 | 发动机 | 特色 |
|---|---|---|
| `main` | 涡扇 Turbofan | 大涵道比 · 双转子 · 内外涵气流 |
| `turbojet-engine` | 涡喷 Turbojet | 加力燃烧室 · 可调喷口 · 激波菱形 |
| `single-cylinder` | 单缸机 Single-Cylinder | 曲柄连杆运动学 · 示功图 · 慢放 |
| `four-cylinder-engine` | 四缸机 Inline-4 | 平面曲轴 · 发火顺序 1-3-4-2 · DOHC 16V |
| `f35` | F-35 战斗机 | 隐身机身 · 锯齿蒙皮 · 内置弹舱 · 可开座舱盖 |
| `b2` | B-2 隐身轰炸机 | 飞翼布局 · 双 W 尾缘 · 旋转弹舱 · 开裂方向舵 |
| `uh60` | UH-60 黑鹰直升机 | 全铰接旋翼 · 倾斜尾桨 · ESSS 副油箱 · 后货桥 |
