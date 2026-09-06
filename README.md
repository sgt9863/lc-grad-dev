# lc-grad-dev

グラジエント LC メソッド設計ツール（**stlite** 版）の公開用リポジトリ。

- 公開先: <https://sgt9863.com/lc-grad-dev/>
- 開発元: `~/Claude/lc-method-dev`（ローカル。ここには成果物だけを置く）

## これは何か

LSS モデル（`log k = log kw − S·Φ`、温度は線形項）で保持を予測し、
ピーク幅から N・カラム外分散を推定して、**グラジエント条件のデザインスペース**を
描くツール。ブラウザだけで動く（Pyodide / stlite）ので、インストール不要。

## 中身

| ファイル | 中身 |
|---|---|
| `index.html` | stlite の 1 枚 HTML。Streamlit アプリと `lcmd` パッケージ一式を内蔵 |
| `.nojekyll` | GitHub Pages の Jekyll 処理を止める |

実験データ（クロマトグラム・帰属結果）は**含まれていません**。コードのみ。

## 更新のしかた

開発リポジトリ側でビルドしてから、ここへコピーして push する。

```sh
cd ~/Claude/lc-method-dev
.venv/bin/python tools/build_stlite.py
.venv/bin/python tools/publish_site.py --out ~/Claude/lc-grad-dev
cd ~/Claude/lc-grad-dev && git add -A && git commit -m "rebuild" && git push
```
