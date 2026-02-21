# LINEの通知が届かないバグの対処法

LSPatch環境でLIMEs適用時に通知が届かない場合の対処法です。

> [!IMPORTANT]
> 通知が来ないバグはFCM由来のため、LINEをReVancedでGmsCore対応をさせることで根本的に解決しました。 <br>

> [!NOTE]
> LSPatch環境でLINEにパッチを適用した際、  
> 通知が届かなくなる場合があります。 <br>
> そのバグを解決する手順です。

---
> 最新情報は[Discordサーバー](https://github.com/areteruhiro/LIMEs/tree/master?tab=readme-ov-file#%E3%82%B5%E3%83%9D%E3%83%BC%E3%83%88)に参加して受け取ってください。 <br>

## 事前準備

トークのバックアップ/リストアはこの適用では有効にされません

## 環境準備

## 自分でパッチを当てる場合

* Revancdをインストール
https://github.com/revanced/revanced-manager

* Original LINEのダウンロード
https://discord.com/channels/1392057820316303362/1474590111659331727/1474590232413208616

* 署名(bks) 　(配布済みパッチ済みから更新する場合)
https://mega.nz/file/HB1zzTKK#Wb3bjDPGujlyOQwT1BxKDn_RpTsTvbRq6eucDtbOwkw

以下どちらか一つをインストール

NPatch
* https://github.com/areteruhiro/NPatch/releases/

LsPatch
* https://github.com/JingMatrix/LSPatch

## パッチ済みを使う場合

* https://discord.com/channels/1392057820316303362/1469897969909240051/1469900201975218351

  15.12.2 /NPatch/ local/ revanced適用済み
　
> [!IMPORTANT]
> [この署名と異なる場合](https://discord.com/channels/1392057820316303362/1474586114844135474/1474586372684779542)はパッチ適用時にアンインストールを促される場合があります<br>
> 事前にバックアップを行うようにしてください。

---

## 手順1：LINEにRevancedパッチ導入

1.Revancedを開く
2.設定から、代替ソースを<br>
Patchの組織を"areteruhiro"
Pachesのソースを"line" に変更 <br>
3.パッチ選択の変更を許可に変更
4.パッチャー項目→アプリを選択→APKファイルを選択→先ほどダウンロードした"line-revanced_v15122-patches_v30-505-npatched.apkを"選択
5.GMS Core supportとLINE remove unsupported attrsを有効に→パッチを開始
6.左下の保存ボタンをクリックして、任意の場所に保存(わかり易い名前にしておくことをおすすめします))

## 手順2：LINEにNPach/LSpachの適用させる

＋ボタン→Storageからapkを選択→先ほど保存したapkをタッチ→パッチを開始

> [!NOTE]
> 「ローカル」　をおすすめします<br>
> LSPachからNPachに移行する場合　設定から"署名のキーストア"のキーストアファイルを　署名(bks)　を選択してください<br>
> パスワード "123456" <br>
> エイリアス "key0" <br>
> エイリアスのパスワード 123456" <br>

## 手順3：
1.Micro-Gを開きます
2.Googleアカウント二ログインします
3.Googleのデバイス登録を開き有効にします
4.Cloud Messagingを有効にします

## 手順4
1.NPach/LSpachを開き、モジュールのスコープでLIMEsを選択
2.LINEを開きます
3.その他→TokenGetを有効にして再起動
4.次回起動時にLIMEs : Sucess FCM　が表示されれば登録が完了です
> [!NOTE]
> "X.509 証明書のバイナリ(HEX)を入力してください。FCM登録で利用されます"が表示される場合自分で署名バイナリを入力する必要があります。
> URI先にある"lsposed_module.log.txt"ファイルからX.509 証明書のバイナリ(HEX)を探してください<br>

## クレジット
@areteruhiro <br>
@2ipper <br>
@masahiko_masahiko <br>
<br>
皆様、情報提供ありがとうございます！ <br>
<br>
出典: https://discord.com/channels/1392057820316303362/1453311780502765574 <br>
