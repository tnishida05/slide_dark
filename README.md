# スライドテンプレート（ダークモード）

## コンパイルについて

lualatexを利用します。必要ない場合、`jobname` や `output-directory` は取り除いてください。
```
lualatex -jobname=output -output-directory=output main.tex
```
上のようにコンパイルした場合は、次のように bibtex を実行してください。
windowsのcmdで実行する場合、パス区切り文字に注意してください。
```
pbibtex output/output.aux
```

相互参照のため、`lualatex` → `pbibtex` → `lualatex` → `lualatex` と実行してください。
`latexmk`など使うと、良い感じにやってくれると思います。

その他、GUIのソフトを使う場合も、`lualatex`でのコンパイルであれば問題ありません。

出力結果は、`output/output.pdf`です。

## 色設定について

このテンプレートは、`metropolis`というテーマを利用しています。

ライトモードを基準にして、「紺色」をイメージして色を設定しました。
背景色が青みがかった黒なので、追加する色によっては見た目が悪くなるかもしれません。
