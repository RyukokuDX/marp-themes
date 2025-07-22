---
marp: true
theme: rdx
paginate: true
math: katex
---

<!-- _class: lead -->

# RDXのスライドテンプレート的なもの

### 〜Beamerを卒業できない??〜

<br>

**藤原 和将**
2025/07/21

---

<!-- _header: 目次 -->

1. はじめに
1. vscode/Cursor への導入
1. 本スタイルを利用する為のフロントマター

---

<!-- _header: はじめに -->

- Marp とは **Markdown** で**スライド**を作成するためのソフトウェアである。
  - 基本的な Markdown のシンタックスがサポートされている。

- 本テンプレートは, rdxのサンプルテンプレートである。

- Markdown 上で `---` という区切り線を入れるだけで、次のページに移動することができる。$^1$

> 註については, [kaisugi/marp-theme-academic](https://github.com/kaisugi/marp-theme-academic)のコードを流用しています


---

<!-- _header: VScode/Cursor への導入 -->
1. `setting.json`を開く
  - windowsなら`Ctrl+Shift+P`で`settings.json`を検索
  - macなら`Cmd+Shift+P`で`settings.json`を検索

2. json内に以下を追加
```json
"markdown.marp.themes": [
    "https://ryukokudx.github.io/marp-themes/rdx.css",
],
```

---
<!-- _header: 本スタイルを利用する為のフロントマター  -->

コードのフロントマターとして以下を先頭に追加
```md
---
marp: true
theme: rdx
painate: true
math: katex
---
```