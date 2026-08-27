# Hiyomaru Rhythm v0.5.7

BGM本命修正版です。

## 原因
ゲームスクリプトが `document.getElementById("bgm")` を実行した時点で、
`<audio id="bgm">` がまだHTMLの後方にあり、BGM要素を取得できていませんでした。

## 修正
- `<audio id="bgm">` をゲームJavaScriptより前に移動
- v0.5.6の「3.04秒無音リードイン」方式を継続
- スタートをタップした瞬間に再生開始
- 3 → 2 → 1 → GO! の間は無音
- GO!終了付近からBGM本編開始
- 音ON/OFF機能を継続

GitHub Pagesのrootへ、このZIPの中身をすべて上書きアップロードしてください。
