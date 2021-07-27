# 詳細
桃鈴ねね非公式ファンサイトに掲載する情報をTwitter、YouTubeAPIを使用して取得するためのツールです。
[![Image from Gyazo](https://i.gyazo.com/e3fb4785ae9d6d44915d68cf513f4b81.jpg)](https://gyazo.com/e3fb4785ae9d6d44915d68cf513f4b81)
[![Image from Gyazo](https://i.gyazo.com/82380d58d8fbb4fda1fcff3a928029e3.jpg)](https://gyazo.com/82380d58d8fbb4fda1fcff3a928029e3)

https://konnene-matanene.herokuapp.com/

Archives、Clips、FanArtsページに掲載している情報を取得しています。

## 開発環境

ー Python
ー GoogleColaboratory

## 機能

### アーカイブ情報の取得

[![Image from Gyazo](https://i.gyazo.com/fbb6c410379826b42831ea96849b2ada.png)](https://gyazo.com/fbb6c410379826b42831ea96849b2ada)

YouTubeAPIを使用して、「Nene Ch.桃鈴ねね」のID、動画タイトル、再生数、投稿日時を取得しています。
該当チャンネル
https://www.youtube.com/channel/UCAWSyEs_Io8MtpY3m-zqILA

取得したIDを元に、URLとサムネイルURLを作成して、データフレームに変換しております。
nenechannelget.pyを実行

### 切り抜き動画情報の取得

[![Image from Gyazo](https://i.gyazo.com/3a169de56f89d7a41cdfc70e4628c099.png)](https://gyazo.com/3a169de56f89d7a41cdfc70e4628c099)

YouTubeAPIを使用して、「桃鈴ねね」「切り抜き」で検索をして、動画ID、動画タイトル、再生数、投稿日時を取得しています。
再生数と投稿日時を基準に取得しています。

取得したIDを元にURLとサムネイルURLを作成して、データフレームに変換しております。
nenechannelget.pyを実行

### ファンアート情報の取得

[![Image from Gyazo](https://i.gyazo.com/3d316180f54c675f8b64614d4ea9067d.png)](https://gyazo.com/3d316180f54c675f8b64614d4ea9067d)

TwitterAPIを使用して、「#ねねアルバム」というハッシュタグがついたツイートのIDとユーザー名を取得しています。
(#ねねアルバムはファンアートで非公式で桃鈴ねねさんの絵を書いた方が絵を投稿する際に使用するハッシュタグです。)
