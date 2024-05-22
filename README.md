facebook開発のprophetを使った予測

prophetを理解するのにこのサイトが非常にわかりやすい　    https://devblog.thebase.in/entry/2019/12/20/110000_1
原論文　https://peerj.com/preprints/3190.pdf

y(t) = g(t) + s(t) + h(t) + ε   で時系列を表す

g(t): トレンド関数     s(t): 季節変化     h(t): イベント効果    ε:誤差項


とりあえずデフォルトで予測(使った井戸は15T)

予測外している箇所をピックアップ

optunaで予測改善はかる(時間結構かかる)

sktimeが提供しているupdate()という学習メソッドを使用してfit()とのパフォーマンスを比較

使った時系列データは2016年8月２２日から同年9月17日

学習粒度を1時間　学習期間20日間　予測期間7日間とした
