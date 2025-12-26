# どこでもバキュームベット  
*Anywhere Vacuum Bed / Rubber Vacuum Bed*

掃除機と袋があれば、どこでも簡易的な真空固定・圧縮ができる  
オープンソースのバキューム治具です。

![overview](document/img/overview.jpg)

3Dプリンタ（FDM）で再現可能。  
専用シートや高価な真空ポンプは不要です。

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

---

## 想定用途

- 簡易バキュームベッド / 仮固定治具
- 収納・圧縮（衣類・ぬいぐるみ等）
- ゴム・ラバー・TPU・フィルム等の柔軟素材固定
- 塗装・接着・成形前の仮固定
- 教育・FabLab・DIY用途
- 個人利用・研究用途

⚠ **人体・物体を問わず、使用はすべて自己責任です。**  
⚠ 本設計は医療・安全認証を意図したものではありません。

---

## クイックリンク（最初に読む）

- 🔧 **組み立て方法（Assembly）**  
  → [`document/howto/assembly.md`](document/howto/assembly.md)

- 🧰 **使い方：伸縮性のない一般ゴミ袋**  
  → [`document/howto/use_trashbag.md`](document/howto/use_trashbag.md)

- 📐 **FreeCAD 全体アセンブリ**  
  → [`Assembly.FCStd`](Assembly.FCStd)

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