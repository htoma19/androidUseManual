# AndroidStudio利用マニュアル
## プロジェクトの作成
### コマンドプロンプトで下記コマンドを実行
- npx @react-native-community/cli init MyKakeiboApp
## 仮想スマホを起動
- Android Studioを開き、「More Actions」>「Virtual Device Manager」を押下
- すでにある仮想スマホの右側の「▶︎（再生ボタン）」を押して起動（なければ「Create device」から作成）
- コマンドプロンプトでアプリのフォルダに移動
- コマンドプロンプトで下記コマンドを実行
  - npx react-native run-android
## プロジェクトのクリーンアップ
### 1. キャッシュのクリア（重要！）
 - npm start -- --reset-cache
### 2. androidフォルダに移動
 - cd android
### 3. ビルドゴミを削除
 - ./gradlew clean
### 4. 元のフォルダに戻る
 - cd ..
### 5. サーバー再起動
 - npx react-native start --reset-cache
