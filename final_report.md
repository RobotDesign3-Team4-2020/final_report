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
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture6.png" width="400" >
 
### 何が面白い？  
- うんこが消毒される  
- うんこは消毒されるものなのか
- というか他のもの消毒したら実用的

### 使用した道具  
- crane_x7    
- ubuntu18.04(WSL/Desktop)  
  - Gazebo  
  - rviz  
- OpenCV  
- RealSense
- うんこのおもちゃ   
- 据え置き型アルコールスプレー
- マーカー(赤、黄色)

###  実行環境
- ubuntu18.04
- ROS Melodic Morenia

### 実機操作説明

#### モデル配置
- 用意するもの
  - うんこのおもちゃ
  - 市販の据え置き型アルコールスプレー  
<img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/img4.jpg" width="400">

- 配置方法

#### 実機の動かし方
[READMEに従ってください](https://github.com/RobotDesign3-Team4-2020/crane_x7_/blob/R.kamioka/README.md)

### プログラム説明
- test.cpp
  - RealSenseで黄色の長方形を検出
- red_seach.py
  - test.cppのデータを受け取り、crane_x7を動かす
  
詳しくは以下をご覧下さい。  
[コメント付きソースコード](https://github.com/RobotDesign3-Team4-2020/crane_x7_/blob/R.kamioka/crane_x7_examples/scripts/red_search.py)

### 実演動画

### 目標段階での開発スケジュール予定
| 内容 |ノズルを判別して回すノード | うんこを移動して消毒するノード | タオルで拭く動作 |最終発表の資料作成 |
| :--: | :-----------: | :-----------: |:-------------: |:-------------: |
| 担当 |[Ikeda](https://github.com/ikeda-hitomi), [Sakamoto](https://github.com/Sakamoto-Takaya), [Kamioka](https://github.com/rlove1023), [Shu](https://github.com/shukouki)| 左同 | [Mitsuike](https://github.com/SomaMitsuike), [Nakajima](https://github.com/Isamu-Nakajima) | 左同 |
| 期日 | 12/7 | 12/7 | 12/14 | 12/14 | 12/20|

### 実際の進捗

 

### 最終的に担当したもの及び活動場所
- [Ikeda](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/ikeda)
  - README作成
- [Kamioka](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/R.kamioka)
  - ノズルを判別して回すノード作成
  - README作成
- [Sakamoto](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/T.sakamoto)
  - 昨年のプログラムのLICENSE取得
  - README作成
- [Nakazima](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/dev/nakajima)
  - README作成
- [Mitsuike](https://github.com/RobotDesign3-Team4-2020/crane_x7_/tree/mitsuike)
  - README作成
- syu 
  - RealSense受け取り
  - 実機動作確認
  - README作成
  
- [その他](https://github.com/RobotDesign3-Team4-2020/final_report/tree/master)

### まとめ
- 環境構築に時間がかかり、各ノード作成に時間を割けなかった
- Github/slack/backlogなどのサービスをうまく利用できなかった
  - 各々の進捗を把握できなかった
- 作業量に偏りができてしまった
