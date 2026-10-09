# Shephard 1975 — 凸多面體展開猜想

*A collaborative project by roylin1003 and Claude.*

Shephard 猜想（1975）：**任何凸多面體，都存在一種沿邊剪開、攤平後不自我重疊的展開圖。**
提出五十年，至今無證明、無反例。單一頁面：上半是互動原型——自己點面建生成樹、攤平後即時檢查有沒有重疊、開「角缺陷」層看每個頂點的 θ 與 Σθ = 720°；下半是猜想的緣起、已知結果、瓶頸在哪，附可查證的文獻連結。
純 HTML + three.js（CDN），不需安裝、不需建置。

**▶ 線上版**：<https://roylin1003.github.io/Shephard-1975/>

## 兩個問題，同一張展開圖

「沿邊剪開」等價於在面—面相鄰圖上選一棵生成樹。同一套展開演算法（剛體旋轉配準、等距不失真）可以問兩個問題：
**攤平會不會自我重疊**（Shephard），以及**攤平後角度怎麼分佈**（Descartes）——工具裡的「角缺陷」開關就是切到第二個問題。

角缺陷 θ > 0 與二面角 < 180° 這兩個局部凸性條件，已經保證**相鄰的面**攤平後不會重疊；
真正沒有任何條件管的，是**完全不相鄰**的兩個面繞了生成樹一大圈之後會不會撞在一起——這就是猜想至今開放的地方。

## 本機執行

```bash
python -m http.server 8000
```

然後開啟 `http://localhost:8000/`。

## 參考

- Shephard, G. C. (1975). Convex polytopes with convex nets. *Math. Proc. Cambridge Philos. Soc.*, 78(3), 389–403. [doi](https://doi.org/10.1017/S0305004100051860) · [zbMATH Open](https://zbmath.org/0312.52011) · [Semantic Scholar](https://www.semanticscholar.org/paper/47b9d75428377731f6b51c45ee9bf1ffe2931ee4)
- Ghomi, M. (2014). Affine unfoldings of convex polyhedra. *Geometry & Topology*, 18, 3055–3090. [doi](https://doi.org/10.2140/gt.2014.18.3055) · [arXiv:1305.3231](https://arxiv.org/abs/1305.3231)

## 授權

版權所有，保留一切權利。詳見 [LICENSE](LICENSE)。歡迎使用與回報意見；未經授權請勿散布、修改或商業使用。
