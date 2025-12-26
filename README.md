# どこでもバキュームベット
*Anywhere Vacuum Bed / Rubber Vacuum Bed*

*Anywhere Vacuum Bed* is an open, vacuum-fixture style project you can build anywhere with just a household vacuum and a bag—no specialty pumps needed.

掃除機と袋があれば、どこでも簡易的な真空固定・圧縮ができる
オープンソースのバキューム治具です。

With a regular shop vac and a bag, you get quick vacuum clamping or compression anywhere. The whole design is open source.

![overview](document/img/overview.jpg)

3Dプリンタ（FDM）で再現可能。
専用シートや高価な真空ポンプは不要です。

Reproducible on common FDM printers. No custom sheets or pricey vacuum pumps required.

▶️ Demo Video (2 min)  
https://youtube.com/shorts/qQuK8cIHQdQ?si=-0dno3jXxC5wWSed


---

## 特徴

- 掃除機・ブロワ対応（真空ポンプ不要）
- 袋（PE / PP / PVC / TPU など）を消耗品として使用
- 伸びる素材・伸びない素材の両対応
- 薄く柔らかい素材でも流路を塞がない裏側リブ構造
- 逆流防止弁内蔵（初速・保持の両立）
- 工具不要で解除可能
- FDM積層の気密問題を**シリコングリス前提**で解決
- 年齢・用途を限定しない構造（使用は自己責任）

**Features (California/Texas US English)**

- Works with household vacuums and blowers—no dedicated pump.
- Uses common bags (PE/PP/PVC/TPU, etc.) as consumables.
- Handles stretchy and non-stretch films alike.
- Backside ribs keep airflow paths open even with thin, soft materials.
- Built-in check valve balances fast start-up with reliable holding.
- Release without tools.
- Airtightness assumes silicone grease to tame FDM layer leakage.
- Open form factor for all ages and uses—always at your own risk.

---

## 想定用途

- 簡易バキュームベッド / 仮固定治具
- 収納・圧縮（衣類・ぬいぐるみ等）
- ゴム・ラバー・TPU・フィルム等の柔軟素材固定
- 塗装・接着・成形前の仮固定
- 教育・FabLab・DIY用途
- 個人利用・研究用途

**Intended Uses (CA/TX English)**

- Quick vacuum bed or temporary jigging.
- Storage and compression for clothes, plush toys, and similar items.
- Holding flexible materials such as rubber, TPU, and films.
- Temporary holding before painting, bonding, or forming.
- Education, FabLab, and DIY settings.
- Personal projects and research.

⚠ **人体・物体を問わず、使用はすべて自己責任です。**
⚠ 本設計は医療・安全認証を意図したものではありません。

⚠ **Use at your own risk for people or objects.**
⚠ This design is not intended for medical or safety certification.

---

## クイックリンク（最初に読む）

- 🔧 **組み立て方法（Assembly）**
  → [`document/howto/assembly.md`](document/howto/assembly.md)

- 🧰 **使い方：伸縮性のない一般ゴミ袋**
  → [`document/howto/use_trashbag.md`](document/howto/use_trashbag.md)

- 📐 **FreeCAD 全体アセンブリ**
  → [`Assembly.FCStd`](Assembly.FCStd)

**Quick Links (read first)**

- 🔧 Assembly guide → [`document/howto/assembly.md`](document/howto/assembly.md)
- 🧰 Using non-stretch trash bags → [`document/howto/use_trashbag.md`](document/howto/use_trashbag.md)
- 📐 Full FreeCAD assembly → [`Assembly.FCStd`](Assembly.FCStd)

---

## ディレクトリ構成

```text
/
├─ README.md
├─ Assembly.FCStd              # 全体アセンブリ（FreeCAD）
├─ Bild/
│  └─ Assy/
│     └─ *.FCStd               # 各パーツ（FreeCAD）
├─ stage/
│  └─ stl/
│     └─ *.stl                 # 3Dプリント用STL
└─ document/
   ├─ img/                     # 写真・図解
   └─ howto/                   # 作り方・使用方法
      ├─ assembly.md
      └─ use_trashbag.md
```


---

## 仕組みについて（設計思想）

### 裏側リブ構造
裏側の放射リブ形状は、

- 薄い素材が吸着時に流路を塞がない
- 真空初速を維持
- 完全密閉にならず自然解除しやすい

という **安全側に倒した流路保持構造**です。

**Design Approach (CA/TX English)**

### Backside rib structure
The radiating ribs on the underside are sized so that thin materials don’t choke the airflow, startup vacuum speed stays quick, and the system can gently vent instead of locking shut—prioritizing safe flow retention.

---

## シールについて（FDM前提）

本設計では **シリコングリスの使用を前提**としています。

- FDM積層による微細リーク対策
- 材料・プリンタ個体差の吸収
- 分解・清掃・再利用が容易

**Sealing (FDM-first perspective)**

The design assumes silicone grease from the start. It handles micro-leaks from FDM layers, smooths out printer/material variances, and keeps teardown and cleaning simple.

### 塗布箇所
- 外周の袋シール溝
- **中央の逆流防止ゴム面（薄塗り）**

※ 潤滑ではなく **気密補助目的**です。

### Where to apply
- Perimeter groove that seals the bag.
- **Center check-valve rubber face (light coat).**

Note: This is for airtightness support, not for lubrication.

---

## 袋の取り付け方法（2通り）

### ① 伸びる素材（PE / TPU など）
1. 袋に **約52mmの穴**を開ける
2. 本体に袋を挟み、ネジで固定

### ② 伸びない素材（PP / 硬質PVC 等）
1. **袋に下穴は開けない**
2. そのまま本体に袋を挟んで固定
3. バキューム前に
   **中央吸入口に指を入れて袋を破る**
4. そのまま吸引開始

※ 中央弁構造により、
　破断後も袋が吸い込まれにくい設計です。

**How to attach bags (two options)**

### 1) Stretchy materials (PE/TPU, etc.)
1. Punch a **~52 mm hole** in the bag.
2. Clamp it to the body and tighten the screws.

### 2) Non-stretch materials (PP, rigid PVC, etc.)
1. **Do not pre-drill** the bag.
2. Clamp it to the body as-is.
3. Right before vacuuming, **poke the center inlet with a finger to tear the film.**
4. Start vacuuming immediately.

The center valve design keeps the torn bag from getting sucked in.

---

## 使用・解除方法（概要）

### 使用
1. 袋に対象物を入れる
2. 袋の口を縛る
3. 掃除機で吸引

### 解除
- ネジを外す
- 袋の端をつまむ
（工具不要）

**Use / Release (overview)**

### Use
1. Place the item in the bag.
2. Tie the bag closed.
3. Pull vacuum with a household vacuum.

### Release
- Remove the screws.
- Pinch the bag edge to vent (no tools needed).

---

## 3Dプリントについて

- 推奨方式：FDM
- 材質：PLA / PETG / ABS（用途に応じて）
- 機能面（シール面）は **ビルドプレート直置き推奨**
- サポート不要設計

**3D printing notes**

- Recommended process: FDM.
- Materials: PLA / PETG / ABS depending on use.
- Functional sealing faces: **print flat on the build plate**.
- Designed to avoid supports.

---

## FDM造形テック（サポート不要設計）

本設計では、**裏側リブおよび溝構造の幅をすべて 5mm 以下**に制限しています。

これは一般的なFDM 3Dプリンタにおいて、

- サポート材を使用せずに
- 安定したオーバーハング／ブリッジ造形が可能

という **実運用での再現性**を最優先した設計判断です。

**FDM build strategy (supportless)**

All underside rib and groove widths stay at or below 5 mm. On typical FDM printers, that means you can bridge and overhang without supports while keeping real-world repeatability as the top priority.

### この設計によるメリット

- サポート除去が不要
  → 表面荒れ・寸法誤差・シール面破壊を防止
- 印刷後の後処理が不要
  → プリント後すぐに使用可能
- シール面の平面性を確保
  → 真空用途における気密性向上

### Benefits of this approach

- No support removal → avoids surface roughness, dimensional drift, and seal-surface damage.
- No post-processing → use the print right away.
- Flat sealing surfaces → better airtightness for vacuum duty.

### 設計思想（FDM前提）

- 真空流路として十分な断面を確保しつつ
- 「FDMで確実に橋渡しできる寸法」を上限条件として採用

この 5mm という数値は理論値ではなく、

- ノズル径：0.4mm  
- レイヤー高：0.2〜0.28mm  
- 家庭用FDMプリンタ

という **一般的な環境での実証ベース**の設計です。

真空用途のため、微細な糸引きや軽微なたわみは
**機能的に問題にならない**ことも考慮しています。

むしろサポートを使用することで、

- シール面の精度低下
- 表面の荒れ
- 再現性の低下

が起きやすいため、本設計では **サポート不要を前提**としています。

### Design mindset (FDM-first)

- Cross-sections stay big enough for vacuum flow while capped at dimensions that bridge reliably on FDM.
- The 5 mm limit is practical, not theoretical—based on common home FDM setups (0.4 mm nozzle, 0.2–0.28 mm layers).
- For vacuum use, small strings or slight sag usually don’t matter.
- Using supports tends to hurt seal precision, roughen surfaces, and lower repeatability, so the design assumes no supports.

---


## ライセンス

本プロジェクトは **CERN Open Hardware Licence Version 2 – Permissive (CERN-OHL-P)**
の下で公開されています。

**License**

Released under the **CERN Open Hardware Licence Version 2 – Permissive (CERN-OHL-P)**.

- 商用利用可
- 改変可
- 再配布可
- 派生物の公開義務なし

⚠ **本設計の使用により生じた事故・損害について、作者は一切の責任を負いません。**

ライセンス全文：  
https://ohwr.org/cern_ohl_p_v2.txt

---

## 名前について

「どこでもバキュームベット」は  
**ドラえもん道具的に、誰でも・どこでも使える道具**  
という思想から名付けています。

用途・文脈・分野は限定していません。

---

## English (Short)

**Anywhere Vacuum Bed**  
An open-source vacuum fixture using a vacuum cleaner and plastic bags.

Released under **CERN-OHL-P v2**.  
Use at your own risk, for any object or body.

---


