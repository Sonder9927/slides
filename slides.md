---
theme: default
class: text-center
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
transition: slide-left
title: 地球深部过程
---

# 地球深部过程
## Science & Nature 文献汇报

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-4 py-2 rounded cursor-pointer bg-white bg-opacity-10 hover:bg-opacity-20 transition">
    开始汇报 <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 text-sm opacity-50">
  汇报人：Sonder | 日期：2026.4.22
</div>

<!--
开场白：今天我们将解析两篇发表在Science和Nature上的文章，分别探讨黄石火山系统的构造起源和马里亚纳俯冲带的水循环。
-->

---
layout: center
class: text-center
---

# 汇报大纲

<div class="grid grid-cols-2 gap-8 pt-8">
<div>

## 🔥 第一篇
# *Science* (2026)
### 黄石火山系统的构造起源
**核心问题**：超级火山的岩浆从何而来？

</div>
<div>

## 🌊 第二篇
# *Nature* (2018)
### 马里亚纳俯冲带的水输入
**核心问题**：海水如何进入地球深部？

</div>
</div>

<div class="mt-12 text-xl opacity-80">
"从火山到海沟，探索地球内部的物质循环"
</div>

<!--
今天的汇报分为两大模块。第一篇是关于黄石超级火山，挑战了传统的地幔柱假说；第二篇是关于马里亚纳海沟，重新估算了俯冲带的水通量。两个问题都关乎地球深部的物质和能量交换。
-->

---
layout: center
class: text-center
---

# 文章一
# 黄石火山系统的构造起源
## *Science* (2026)

<div class="text-2xl mt-8 opacity-80">
Zebin Cao, Lijun Liu, et al.
</div>
<div class="text-xl mt-4 opacity-60">
"Tectonic origin of Yellowstone's translithospheric magma plumbing system"
</div>

<!--
进入第一篇。这篇文章的核心贡献是提出了"跨岩石圈岩浆通道系统"（TLMPS）的概念，认为黄石的岩浆系统主要由构造力控制，而非深部地幔柱。
-->

---
layout: center
---

## 双峰式火山活动与岩浆系统示意
Bimodal volcanism and magma system


火山喷发产物中，同时大量出现基性岩（玄武质）和酸性岩（流纹质/花岗质），但中间成分（安山岩、英安岩）明显较少，形成“双峰分布”

<div class="grid grid-cols-2 gap-10 items-center mt-6">

<!-- 左图：分布 -->
<div class="flex flex-col items-center">

<svg viewBox="0 0 320 240" width="300">

  <!-- 背景 -->
  <rect x="0" y="0" width="320" height="240" fill="white"/>

  <!-- 坐标轴 -->
  <line x1="50" y1="200" x2="300" y2="200" stroke="#333" stroke-width="0.8"/>
  <line x1="50" y1="40" x2="50" y2="200" stroke="#333" stroke-width="0.8"/>

  <!-- 曲线（灰度主导） -->
  <path d="M50 200 Q120 100 170 200"
        fill="none" stroke="#666" stroke-width="1.2"/>
  <path d="M170 200 Q250 90 300 200"
        fill="none" stroke="#666" stroke-width="1.2"/>

  <!-- 强调峰 -->
  <circle cx="120" cy="105" r="3" fill="#b2182b"/>
  <circle cx="250" cy="95" r="3" fill="#2166ac"/>

  <!-- 标签 -->
  <text x="95" y="95" font-size="3" fill="#b2182b">Basalt</text>
  <text x="235" y="85" font-size="3" fill="#2166ac">Rhyolite</text>
  <text x="160" y="185" font-size="3" fill="#444">Composition gap</text>

  <!-- 坐标说明 -->
  <text x="230" y="215" font-size="3" fill="#333">SiO₂ (wt%)</text>
  <text x="20" y="50" font-size="3" fill="#333">Frequency</text>

</svg>

<div style="font-size:11px; margin-top:6px; color:#444">
(a) Bimodal distribution of volcanic compositions
</div>

</div>

<!-- 右图：剖面 -->
<div class="flex flex-col items-center">

<svg viewBox="0 0 320 240" width="300">

  <!-- 背景 -->
  <rect x="0" y="0" width="320" height="240" fill="white"/>

  <!-- 地表 -->
  <line x1="0" y1="60" x2="320" y2="60" stroke="#333" stroke-width="0.8"/>

  <!-- 火山 -->
  <polygon points="150,60 170,60 160,35" fill="#555"/>

  <!-- Moho -->
  <line x1="0" y1="140" x2="320" y2="140" stroke="#999" stroke-dasharray="2,2"/>
  <text x="10" y="135" font-size="3" fill="#666">Moho</text>

  <!-- 深部基性 -->
  <ellipse cx="160" cy="190" rx="65" ry="25"
           fill="#d9d9d9" stroke="#666" stroke-width="0.8"/>
  <text x="110" y="195" font-size="3" fill="#333">Basaltic source</text>

  <!-- 浅部酸性 -->
  <ellipse cx="160" cy="110" rx="55" ry="20"
           fill="#f0f0f0" stroke="#666" stroke-width="0.8"/>
  <text x="105" y="112" font-size="3" fill="#333">Rhyolitic mush</text>

  <!-- 通道 -->
  <line x1="160" y1="165" x2="160" y2="125"
        stroke="#444" stroke-width="1"/>
  <line x1="160" y1="125" x2="160" y2="65"
        stroke="#444" stroke-width="1"/>

  <!-- 箭头 -->
  <polygon points="160,65 155,75 165,75" fill="#444"/>

  <!-- 深度标注 -->
  <line x1="300" y1="60" x2="300" y2="200" stroke="#999"/>
  <text x="305" y="65" font-size="3">0 km</text>
  <text x="305" y="140" font-size="3">~30 km</text>
  <text x="305" y="200" font-size="3">~80 km</text>

</svg>

<div style="font-size:11px; margin-top:6px; color:#444">
(b) Conceptual magma plumbing system
</div>

</div>

</div>

双峰性可以看作岩浆系统结构分离的直接表现。

---
layout: two-cols
---

::left::

# 黄石：超级火山的威胁

<div class="mt-4">

- **过去200万年**：3次超级喷发
  - 2.1 Ma: Huckleberry Ridge
  - 0.63 Ma: Lava Creek（最近一次）
  
- **双峰式火山作用**：
  - 黄石：间歇性流纹质（酸性）
  - 蛇河平原：连续性玄武质（基性）

</div>

::right::

![Fig.1A](/images/literatures/science.ady2027-f1.jpg)

*Fig.1A: 黄石地区火山分布与地形。红色=基性火山，白色=酸性火山。注意黄石与ESRP之间的"火山空白区"。*

<!--
黄石是世界上最大的活火山系统之一。过去200万年发生了3次超级喷发，最近一次是63万年前。一个有趣的现象是：黄石以酸性火山为主，而西侧的蛇河平原以基性火山为主，中间存在一个"火山空白区"。这种双峰分布一直是个谜。
-->

---
layout: two-cols
---

::left::

# 传统观点 vs 新发现

<div class="mt-4">

**传统观点：地幔柱模型**
- 深部地幔柱垂直上升
- 岩浆垂直运移
- 与地震观测的横向偏移矛盾

**新发现：倾斜跨岩石圈岩浆通道系统 (TLMPS)**
- 地震层析成像显示**不连续、横向偏移**的异常体
- 浅部近垂直 → 中部向西南倾斜 → 深部近水平
- 熔体富集区位于上覆软流圈顶部

</div>

::right::

![Fig.1B-F](/images/literatures/science.ady2027-f1.jpg)

*Fig.1B-F: 不同深度的地震波速异常。90km深度（B）低速异常在黄石下方；50km（C）和70km（D）异常体向西南偏移；35km（E）和8km（F）回到黄石下方。*

<!--
传统观点认为黄石下方有一个深部地幔柱，像烟囱一样垂直输送岩浆。但地震成像发现，深部的低速异常体并不在黄石正下方，而是向西南偏移了！这说明岩浆路径是倾斜的，不是垂直的。这就引出了TLMPS的概念。
-->

---
layout: center
class: text-center
---


<div class="text-4xl font-bold mt-8 text-orange-400">
Translithospheric Magma Plumbing System
</div>
<div class="text-2xl mt-4">
跨岩石圈岩浆通道系统
</div>

<div class="grid grid-cols-3 gap-4 mt-12 text-lg">
<div class="p-4 bg-gray-300 rounded">

### 上地壳
**近垂直**
流纹质岩浆房
~10 km

</div>
<div class="p-4 bg-gray-300 rounded">

### 中-下地壳
**向西南倾斜**
玄武质岩浆糊状物
~35 km

</div>
<div class="p-4 bg-gray-300 rounded">

### 岩石圈地幔
**近水平**
软流圈熔体来源
~40-90 km

</div>
</div>

<div class="mt-8 text-xl opacity-80">
💡 <span class="text-yellow-400">通俗理解</span>：岩浆不是直上直下，而是走"斜坡通道"，从西南侧"流"进黄石
</div>

<!--
TLMPS是这个研究的核心概念。它描述了岩浆从软流圈进入岩石圈，最终到达地壳的完整路径。关键是这个路径是倾斜的，不是垂直的。就像水不是垂直向上喷，而是沿着管道流动一样。
-->

---
layout: two-cols
---

::left::

## 三维地球动力学模型

<div class="mt-4">

**模型构建**
- 软流圈：时变地幔流模拟
- 岩石圈：地球物理反演约束
- 地壳：考虑蛇河平原玄武质富集效应

**验证成果**

✅ 地表地形

✅ 地壳应力场（Aφ 参数）

✅ 地震各向异性

✅ 软流圈流动模式
</div>

::right::

![Fig.2](/images/literatures/science.ady2027-f2.jpg)

*Fig.2: 软流圈热流侵入蛇河平原下方，来自法拉隆板块俯冲驱动的向东地幔流。*

<!--
为了解释TLMPS的成因，作者构建了一个三维地球动力学模型。这个模型的独特之处在于同时计算岩石圈和软流圈的动力学。模型显示，法拉隆板块的俯冲驱动了向东的地幔流，这股"地幔风"在蛇河平原下方形成了一个热通道。
-->

---
layout: two-cols
---

::left::

# 应力状态与变形率预测

<div class="mt-4 text-sm">

**A–C | 应力状态（Aφ 参数）**
- 红色 = 拉张，蓝色 = 挤压
- 黄石及 ESRP 周缘：强烈拉张
- ESRP 东端：应力宁静

**D–F | 变形率**
- 高变形带向西南倾斜
- 与低速异常几何吻合

**G–I | 剖面对比**
- H（预测变形率）vs I（观测 P 波）
- **高变形通道 ≈ 低速异常**

</div>

::right::

![Fig.3](/images/literatures/science.ady2027-f3.jpg)

*Fig.3: 预测应力状态、变形率与观测地震结构对比。(A–F) 平面分布；(G–I) 沿剖面。预测的高变形舌状体与观测低速异常高度吻合。*

<!--
Fig.3是核心验证。模型预测的高变形率区域（H面板）与地震观测的低速体（I面板）在空间上惊人一致，证明TLMPS是构造变形的产物。
-->

---
layout: two-cols
---

::left::

# 构造力的"双重奏"

<div class="mt-4">

**1. 底部牵引力（Basal Traction）**
- 软流圈"地幔风"的剪切拖曳
- 在黄石西侧产生压缩
- 在黄石下方产生向东的拉张

**2. 岩石圈体力（Body Force）**
- 蛇河平原致密玄武质地壳下沉 → 拉张
- 黄石高海拔重力势能 → 拉张
- 东侧致密克拉通根 → 压缩

<div color="gray">
3. 相邻板块边界力 (plate boundary forces)
</div>

**叠加效应**
- ESRP 东端：**应力抵消** → 构造宁静区 → 火山空白区

</div>


::right::

![Fig.4](/images/literatures/science.ady2027-f4.jpg)

*Fig.4: 应力机制分解。(A,B) 总应力；(C,D) 底部拖曳力；(E,F) 岩石圈体力；(G,H) 沿剖面分解。两种应力在 ESRP 东端抵消，形成火山空白区。*

<!--
关键机制来了！作者提出两种构造力的叠加：底部拖曳力和岩石圈体力。软流圈流动像"风吹"岩石圈底部产生剪切；而岩石圈自身的密度差异像"重力拉扯"。两者叠加，在ESRP和黄石之间形成了一个应力"宁静区"——这就是火山空白区的成因！
-->

---
layout: center
class: text-center
---

## TLMPS 的三维构造模型

<div class="grid grid-cols-2 gap-8 items-center mt-8">
<div class="text-left text-lg">

**倾斜岩浆通道的几何形态**
- 上地壳：近垂直补给黄石岩浆房
- 中下地壳：向西南倾斜的玄武质糊状物
- 岩石圈地幔：近水平连接软流圈熔体

**构造控制核心**
- 底部拖曳 + 岩石圈体力
- 共同塑造三维应力场
- 应力宁静区 = 岩浆"分水岭"

</div>
<div>

![Fig.5](/images/literatures/science.ady2027-f5.jpg)

*Fig.5: TLMPS 三维概念模型。展示构造力如何塑造倾斜的跨岩石圈岩浆通道，以及火山空白区的应力抵消机制。*

</div>
</div>

<!--
Fig.5是全文总结。它将应力机制、变形场与岩浆路径整合为一个统一的三维模型，清晰展示了构造力如何"雕刻"出倾斜的岩浆通道。
-->

---
layout: two-cols
---

::left::

## 文章1 核心贡献总结


<div style="display: grid; grid-template-columns: repeat(1, 1fr); gap: 0.5rem; font-size: 0.75rem;">
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">1. 提出TLMPS概念</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>倾斜的跨岩石圈岩浆通道</li>
      <li>连通软流圈与地壳糊状物</li>
    </ul>
  </div>
  
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">2. 揭示构造控制机制</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>底部拖曳 + 岩石圈体力</li>
      <li>塑造三维应力场与变形</li>
    </ul>
  </div>
  
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">3. 解释双峰式火山分布</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>应力宁静区 = 火山空白区</li>
      <li>岩浆分流机制</li>
    </ul>
  </div>
  
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">4. 挑战地幔柱假说</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>无需深部地幔柱</li>
      <li>浅部软流圈熔体即可</li>
    </ul>
  </div>
</div>


::right::

<div class="h-full flex items-center justify-center">

<div class="text-center">
<div class="text-6xl mb-4">🎯</div>
<div class="text-2xl font-bold text-orange-400">

**Science 为何接受？**

</div>
<div class="text-left mt-6 text-lg">

<ul style="font-size: 0.9rem; line-height: 1.6;">
  <li><strong>颠覆性</strong>：挑战黄石地幔柱经典模型</li>
  <li><strong>多学科强约束</strong>：地震+电磁+模拟+地表记录</li>
  <li><strong>填补空白</strong>：回答"岩浆如何穿过刚性岩石圈"</li>
  <li><strong>普适性</strong>：为全球大火成岩省提供新范式</li>
  <li><strong>灾害意义</strong>：超级火山预测的新构造框架</li>
</ul>

</div>
</div>
</div>

<!--
第一篇总结。这篇文章的最大价值在于颠覆性——它挑战了教科书级的地幔柱假说，而且不是空口无凭，而是用多学科数据+高分辨率模拟给出了替代方案。这就是Science级别的创新。
-->

---
layout: center
class: text-center
---

# 文章二
# 马里亚纳俯冲带的水输入估算
## *Nature* (2018)

<div class="text-2xl mt-8 opacity-80">
Chen Cai, Douglas A. Wiens, Weisen Shen, Melody Eim
</div>
<div class="text-xl mt-4 opacity-60">
"Water input into the Mariana subduction zone estimated from ocean-bottom seismic data"
</div>

<!--
进入第二篇。这篇文章研究的是俯冲带的水循环——海水进入地球深部的"入口"。马里亚纳是地球上最深的海沟，也是研究俯冲带的天然实验室。
-->

---
layout: two-cols
---

## 俯冲带：地球深部的"水泵"

::left::

<div class="mt-4">

**核心问题**
- 俯冲带是唯一将水带入地球深部（>100 km）的机制
- 但**输入水通量估算存在巨大不确定性**
- 最大未知：俯冲板片上地幔的初始含水量

**前人研究局限**
- 主动源地震：只探测年轻板片，穿透深度有限
- 假设水化层厚度：通常仅 **2 km**
- 老、冷板片的数据严重缺失

</div>

::right::

<div style="display: flex; flex-direction: column; justify-content: center; align-items: center; height: 100%;">
  <img 
    src="/images/literatures/cai2018nature-f1.webp" 
    style="width: 100%; max-width: 800px; height: auto;"
  >
  <p style="font-size: 0.85rem; color: #555; margin-top: 12px; text-align: center;">
    <strong>Fig.1:</strong> 马里亚纳海沟地震台站分布（a）与外隆区高分辨率地形与地震（b）。红点=海底地震仪，白线=磁条带。
  </p>
</div>

<!--
俯冲带就像地球的水泵，把海水"抽"进地幔。但问题是：到底抽了多少水？前人估算差异巨大，主要是因为不知道俯冲板片的水化层有多厚。特别是像马里亚纳这样的老、冷板片（1.5亿年），数据非常缺乏。
-->

---
layout: two-cols
---

::left::

## 海底地震学突破

<div class="mt-4">

**技术创新**
- **19台海底宽频地震仪（OBS）** + 7个临时岛基台站
- 覆盖外隆区 + 前弧区

**方法优势**
- 瑞利面波分析（Rayleigh-wave）
- **剪切波速度（Vs）** 对水化更敏感
- 避免方位各向异性偏差
- 分辨深度更大（~60 km）

</div>

::right::

<div style="display: flex; flex-direction: column; align-items: center;">
  <img 
    src="/images/literatures/cai2018nature-f2.webp" 
    style="width: 53%; max-width: 800px; height: auto;"
  >
  <p style="font-size: 0.85rem; color: #555; margin-top: 12px; text-align: center;">
    <strong>Fig.2a-c:</strong> 跨海沟剖面的剪切波速度（Vsv）结构。暖色=低速（水化），冷色=高速。白圈=地震，白线=Moho面。
  </p>
</div>

<!--
这篇文章的方法突破在于使用了海底地震仪阵列。与船载主动源地震不同，OBS可以长期记录天然地震的面波信号，探测深度更大，而且对剪切波速度敏感——而剪切波对岩石水化（蛇纹石化）非常敏感。
-->

---
layout: center
class: text-center
---

## **水化层厚达 24 km！**

<div class="grid grid-cols-2 gap-8 items-center mt-8">
<div class="text-left text-xl">

**观测事实**
- 低速层从海沟轴向外延伸
- 底部达 **30±5 km** 深处
- 其中 **24±5 km** 进入上地幔
- 俯冲后仍保持 **30±5 km** 厚度

**关键机制**
- 板片弯曲区正断层发育
- 中性面深度 ~30 km
- 脆性破裂可深达此处
- 海水沿裂隙渗入 → 蛇纹石化

</div>
<div>

<div style="display: flex; flex-direction: column; align-items: center;">
  <img 
    src="/images/literatures/cai2018nature-f2.webp" 
    style="width: 52%; max-width: 800px; height: auto;"
  >
</div>

</div>
</div>

<div class="mt-6 text-2xl text-blue-400 font-bold">
💡 前人假设：2 km → 实际发现：24 km（12倍差异！）
</div>

<!--
这是文章的核心发现。地震成像显示，低速异常体（代表水化岩石）一直延伸到Moho面以下24公里！这意味着板片弯曲产生的正断层把海水带到了前所未有的深度。前人通常假设只有2公里，差了整整12倍。
-->

---
layout: two-cols
---

## 定量估算：水通量上调 4.3 倍

::left::

<div class="mt-4">

**计算参数**
- 蛇纹石化：~19 vol%（~2 wt% 水）
- 蛇纹石类型：利蛇纹石（低温稳定）
- 汇聚速率：50 mm/yr

**马里亚纳总水通量**
- 地幔蛇纹石化：**79±17 Tg/Myr/m**
- 沉积物 + 地壳（前人）：**15 Tg/Myr/m**
- **总计：94±17 Tg/Myr/m**

**对比前人估算**
- van Keken et al. (2011): ~22 Tg/Myr/m
- **本文结果：4.3 倍提升**

</div>

::right::

<div class="h-full flex flex-col justify-center">

<div class="bg-gray-300 p-6 rounded-lg mb-6">

### 全球尺度修正
**老、冷俯冲带**（>40 Myr）
- 水化层延伸至 Moho 下 **20-25 km**
- 全球深部水通量：**3.0×10⁹ Tg/Myr**
- **比前人估算增加约 3 倍**

</div>

<div class="text-sm opacity-80">

*注：年轻、暖板片（<40 Myr）600°C等温线浅，蛇纹石不稳定，维持前人估算。*

</div>
</div>

<!--
定量估算是这篇文章的另一大贡献。基于地震速度与水含量的实验标定关系，作者计算出马里亚纳的水通量是前人估算的4.3倍。推广到全球所有老、冷俯冲带，全球深部水通量需要上调约3倍。
-->

---
layout: two-cols
---

::left::

## 方位各向异性：裂隙的指向

<div class="mt-4 text-sm">

**短周期（12–16 s）**
- 快轴**平行海沟**
- 采样深度 ~25 km
- 对应水化裂隙/蚀变带
- 与正断层走向一致

**长周期（>27 s）**
- 快轴**平行古扩张方向**
- 反映深部未蚀变岩石圈
- 板块增生期各向异性

**启示**
- 低速层 = 板片弯曲裂隙 + 蛇纹石化
- 非各向同性孔隙介质

</div>

::right::

<div style="display: flex; flex-direction: column; justify-content: center; align-items: center; height: 100%;">
  <img 
    src="/images/literatures/cai2018nature-f3.webp" 
    style="width: 100%; max-width: 800px; height: auto;"
  >
  <p style="font-size: 0.85rem; color: #555; margin-top: 12px; text-align: center;">
    <strong>Fig.3:</strong> 方位各向异性结果。短周期（12-16s）快轴平行海沟→水化裂隙；长周期（>27s）快轴平行古扩张方向→板片各向异性。
  </p>
</div>

<!--
这里有一个有趣的地球系统科学问题。如果输入的水多了3倍，但海平面长期稳定，那输出端（火山弧、洋中脊）的水通量估算也可能被低估了。这提示我们需要重新思考弧岩浆的水含量和熔体通量。
-->

---
layout: two-cols
---

::left::

## 文章2 核心贡献总结


<div style="display: grid; grid-template-columns: repeat(1, 1fr); gap: 0.5rem; font-size: 0.75rem;">
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">1. 地震学突破</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>首次约束老、冷板片地幔水化层深度</li>
      <li>发现 24 km 厚水化层（前人 2 km）</li>
    </ul>
  </div>
  
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">2. 定量修正水通量</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>马里亚纳：上调 4.3 倍</li>
      <li>全球：上调约 3 倍</li>
    </ul>
  </div>
  
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">3. 揭示机制</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>板片弯曲正断层 → 深部水化</li>
      <li>中性面深度控制水化下限</li>
    </ul>
  </div>
  
  <div style="background: #f5f5f5; padding: 0.75rem; border-radius: 8px;">
    <strong style="font-size: 0.8rem;">4. 地球系统启示</strong>
    <ul style="margin: 0.5rem 0 0 0; padding-left: 1.2rem;">
      <li>挑战水循环收支平衡</li>
      <li>提示输出端（弧火山）估算不足</li>
    </ul>
  </div>
</div>


::right::

<div class="h-full flex items-center justify-center">

<div class="text-center">
<div class="text-6xl mb-4">🎯</div>
<div class="text-2xl font-bold text-green-400">

**Nature 为何接受？**

</div>
<div class="text-left mt-6 text-lg">

<ul style="font-size: 0.85rem; line-height: 1.6; margin: 0; padding-left: 1.2rem;">
  <li><strong>关键数据空白</strong>：首次给出老俯冲带水化层厚度硬约束</li>
  <li><strong>方法创新</strong>：海底OBS + 面波层析成像，突破主动源深度限制</li>
  <li><strong>重大估算修正</strong>：全球水通量上调3倍，影响深远</li>
  <li><strong>地球系统意义</strong>：挑战深部水循环平衡，开启新研究方向</li>
  <li><strong>普适性强</strong>：老俯冲带占全球大部分，适用性广</li>
</ul>

</div>
</div>
</div>

<!--
第二篇总结。这篇文章被Nature接受的核心原因是它解决了一个长期存在的"数据盲区"——老俯冲板片的水化层厚度。这个参数直接影响全球水循环估算，而前人一直靠猜测。本文用海底地震学给出了第一个硬约束。
-->



---
layout: center
class: text-center
---

# 不同视角，共同追求

<div class="grid grid-cols-2 gap-12 mt-8">
<div class="p-6 bg-gray-300 rounded-lg">

## 🔥 *Science* (2026)
**黄石火山**

**研究对象**：板内火山系统  
**核心方法**：三维地球动力学模拟  
**关键突破**：构造力控制岩浆路径  
**颠覆对象**：地幔柱假说  
**尺度**：岩石圈-软流圈相互作用  

</div>
<div class="p-6 bg-gray-300 rounded-lg">

## 🌊 *Nature* (2018)
**马里亚纳海沟**

**研究对象**：俯冲带系统  
**核心方法**：海底地震学成像  
**关键突破**：水化层厚度约束  
**颠覆对象**：全球水通量估算  
**尺度**：板片-地幔水交换  

</div>
</div>

<div class="mt-8 text-xl opacity-80">
共同主题：<span class="text-yellow-400 font-bold">利用先进地球物理技术，揭示深部过程，修正经典认知</span>
</div>

<!--
两篇论文虽然研究对象不同，但共享一个核心方法论：用先进的地球物理观测（三维模拟、海底地震）去约束过去只能靠猜测的深部参数，从而修正我们对地球系统的基本认知。
-->

<div class="mt-12">
<span @click="$slidev.nav.next" class="px-4 py-2 rounded cursor-pointer bg-white bg-opacity-10 hover:bg-opacity-20 transition">
进入 Q&A <carbon:arrow-right class="inline"/>
</span>
</div>

---
layout: center
class: text-center
---

# Q&A / 致谢

<div class="text-2xl mt-8 opacity-80">
感谢聆听，欢迎提问！
</div>

<div class="mt-12 text-lg opacity-60">
参考文献：
</div>
<div class="text-sm opacity-50 mt-2">

1. Cao, Z., Liu, L., Wan, B., Chen, L., & Lundstrom, C. (2026). Tectonic origin of Yellowstone's translithospheric magma plumbing system. *Science*, 392(6794), eady2027.

2. Cai, C., Wiens, D. A., Shen, W., & Eim, M. (2018). Water input into the Mariana subduction zone estimated from ocean-bottom seismic data. *Nature*, 563, 389-392.

</div>

<div class="abs-br m-6 text-sm opacity-50">
  Sonder
</div>

<!--
结束页。这两篇文章都是地球深部过程研究的典范，展示了如何通过技术创新获取关键约束，从而推动学科认知的范式转变。谢谢大家！
-->

