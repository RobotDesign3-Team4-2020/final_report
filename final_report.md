# 4班最終発表

##  目標
- realsenseの画像認識を用いてウンコを探し、ノズルを回転させて消毒する


## 問題点と修正
- ノズルを回転させる場合アームに負担がかかる
　　→ノズルの先端を画像認識で探させて、そこへウンコを運び消毒する
  
<img src="https://github.com/RobotDesign3-Team4-2020/final_report/blob/master/%E7%84%A1%E9%A1%8C%E3%81%AE%E3%83%97%E3%83%AC%E3%82%BC%E3%83%B3%E3%83%86%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%20(3).png" width="400">
<img src="https://github.com/RobotDesign3-Team4-2020/final_report/blob/master/%E7%84%A1%E9%A1%8C%E3%81%AE%E3%83%97%E3%83%AC%E3%82%BC%E3%83%B3%E3%83%86%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%20(4).png" width="400">



## 環境構築
### 必要な道具
- crane_x7    
- RealSense
- うんこのおもちゃ   
- 据え置き型アルコールスプレー
- 黄色のマーカー(折り紙を使用)

###  実行環境
- ubuntu18.04(WSL/Desktop)  
  - Gazebo  
  - rviz  
- OpenCV 
- ROS Melodic Morenia

### モデル配置
- 用意するもの
  - うんこのおもちゃ
  - 市販の据え置き型アルコールスプレー  
<img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/img4.jpg" width="400">

  アルコールスプレーのノズルには以下の画像のようにマーカーを付けます
  
<img src="https://user-images.githubusercontent.com/70384485/102332471-76de6a80-3fcf-11eb-9a8e-3b5462a1ad7b.png" width="400px">

- 配置方法
<img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/img5.png" width="400">  
<img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/img2.jpg" width="400">  

## 実機の動かし方

[READMEに従ってください](https://github.com/RobotDesign3-Team4-2020/crane_x7_/blob/R.kamioka/README.md)

## プログラム説明
- test.cpp
  - RealSenseで黄色の長方形/💩を検出
  
<img src="https://github.com/RobotDesign3-Team4-2020/final_report/blob/master/%E7%84%A1%E9%A1%8C%E3%81%AE%E3%83%97%E3%83%AC%E3%82%BC%E3%83%B3%E3%83%86%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%20(6).png" width="600">

- red_seach.py
  - test.cppのデータを受け取り、座標へ変換後、💩をアルコールの前まで動かす一連の動作
  
詳しくは以下をご覧下さい。  
[コメント付きソースコード](https://github.com/RobotDesign3-Team4-2020/crane_x7_/blob/R.kamioka/crane_x7_examples/scripts/red_search.py)

## 実演動画
[![](http://img.youtube.com/vi/XUe6zGDWI2U/0.jpg)](http://www.youtube.com/watch?v=XUe6zGDWI2U "実演動画１")

　↑画像をクリックすると動画が再生されます

[![](http://img.youtube.com/vi/HD80IjuEiw4/0.jpg)](http://www.youtube.com/watch?v=HD80IjuEiw4 "実演動画２")

　↑画像をクリックすると動画が再生されます

## 作業フローと分担
### 目標段階での開発スケジュール予定
| 内容 |ノズルを判別して回すノード | うんこを移動して消毒するノード | タオルで拭く動作 |最終発表の資料作成 |
| :--: | :-----------: | :-----------: |:-------------: |:-------------: |
| 担当 |[Ikeda](https://github.com/ikeda-hitomi), [Sakamoto](https://github.com/Sakamoto-Takaya), [Kamioka](https://github.com/rlove1023), [Shu](https://github.com/shukouki)| 左同 | [Mitsuike](https://github.com/SomaMitsuike), [Nakajima](https://github.com/Isamu-Nakajima) | 左同 |
| 期日 | 12/7 | 12/7 | 12/14 | 12/14 | 12/20|
  
<img src= "https://user-images.githubusercontent.com/71888687/102723088-1cd00300-4349-11eb-8ec0-9ca0031f6488.png" width="800" >
  

### 最終的に担当したもの及び活動場所
- [池田](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/ikeda)
  - README作成
  - コードにコメント追加、インデント修正
  - コードの体裁の調整
  - 使えそうな関数の調査
  - 情報収集
- [上岡](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/R.kamioka)
  - README作成
  - コード作成
  - 実機動作確認・調整
  - 使えそうな関数の調査
  - 情報収集
- [坂本](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/T.sakamoto)
  - 昨年のプログラムのLICENSE取得
  - realsenseの使い方調査
  - 使えそうな関数の調査
  - 情報収集
  - 会議の段取りや話の進行
  - cmakelistへの変更、c++のコンパイル、実行方法の確認
- [中島](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/dev/nakajima)
  - 情報収集
- [三ツ池](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/mitsuike)
  - README作成
  - 使えそうな関数の調査
  - 情報収集
  - Backlogの管理
- [朱](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/R.kamioka)
  - README作成
  - realsenseの使い方調査
  - 使えそうな関数の調査
  - 実機動作確認・調整
  - 動画撮影
  - 買い物
  - 情報収集
  
- [資料作成](https://github.com/RobotDesign3-Team4-2020/final_report/tree/master)

## まとめ
- 目標であったウンコの消毒には成功した
- 追加でウンコの位置も認識させることができた
- 環境構築に時間がかかり、各ノード作成に時間を割けなかった
- Github/slack/backlogなどのサービスをうまく利用できなかった
  - 各々の進捗を把握できなかった

### 参考
中間発表について
- [目標記載ページ](https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/target.md)
- [目標リポジトリ](https://github.com/RobotDesign3-Team4-2020/crane_x7_ros.git)  
- [発表資料](https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/interim_report.md)

最終発表について
- [目標記載ページ](https://github.com/RobotDesign3-Team4-2020/final_report/blob/master/target.md)
