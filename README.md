# Teachable-Machine-Example
Google Teachable Machineを活用した簡単な例題です。

## Google Teachable Machineとは何ですか？
Teachable Machine は、誰でも短時間で簡単に機械学習モデルを作成できる、ウェブベースのツールです。

## 学習データは何ですか?
[こちら](https://lttm.dei.unipd.it/downloads/gesture/#kinect_leap)です。  
データから4人が11個の手ポーズをします。  
S1/S2/S3/S4 (4人)  
G1/G2/G3/G4/G5/G6/G7/G8/G9/G10/G11 (11個の手ポーズ)  

## 学習方法
S1のデータを活用して11個の手ポーズ（各30枚のpng）を学習しました。

## 学習結果
![image](https://media.discordapp.net/attachments/793673760242008124/793674287528542248/sample.png?width=950&height=356)  
(左:学習した写真S1/右:確認する写真S3)  

S3の各1枚目の写真を入力し、類似度を確認しました。  
Google Teachable Machaineですぐに確認でき、コードと学習モデルをダウンロードして確認することができます。  
S3のG1 : 68%  (正確)  
S3のG2 : 0.2% (不正確)

## コードの使い方
- `numpy`, `tenserflow`, `pillow` をインストールしてください。
- `test_photo.png`を同一フォルダに入れてください。
- `python3 gtm.py`を実行してください。

