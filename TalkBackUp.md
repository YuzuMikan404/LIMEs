# トークのバックアップ復元方法

手順は2つあります。

1. [**作成済みプロジェクトを利用する**](https://discord.com/channels/1392057820316303362/1472210371501625477/1474411172664185025)
2. **自分でプロジェクトを作成する**（以下、詳細手順）

---

## 利用するサイト

- [Google Cloud Console](https://console.cloud.google.com/enable-mfa?redirectTo=%2F)
- [OAuth 2.0 Playground](https://developers.google.com/oauthplayground)

---

## 自分でプロジェクトを作成する手順

- [Google Cloud Console](https://console.cloud.google.com/enable-mfa?redirectTo=%2F)　にアクセス

### 1. プロジェクトの作成

プロジェクトを選択画面で「新しいプロジェクト」をクリックします。

<img src="https://github.com/user-attachments/assets/319c74f4-9c15-42ae-979c-288f8ae06b2f" width="600" alt="エラー画面" />
*このエラーが発生する場合は手順に従って有効にしてください。*

プロジェクトの選択画面：

<img src="https://github.com/user-attachments/assets/5eb91585-08a8-43c7-929d-a27f79b7691a" width="600" alt="プロジェクト選択" />

新しいプロジェクト作成：

<img src="https://github.com/user-attachments/assets/14bba63d-4183-4ef3-9987-a9fdf37da0f2" width="600" alt="新しいプロジェクト" />

プロジェクト名を記入して作成：

<img src="https://github.com/user-attachments/assets/f137ae12-45e3-447e-890f-20d3723e7048" width="600" alt="プロジェクト名入力" />

### 2. Google Drive API の有効化

「APIとサービス」 > 「ライブラリ」 で Google Drive API を有効にします。

<img src="https://github.com/user-attachments/assets/6c4f42f5-0ab5-4a25-818b-0ada663d3548" width="600" alt="APIとサービスライブラリ" />

「APIとサービスを有効にする」をクリック：

<img src="https://github.com/user-attachments/assets/f2713d3b-3991-4d8e-b532-0fecd4113930" width="600" alt="API有効化" />

「Google Drive API」を選択：

<img src="https://github.com/user-attachments/assets/479ef737-41e8-4c4c-a439-ae4732ad12db" width="600" alt="Google Drive API選択" />

「有効にする」をクリック：

<img src="https://github.com/user-attachments/assets/bc711f32-0892-4b87-a50b-bbea0eb90096" width="600" alt="有効化ボタン" />

### 3. OAuth同意画面の設定

「OAuth同意画面」を設定し、ユーザータイプを「外部」にします。

<img src="https://github.com/user-attachments/assets/d17fa100-8472-4be9-a0c4-f5ef0657520a" width="600" alt="OAuth同意画面" />

### 4. OAuthクライアントIDの作成

「Googleクライアントを作成」をクリック：

<img src="https://github.com/user-attachments/assets/c70203fd-39ef-40b6-b193-0016690c11b8" width="600" alt="クライアント作成" />

承認済みのリダイレクトURLに `https://developers.google.com/oauthplayground` を追加します。

<img src="https://github.com/user-attachments/assets/4182910c-6218-49d1-87d5-c7327ab663d9" width="600" alt="リダイレクトURL設定" />

「認証情報」 > 「認証情報を作成」 > 「OAuthクライアントID」 で 「ウェブアプリケーション」 を選択し、クライアントIDとシークレットを控えます。

<img src="https://github.com/user-attachments/assets/f6830920-97d3-415f-b808-4b6fc2c2f87f" width="600" alt="クライアントID作成" />

### 5. OAuth 2.0 Playground での設定 {#oauth-playground}
- [OAuth 2.0 Playground](https://developers.google.com/oauthplayground)にアクセス
<img src="https://github.com/user-attachments/assets/b1db5935-8ee1-486e-ba27-75806a76a7ef" width="600" alt="本番環境プッシュ" />

右上の設定マークをクリックし、取得したクライアントIDとシークレットを入力します。


<img src="https://github.com/user-attachments/assets/6a268d92-fdc2-44d0-9ae0-f371ab66490c" width="600" alt="設定入力" />

Drive APIのスコープを選択します（例：`https://www.googleapis.com/auth/drive` など）。

<img src="https://github.com/user-attachments/assets/ab5ae17e-4702-4aa4-ae67-6ba38d96d788" width="600" alt="スコープ選択" />

青いボタン「Authorize APIs」を押します。

<img src="https://github.com/user-attachments/assets/ce1e5741-1d24-48ef-abda-573fb19896f9" width="600" alt="認証ボタン" />

アカウントを選択：

<img src="https://github.com/user-attachments/assets/2089e44f-c368-4882-9ab8-06284fa9f052" width="600" alt="アカウント選択" />

ログイン（必要な場合）：

<img src="https://github.com/user-attachments/assets/8bb36289-382e-47eb-ad66-281d4628b51a" width="600" alt="ログイン画面" />

許可：

<img src="https://github.com/user-attachments/assets/12b6a80d-39a9-4754-b7a4-0e7fe9ff6b78" width="600" alt="許可画面" />

### 6. リフレッシュトークンの取得

認証が完了すると、以下のような画面が表示されます。ここに表示される**リフレッシュトークン**をコピーして保存してください。

<img src="https://github.com/user-attachments/assets/eeabcac7-38da-4b86-9d61-8d327fa649ef" width="400" alt="リフレッシュトークン表示" />

詳細画面：

<img src="https://github.com/user-attachments/assets/a90203ba-5ca1-473c-8780-2e668651dc96" width="600" alt="トークン詳細" />

以上で、リフレッシュトークンの取得が完了です。このトークンを使ってバックアップの復元処理を実行できます。
