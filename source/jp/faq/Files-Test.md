---
title: 7番目のベイの使用
description:
type: “Docs”
tip: 上部の固定フォーマットを削除しないでください。descriptionは記事の説明であり、記入しない場合は内容の最初の段落を切り取ります。
---
# 7番目のベイの取り付けと取り外し
## 準備:
ZimaCubeの電源がオフで、プラグが抜かれていることを確認してください。
取り付けるハードドライブを準備します。
## 具体的な手順:
ステップ1: ケースのフロントパネルを取り外します。
![](https://manage.icewhale.io/api/static/docs/1722418820491_image.png)
ステップ2: 6番目のベイを取り外します。
![](https://manage.icewhale.io/api/static/docs/1722418858886_image.png)
ステップ3: 反時計回りに回して、7番目のドライブを固定しているネジを外します。
![](https://manage.icewhale.io/api/static/docs/1722418913222_image.png)
ステップ4: 7番目のベイを取り外します。
![](https://manage.icewhale.io/api/static/docs/1722418964759_image.png)
![](https://manage.icewhale.io/api/static/docs/1722418974044_image.png)
ステップ5: SSDを7番目のベイに自由に取り付けます。
![](https://manage.icewhale.io/api/static/docs/1722419028169_image.png)
ステップ6: 7番目のベイを正しい位置に押し込み、ネジを時計回りに締めます。
![](https://manage.icewhale.io/api/static/docs/1722419069919_image.png)

# ZimaCube 7番目のライトファームウェアをアップグレードする方法
*ESP32がOTA（Over-The-Air）アップデートで失敗するのを防ぐために、有線アップデート方法をここで紹介します。*
## 3ステップの解決策
1. WiFiに接続
コンピュータでWiFiに接続します
名前: "ZimaCube"
パスワード: "homecloud"
2. URLを入力
ブラウザに入力: 172.16.1.1
3. ファームウェアをアップロード
[https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link](https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link)

## バックアッププラン

**アップデート前の準備**
- コンピュータ
- タイプCデータケーブル
- ディスク 7
- 圧縮パッケージをダウンロードして解凍
[https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link](https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link)

**アップデートの開始**
3.1 タイプCデータケーブルを使用して、コンピュータを7番のディスクのチップのタイプCに接続します。
3.2 コンピュータでリンク[espressif.github.io](espressif.github.io)を開きます。
3.3 '接続'をクリックします。
![](https://manage.icewhale.io/api/static/docs/1730360675989_image.png)

3.4 接続するシリアルポートを選択します。
![](https://manage.icewhale.io/api/static/docs/1730360689217_image.png)

3.5 'DIY'をクリックします。
![](https://manage.icewhale.io/api/static/docs/1730360715808_image.png)

3.6 'ファイルを追加'を2回クリックします。
![](https://manage.icewhale.io/api/static/docs/1730360989529_image.png)

3.7 書き込みアドレスを変更し、ファイルを選択します。
*具体的な書き込みアドレスは図のように、解凍後に順番に3つのファイルを選択します。*
![](https://manage.icewhale.io/api/static/docs/1730360997291_image.png)

3.8 'プログラム'をクリックして書き込みを開始します。
![](https://manage.icewhale.io/api/static/docs/1730361017895_image.png)

3.9 書き込みが完了したら、RSTリセットボタンを押して、ファームウェアが正常に更新されます。