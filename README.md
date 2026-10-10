# Rokid DOOM

表示付き Rokid AI Glasses / RV101 を対象にした、初代 DOOM エンジンの非公式 Android APK です。

**開発中・実機未検証。** DOOM エンジンはグラス内の Android WebView / WebAssembly で動作し、PCからの映像転送は不要です。
Freedoom Phase 1 0.13.0 を同梱し、手持ちの DOOM / DOOM II の IWAD を取り込めます。市販 DOOM のゲームデータは含みません。

- 480×640 の縦画面内、中央 448×336 に4:3補正したゲーム画面を表示
- 緑の階調表示、カラー切替
- タップ・前後スワイプ・ダブルタップ、ゲームパッド入力
- 相対姿勢センサーによる旋回モード（実機検証待ち）
- オフライン実行、外部通信権限なし

初版APK、詳細な操作手順、検証スクリーンショットを準備中です。

## 構成

`app/` : AndroidホストとWebViewゲームUI

`vendor/doomgeneric/` : DOOMエンジンの上流ソース（GPL-2.0）

上流: https://github.com/ozkl/doomgeneric （dcb7a8dbc7a16ce3dda29382ac9aae9d77d21284）

配布済みWebAssembly: https://ozkl.github.io/doomgeneric/doomgeneric.wasm

Freedoom: https://freedoom.github.io/ （同梱ライセンス: app/assets/COPYING.txt）

このプロジェクトはRokid、id Software、Freedoom公式による製品ではありません。
