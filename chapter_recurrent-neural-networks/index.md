# リカレントニューラルネットワーク
:label:`chap_rnn`

これまで、表形式データと画像データの 2 種類のデータに遭遇しました。後者については、規則性を活用するために特殊なレイヤーを設計しました。言い換えれば、画像内のピクセルを置換すると、アナログTVの時代のテストパターンの背景によく似たものの内容を推論することははるかに困難になります。 

最も重要なことは、これまでのところ、私たちのデータはすべて何らかの分布から引き出され、すべての例が独立して同一に分布している（つまり、すなわち）ことを暗黙のうちに想定していたことです。残念ながら、これはほとんどのデータには当てはまりません。例えば、この段落の単語は順番に書かれており、ランダムに並び替えればその意味を解読するのはかなり難しいでしょう。同様に、動画の画像フレーム、会話の音声信号、Web サイトでの閲覧行動は、すべて順番に従います。したがって、そのようなデータに特化したモデルの方がより適切に記述できると仮定するのが妥当です。 

別の問題は、シーケンスを入力として受け取るだけでなく、シーケンスを継続することが期待されるかもしれないという事実から生じます。たとえば、$2, 4, 6, 8, 10, \ldots$系列を継続することが課題です。時系列分析では、株式市場、患者の発熱曲線、レースカーに必要な加速度を予測するためによく見られます。繰り返しますが、このようなデータを処理できるモデルが必要です。 

つまり、CNN は空間情報を効率的に処理できますが、*リカレントニューラルネットワーク (RNN) はシーケンシャルな情報をより適切に処理できるように設計されています。RNN は、現在の入力とともに過去の情報を格納する状態変数を導入し、電流出力を決定します。 

リカレントネットワークを使用する例の多くは、テキストデータに基づいています。したがって、この章では言語モデルを強調します。シーケンスデータのより正式なレビューの後、テキストデータを前処理するための実用的な手法を紹介します。次に、言語モデルの基本的な概念について議論し、この議論をRNNの設計のためのインスピレーションとして利用する。最後に、このようなネットワークを訓練する際に遭遇する可能性のある問題を探るために、RNNの勾配計算法について説明します。

```toc
:maxdepth: 2

sequence
text-preprocessing
language-models-and-dataset
rnn
rnn-scratch
rnn-concise
bptt
```
