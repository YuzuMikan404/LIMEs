

## 1.34.beta

yml



## 1.34.beta

[Yml]
NPatchもパッチ済みに配布

[IMEsTalkBackUpRestore(dev now)[15.12.2]]

- 完全なバックアップを行えないのを修正(May be)



## 1.34.beta

[Yml]
NPatchもパッチ済みに配布

[IMEsTalkBackUpRestore(dev now)[15.12.2]]

- 完全なバックアップを行えないのを修正(May be)



## 1.34.beta

[15.12.2 Only]
- LIMEsTalkBackUpRestore[15.12.2]
　LIMEsオリジナルのトークバックアップ機能の作成
 -Request by 不要那麼凶好不好？ for Discord
-GetToken(FCM)の際contextが取得する前に、getSharedPreferencesが行われていたので、取得を最適化
- Reported by Kotobuki (寿) for Discord

[All Versions: Function Fix]
NotificationReactionで誤った画像が取得されるのを修正
- Report by kamoshita for Discord



## 1.34.2.1beta

URI SETTING FIX



## 1.34.2.beta

E2EE_Disable機能の追加
<危険です,設定をサーバーに送信したい場合、プライバシー管理→LetterSealing以外の項目をON or OFFにしてください>
https://discord.com/channels/1392057820316303362/1479429727239405659
特定の設定状態の際に既読をつけるボタンをおしても既読がつかないのを修正
https://discord.com/channels/1392057820316303362/1480399111378305058
通知に既読をつけるアクションの作成
https://discord.com/channels/1392057820316303362/1479019001945260152
15.12.2既読確認ボタン初期位置を修正
https://discord.com/channels/1392057820316303362/1478537682555637852
May be TokenGetでトーストが限りなく表示されてしまうのを修正



## 1.34.1.bata

minimumAcceptableKeywordLength がNotificationカテゴリに分類されていたのをchatに変更



## 1.34.0.bata

検索時キーワードを1文字でもできるようにするminimumAcceptableKeywordLength機能の追加

16.2.0で以下の機能の対応
removeNaviAichat系
写真のリネーム保存機能
OriginalToneの動的検出機能
RemoveVoiceRecord_Hook_aの対応

自動で着信拒否にするは未対応



## 1.33.2.bata

既読を付けるボタンの作成
非 Root トークバックアップ、復元の別オプション化と設定ボタンの追加
removePremiumRecommendationの改善



## 1.33.1.beta

remove ads の修正



## 1.33.0.beta

remove ads の修正



## 1.33.0.beta

臨機応変にLINEの最新バージョンに対応します。
試験的なバージョンです、下記の機能には不具合が発生する場合があります。
(動的検出対応済み)
> メッセージを送信してから既読する
> チャットリスト関連(PIN機能、再表示無効化)
> ここに記載していない機能すべて

下記は動的検出に対応させていません。(機能名)
//既読確認機能の長押しでボタンを作成
//電話時に自動で着信拒否にする
//Original着信に変更
//トークのバックアップ、通知登録
//写真保存時の名前変更
//ボイス送信機能の無効化
///サブ端末で強制的にダークテーマに着せ替える

不具合が発生すれば、バグ報告でお知らせください



## 1.32.6.5beta

Merge pull request #24 from areteruhiro/areteruhiro-patch-22

Update NPatch + LSPatch.yml



## 1.32.6.5beta

LSpach/NPachでの生体情報の連携を可能にする機能オプションの追加
LIMEsのフォルダ選択ボタンをホームの
ヘッダーにも追加



## 1.32.6.4beta

Sign Fix
FCM fix



## 1.32.6.3beta

Sign Fix



## 1.32.6.2beta

FCM Hex



## 1.32.6.1.beta

removeAlbumの修正



## 1.32.6.alpha

LsPatxh/NPatxh　トークバックアップ/リストアを可能にする機能の追加
既読確認機能の新機能を追加オプションとして管理 <15.12.2のみ>
xiawanli の署名に対応



## 1.32.5.2.2.beta

RemoveNotification　の修正
Read Checker Fix Maybe



## 1.32.5.2.1.beta

revanced



## 1.32.5.1.beta

TokenGet署名 Npatchの対応



## 1.32.5.0.beta

グループ名を変更の改善　
https://discord.com/channels/1392057820316303362/1392059954260873286/1469199662761377832
handleInitPackageResourcesの改善
https://discord.com/channels/1392057820316303362/1392059954260873286/1469005857000788134
FCM TokenGet　Revanced対応
テーマファイルを復元するように
isDark処理を改善
https://discord.com/channels/1392057820316303362/1392059954260873286/1468939654664421461
ReadChecker　15.12.2のみ機能の改善(開発中)
https://discord.com/channels/1392057820316303362/1392834431617859634/1462427491997192233



## 1.32.3.3beta

fcm fix



## 1.32.3.3beta

Dark_Theme_Change機能の追加
Dark_Theme_Change機能の追加に基づくLIMEsのダーク/ライトの検知方法の変更
LYP プレミアムのおすすめを削除　機能の改善(Maybe need report)
更新されたプロフィールを削除　が機能していなかったのを修正



## 1.32.3.2beta

fix 内部ファイルコピー
Maybe ソニーランチャー未読数送信　機能 15.12.2 only



## 1.32.3_beta

fix PreventMarkAsRead_Setting strings.xml -ja
fix CreateMute



## 1.32.2_beta

add option call create mute 固定



## 1.32.1_beta

15.21.3 対応(仮)
fix local change name
add option call create mute
⚠Disable_chat_ui_ai_talk_suggestion 15.18.1のサポートを外して15.21.3に対応



## 1.31.25_beta

fix strings.xml
LocalGroupName Dark



## 1.31.24_beta

Add Call CreateMute
Fix PhotoSave Album
DARK→LIGHT　RAW
Add confirmation button
DisableNotificationAlbumAdd →NOTIFICATIONS　Category



## 1.31.24_alpha

Add Call CreateMute
Fix PhotoSave Album
DARK→LIGHT
Add confirmation button



## 1.31.24_alpha

Add Call CreateMute
Fix PhotoSave Album
DARK→LIGHT
Add confirmation button



## 1.31.23alpha

Reaction Picture icon



## 1.31.22alpha

moduleContext.getResources().getStringの共通呼び出し化,(English、台湾)
NotificationReactionに画像の追加
header →dark to light



## 1.31.21adwwsssalpha

強制的にダークテーマに着せ替える機能の追加(beta)
送信取り消しされたメッセージの通知メッセージの変更ボタンが追加されていなかったのを修正



## 1.31.21alpha

EmbedOptions Fix Crash



## 1.31.20alpha

local name fix chat only bottom

## 1.31.19 alpha
### LocalName機能の追加
- removeOptionがオンの場合Headerにも追加しないように変更
- LIMEs設定ボタンに説明の追加
- 「未読のまま閲覧」→送信後に既読に変更
- NotificationReaction → リアクションされた際に通知
- GroupNotification → グループ通知
- MediaReNameSave → 写真/動画保存時に名前を変更する
- ReactionCount → リアクションカウント
- StopCallTone → 発信音/着信音停止ボタンの作成
- MessageSend → メッセージ送信スケジュール機能

## 1.31.18 alpha
- EmbedOptionsのコメントの追加

## 1.31.17 alpha
### LimeOption 整理
- header_setting_light の追加

## 1.31.16 alpha
- EmbedOptionsにカテゴリ用オプションアクションボタンを追加

## 1.31.15 alpha
- PhotoSave fix cache
- LSPatch / NPatch 用に Xposed ログの current time を無効化
- ReadChecker 修正（LSPatch / NPatch）

## 1.31.14 alpha
- read_checker 修正

## 1.31.13 alpha
- PhotoSave 修正
- DisableNotificationAlbumAdd
- dark / light 追加
- TokenGet 無効化

## 1.31.12 alpha
- main hooks に TokenGet 追加
- DisableSilentMessage のログ無効化
- yml 修正（多分）

## 1.31.11 alpha
- build.gradle の更新

## 1.31.10 alpha
- Downgrade（true）

 
 \n
 
 ## 1.31.9_alphaDisable Notification add　Album
PhotoSave Rename Fix
header_setting_dark.png
header_setting_light.png add
TokenGet(At RISK)\n\n## 1.31.8_alpha
- Fix Reaction count Custom emoji
## 1.31.7_alpha
- EmbedOptionsテーマカラーの調整(お試し)
- 旧設定画面の削除

## 1.31.6_alpha
- yml修正

## v1.30.29alpha
- read data,reaction listのダークモード
- /Setting/Notification_Setting_False.txt が存在している場合全てを通知するように
- 戻るボタンを押した際にlimesボタンが作成されるのを修正

## v1.30.28alpha
- read check write fix
- WalleteRemoveLayout add
- notification fix

## v1.30.27alpha
- 既読者確認についてのクラッシュを修正しました。

## v1.30.26
- Notification Reaction Fix.

## v1.30.25
- fix db Crash option

## v1.30.24a
- CopyFileButtonの作成 
- drawable→rawを参照するように

## v1.30.22a
- Enable_Theme_Validation 機能  
  https://github.com/areteruhiro/LIMEs/issues/32

## v1.30.21a
- StopCallToneが無効時に有効になっていたのを修正

## v1.30.18α
- RemoveGcsLypRecommendの改善
- ボタンの位置を座標で指定できるように
- ボタンの設定を設定しやすいように

## v1.30.14beta
- RemoveGcsLypRecommend の修正
- keepUnreadの修正
- 既読確認機能のクラッシュ対策 Maybe
- SendEnterChange_InChat 機能の仕様変更 → 対応バージョンの制限がなくなりました
- ring機能のエラーを修正
- ReactionList_dbの画像化
- 通話音声系（LsPatch）の修正（切断時の音声を鳴らす機能をオプション化）
- support device dual app(Chat BackUp)
- Pached LINE 15.12.12 _armeabi-v7aに修正
- 主要なボタンを動的に場所を移動できるように変更

## v1.30.8alpha
- RemoveGcsLypRecommend の修正
- keepUnreadの修正
- 既読確認機能のクラッシュ対策 Maybe
- SendEnterChange_InChat 機能の仕様変更

## v1.13.6
- リアクションリストボタンのクラッシュ対策
- 既読データの削除機能の修正
- 主要なボタンを動的に場所を移動できるように変更
- 既読者確認機能のリバース
- チャット非表示機能のバグ修正

## v1.30.5
- 通話のEndtoneの追加
- リアクションリストButtonの追加

## v1.30.3
- 既読者確認についての最適化

## v1.30.1
- メディア保存時 Rename機能を修正
- MessageSend_intent機能の追加
- 参考: https://drive.usercontent.google.com/uc?id=1zB1LhH4YGo9AfeckbtSmxFnjxDfG_CqN&authuser=1&export=download
- SendMessageの保存ファイルを内部化
- 既読者確認データ削除ボタンの位置を動的に移動できるように

## v1.30.0
- 15.12.2対応

## v1.29.11
- chat_ui_square_ai_summary_button delete機能の追加

## v1.29.10
- PIN機能の調整

## v1.29.7
- 一部の端末でエラーが発生するため不必要な権限の削除
- 環境調整

## v1.29.6
- 予約送信機能重複対策
- リアクションカウント機能の強化
- ピン機能のバグの修正
- リアクション通知機能のnull対策
- SendEnterChange_InChat（15.11.2のみ）
- SendEnterChange_ChatListの追加
- minifyEnabled true
- shrinkResources true の適用

## v1.29.5
- MessageSend機能の追加
- https://t.me/LsPosedLIMEs/1649/7529 の修正適用
- 例の機能の修正

## v1.29.3beta
- SendEnterChange機能追加（長押しでボタンの位置を変更出来ます）
- ※15.11.2のみ対応: CallComing機能追加（通話開始時に、着信拒否になる、終わりに着信通知オンになります）自己責任でお願いします
- インテントバックアップのバグ修正
- 取り消しメッセージの改行対応
- URI削除機能
- リアクションNULLバグ修正

## 15.11.2 対応
- 1.28.6で見つかったバグの修正

## v1.28.6
- ReactionListの修正
- チャットリスト内でのAI削除機能
- en修正

## v1.28.5
- GetMidId 取得機能
- バックアップIntentの場所をuriの場所に変更
- デュアルアプリでlimesを開けないバグを修正
- RemoveVoiceRecordを15.9.xに対応
- Reaction Notificationのバグを修正?

## v1.28.4
- androidx.fragment.app.の複数バージョン対応
- ファイルを作成させるように内部ディレクトリ化

## v1.28.2
- リソース系のバグの修正

## v1.28.1alpha
- 設定ボタンの場所をラインラボに変更

## v1.28.0alpha
- 任意の場所に設定を保存できるように、クラス名変更（バックアップは以前のフォルダのまま）

## v1.25.25a
- 15.9.x対応、既読者確認機能のクラス名変更