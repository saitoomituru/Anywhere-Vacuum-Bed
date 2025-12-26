# どこでもバキュームベット
## 作り方：逆流防止弁ユニット組み立て

本ドキュメントは、
「どこでもバキュームベット」に使用する **逆流防止弁ユニット** の
組み立て方法を示します。

本構造は **FDM 3Dプリント前提・実験用途向け** です。

# Anywhere Vacuum Bed
## Assembly: Check-valve unit (CA/TX English)

This guide shows how to assemble the **check-valve unit** for the Anywhere Vacuum Bed. The construction assumes FDM 3D printing and experimental use.

---

## 使用部品（STL）

- 逆流防止弁本体
  `逆流防止弁-AssemblyPocket005.stl`
- オスネジ部
  `オスネジ-AssemblyAdditiveHelix.stl`
- ゼロテンションワッシャ
  `付属逆流防止弁ワッシャ-AssemblyHole.stl`

**Parts (STL files)**

- Check-valve body: `逆流防止弁-AssemblyPocket005.stl`
- Male thread section: `オスネジ-AssemblyAdditiveHelix.stl`
- Zero-tension washer: `付属逆流防止弁ワッシャ-AssemblyHole.stl`

---

## 逆流防止弁（ゴム部）の仕様

### 形状
- ドーナツ状（円環）
- 外径：**45mm**
- 内径：**5mm**
- 厚み：**0.4mm**

### 素材
- **Latex（天然ゴム）**
- 検証済み素材：
  - フェティッシュ用途 高品質衣料用 Latex
  - 厚み 0.4mm

※ 本設計では **伸縮性・復元性・表面平滑性** を重視しています。

**Check-valve rubber spec (CA/TX English)**

### Shape
- Donut (torus)
- Outer diameter: **45 mm**
- Inner diameter: **5 mm**
- Thickness: **0.4 mm**

### Material
- **Latex (natural rubber)**
- Verified material:
  - High-quality clothing-grade latex for fetish use
  - Thickness 0.4 mm

The design prioritizes stretch, recovery, and surface smoothness.

#### 検証済み素材（Latex 0.4mm）

- 販売元：くらげ（KURAGE）
- 用途：高品質衣料用 Latex
- 検証厚み：0.4mm

[https://kurage.style](https://kurage.style)

#### Verified material (Latex 0.4 mm)

- Vendor: Kurage (KURAGE)
- Application: high-grade apparel latex
- Verified thickness: 0.4 mm

[https://kurage.style](https://kurage.style)

---

## 組み立て手順

### 1. ゴム弁のセット

1. 逆流防止弁本体
   `逆流防止弁-AssemblyPocket005.stl`
   の指定位置に、Latex ドーナツを配置します。
2. ゴム面は **シワ・ねじれが無い状態** にしてください。

### 1. Set the rubber valve

1. Place the latex donut on the designated seat of `逆流防止弁-AssemblyPocket005.stl`.
2. Keep the rubber smooth with **no wrinkles or twist**.

---

### 2. オスネジ部の固定

1. `オスネジ-AssemblyAdditiveHelix.stl` を
   ガイドに沿って嵌め込みます。
2. 本体とネジ部の **嵌合隙間** に
   以下のいずれかを流し込み、固定します。

#### 使用可能な接着剤
- シアノアクリレート（瞬間接着剤）
- 低粘度・浸透系接着剤（毛細管浸透タイプ）

※ ゴム面には接着剤を付着させないでください。

### 2. Fix the male-thread section

1. Fit `オスネジ-AssemblyAdditiveHelix.stl` along the guide.
2. Wick one of the following into the **fit clearance** between body and thread to lock it in place.

#### Approved adhesives
- Cyanoacrylate (instant adhesive)
- Low-viscosity penetrating adhesive (capillary type)

Do not let adhesive touch the rubber face.

---

### 3. ゼロテンションワッシャの挿入

1. `付属逆流防止弁ワッシャ-AssemblyHole.stl`
   を **ゴム弁の上に噛ませます**。
2. このワッシャは
   - ゴムの初期テンションを与えない
   - 面圧を均一化する
   目的で使用します。

### 3. Insert the zero-tension washer

1. Set `付属逆流防止弁ワッシャ-AssemblyHole.stl` **on top of the rubber valve**.
2. This washer avoids pre-tension on the rubber and evens out surface pressure.

---

### 4. M3 ネジ固定

1. M3 ネジ（**長さ10mm**）を使用
2. ナットは、弁本体側に
   **ハンダゴテで熱圧入**してください。
3. 締め込みは
   **ゴムが潰れない最小限** に留めます。

### 4. Tighten with M3 hardware

1. Use M3 screws (**length 10 mm**).
2. Heat-set the nuts into the valve body with a soldering iron.
3. Tighten only enough to avoid crushing the rubber.

---

## シール処理（重要）

本設計では **FDM積層による微細リーク対策として
シリコングリス使用を前提** としています。

## Sealing steps (important)

The design assumes **silicone grease to counter micro-leaks from FDM layers**.

### 方法A：シリコングリスのみ（簡易）
- 中央ゴム面に **薄く塗布**
- 外周シール溝にも薄塗り

### 方法B：トップコート併用（耐久重視）
1. FDM面に  
   **透明表面コート系塗料** を薄く塗布
2. 完全乾燥後
   **50cs シリコンオイル** を添付

※ 潤滑目的ではなく **気密補助目的** です。

### Option A: Silicone grease only (simple)
- **Light coat** on the center rubber face
- Light coat on the perimeter sealing groove

### Option B: With top coat (durability focused)
1. Brush a **clear surface coat** lightly onto the FDM faces.
2. After full cure, add **50 cs silicone oil**.

Note: This is for airtightness assistance, not lubrication.

---

## 動作確認

- 指で軽く吸って戻すと
  ゴム弁が **自然に開閉** する
- 強く吸うと
  ゴム面が均一に密着する
- 逆方向から吹いても
  漏れが起きにくい

## Function check

- A gentle suck-and-release with a finger makes the valve **open and close naturally**.
- Strong suction seats the rubber face evenly.
- Blowing from the reverse side is unlikely to leak.

---

## 備考

- ゴム材質・厚み変更は可能ですが
  **0.4mm Latex が最も安定** しました
- FDM積層精度・材料差により
  グリス量は調整してください
- 本設計は **人体・物体問わず自己責任利用** です

## Notes

- You can change rubber material or thickness, but **0.4 mm latex proved most stable**.
- Tune grease amount to your FDM precision and material.
- Use at your own risk for both people and objects.

---

