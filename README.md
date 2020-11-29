# 最終発表の目標

## ロボットアームと消毒スプレーによるうんこの消毒
### 動機
 <img src= "https://user-images.githubusercontent.com/72371336/99922881-2f6d1180-2d76-11eb-8f82-2cab2aff505c.png" width="400" >
 何か消毒するものないかなー
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture10.png" width="400" >
 あ！うんこだ！消毒しなきゃ！
  <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture11.png" width="400" >
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
 
 ### 前回の反省を活かして 

- メンバー間の連絡の取り合いが不足したことでそれぞれが担当するタスク量に差が生まれた   
       ⇨ 話し合いを密に行い報告を欠かさず行う,Backlogをこれまで以上に活用する  
- ハンドを消毒するべきでは？  
       ⇨ タオルでハンドを拭く動作を追加する 
- 去年の画像認識から発展してない  
       ⇨スプレーのノズルを認識してうんこがある方向に回転させる 
       
### 何が面白いか
- うんこが消毒される
- うんこの判別

### 使用する道具
- crane_x7
- RealSense
- ubuntu18.04(WSL/Desktop)
  - Gazebo
  - rviz
- Inventor
- うんこ
- アルコールスプレー 


### 画像認識の方法    



 
### プログラム動作
1． Realsenseでアルコールボトルを見つけてボトルの中心座標を測定//RealSenseで座標を読み取りうんこを掴む  
2． アームでノズルが右を向くようにする//スプレーの隣（テープを張った場所）にうんこを移動する  
3． Realsenseによりうんこ捜索  
4． 先ほどの座標を参考にボトルの横にうんこを置く  
5． スプレーの上部にアームを移動させる  
6． アルコールを噴射させる     
ex) タオルでハンドを拭く

### 想定される問題について
  
- 画像認識の調整が難しい  
　　 ⇨ 去年の資料を読み込んで理解を深める
- 実機で調整するのが難しい  
 　　⇨ 早めにコードを書き換えてTAと連絡を取り合い実機で調整する回数を増やす

### タスク
1.　Realsenseにimageを受け取りデータとして送るノードの作成  
2.　うんこを認識するノードの作成  
3.　うんこを移動して消毒するノードの作成  
4.　タオルで拭く動作の作成  
5.　最終発表の資料作成  

 
### スケジュール/担当
| 内容 |Realsenseにimageを受け取りデータとして送るノード | うんこを認識するノード | うんこを移動して消毒するノード | タオルで拭く動作 |最終発表の資料作成 |
| :--: | :-----------: |:-------------: | :-----------: |:-------------: |:-------------: |
| 担当 |[Ikeda](https://github.com/ikeda-hitomi), [Sakamoto](https://github.com/Sakamoto-Takaya), [Kamioka](https://github.com/rlove1023), [Shu](https://github.com/shukouki)| 左同 |左同 | [Mitsuike](https://github.com/SomaMitsuike), [Nakajima](https://github.com/Isamu-Nakajima) | 左同 |
| 期日 | 11/30 | 11/30 | 12/7 | 12/7 | 12/20|

なお担当の作業が終わり次第,次に近い期日の作業を手伝うこととする

### チームアップから第一週目のやったこと
- 最終発表計画資料の作成
- RealSenseの学習
