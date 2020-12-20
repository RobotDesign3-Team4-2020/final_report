# 4班最終発表
##  ロボットアームと消毒スプレーによるうんこの消毒
### 動機
  <img src= "https://user-images.githubusercontent.com/72371336/99922881-2f6d1180-2d76-11eb-8f82-2cab2aff505c.png" width="400" >
 何か消毒するものないかなー
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture10.png" width="400" >
 あ！うんこだ！消毒しなきゃ！
  <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture11.png" width="400" >
  アルコールを探して...
  <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture12.png" width="400" >
 ノズルの向きを変えて！
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture2.png" width="400" >
 君こっち来いよ！
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture3.png" width="400" >
 これで清潔なうんこになるんだ…
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture4.png" width="400" >
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture5.png" width="400" >
 わーい！綺麗になったよ！
 こうしてcrane-x7くんは清潔なうんこくんと仲良く暮らしましたとさ
 
### 何が面白い？  
- うんこが消毒される  
- うんこの判別

### 使用した道具  
- crane_x7    
- ubuntu18.04(WSL/Desktop)  
  - Gazebo  
  - rviz  
- OpenCV  
- RealSense
- うんこのおもちゃ   
- 据え置き型アルコールスプレー
- 黄色のマーカー(折り紙を使用)

###  実行環境
- ubuntu18.04
- ROS Melodic Morenia

###  変更した点

### 実機操作説明

#### モデル配置
- 用意するもの
  - うんこのおもちゃ
  - 市販の据え置き型アルコールスプレー  
<img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/img4.jpg" width="400">

  アルコールスプレーのノズルには以下の画像のようにマーカーを付けます
  
<img src="https://user-images.githubusercontent.com/70384485/102332471-76de6a80-3fcf-11eb-9a8e-3b5462a1ad7b.png" width="400px">

- 配置方法
<img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/img5.png" width="400">  
<img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/img2.jpg" width="400">  

#### 実機の動かし方
[READMEに従ってください](https://github.com/RobotDesign3-Team4-2020/crane_x7_/blob/R.kamioka/README.md)

### プログラム説明
- test.cpp
  - RealSenseで黄色の長方形/💩を検出
- red_seach.py
  - test.cppのデータを受け取り、座標へ変換後、💩をアルコールの前まで動かす一連の動作
  
詳しくは以下をご覧下さい。  
[コメント付きソースコード](https://github.com/RobotDesign3-Team4-2020/crane_x7_/blob/R.kamioka/crane_x7_examples/scripts/red_search.py)

### 実演動画
[![](http://img.youtube.com/vi/XUe6zGDWI2U/0.jpg)](http://www.youtube.com/watch?v=XUe6zGDWI2U "実演動画１")

　↑画像をクリックすると動画が再生されます

[![](http://img.youtube.com/vi/HD80IjuEiw4/0.jpg)](http://www.youtube.com/watch?v=HD80IjuEiw4 "実演動画２")

　↑画像をクリックすると動画が再生されます

### 目標段階での開発スケジュール予定
| 内容 |ノズルを判別して回すノード | うんこを移動して消毒するノード | タオルで拭く動作 |最終発表の資料作成 |
| :--: | :-----------: | :-----------: |:-------------: |:-------------: |
| 担当 |[Ikeda](https://github.com/ikeda-hitomi), [Sakamoto](https://github.com/Sakamoto-Takaya), [Kamioka](https://github.com/rlove1023), [Shu](https://github.com/shukouki)| 左同 | [Mitsuike](https://github.com/SomaMitsuike), [Nakajima](https://github.com/Isamu-Nakajima) | 左同 |
| 期日 | 12/7 | 12/7 | 12/14 | 12/14 | 12/20|

### 実際の進捗
　- アルコールのノズルの角度の認識
  - ウンコの位置の認識
  - ウンコをノズルの先に移動させる動作
  - アルコールボトルのボタンをプッシュする動作
 

### 最終的に担当したもの及び活動場所
- [池田](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/ikeda)
  - README作成
  - コードにコメント追加、インデント修正
  - コードの体裁の調整
- [上岡](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/R.kamioka)
  - README作成
  - コード作成
  - 実機動作確認・調整
- [坂本](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/T.sakamoto)
  - 昨年のプログラムのLICENSE取得
  - realsenseの使い方調査
  - 会議の段取りや話の進行
  - cmakelistへの変更、c++のコンパイル、実行方法の確認
- [中島](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/dev/nakajima)
  - 情報収集
- [三ツ池](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/mitsuike)
  - README作成
  - 使えそうな関数の調査
- [朱](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/R.kamioka)
  - README作成
  - realsenseの使い方調査
  - 実機動作確認・調整
  - 動画撮影
  - 買い物
  
- [その他](https://github.com/RobotDesign3-Team4-2020/final_report/tree/master)

### まとめ
- 目標であったウンコの消毒には成功した
- 追加でウンコの位置も認識させることができた
- 環境構築に時間がかかり、各ノード作成に時間を割けなかった
- Github/slack/backlogなどのサービスをうまく利用できなかった
  - 各々の進捗を把握できなかった
