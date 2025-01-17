#  予選
:label:`chap_preliminaries`

ディープラーニングを始めるには、いくつかの基本的なスキルを身に付ける必要があります。すべての機械学習は、データから情報を抽出することに関係しています。そこで、データの格納、操作、前処理に関する実践的なスキルを習得することから始めます。 

さらに、機械学習では通常、行が例に対応し、列が属性に対応するテーブルと考えることができる大きなデータセットを扱う必要があります。線形代数は、表形式データを操作するための強力なテクニックを提供します。雑草についてはあまり詳しく説明しませんが、行列演算の基本とその実装に焦点を当てます。 

さらに、ディープラーニングは最適化がすべてです。いくつかのパラメーターを持つモデルがあり、データに*最適*適合するモデルを見つけたいと考えています。アルゴリズムの各ステップで各パラメーターをどの方向に移動させるかを決定するには、少し計算が必要です。これについて簡単に説明します。幸いなことに、`autograd` パッケージは微分を自動的に計算してくれます。これについては次で説明します。 

次に、機械学習は予測を行うことに関係します。観察した情報を考えると、未知の属性にはどのような値がありそうなのでしょうか？不確実性のもとで厳密に推論するには、確率の言語を呼び出す必要があります。 

最終的には、公式ドキュメントには、この本にはない多くの説明と例が記載されています。この章を締めくくるために、必要な情報のドキュメントを検索する方法を示します。 

本書では、ディープラーニングを正しく理解するために、数学的な内容を最小限に留めておきました。しかし、この本が数学フリーであるという意味ではありません。したがって、この章では、本書の数学的な内容の少なくとも「ほとんど」を誰でも理解できるように、基礎的でよく使われる数学を素早く紹介する。数学的な内容の「すべて」を理解したいなら、[online appendix on mathematics](https://d2l.ai/chapter_appendix-mathematics-for-deep-learning/index.html) をさらに復習すれば十分でしょう。

```toc
:maxdepth: 2

ndarray
pandas
linear-algebra
calculus
autograd
probability
lookup-api
```
