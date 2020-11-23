# 最終発表の目標

## ロボットアームと消毒スプレーによるうんこの消毒
### 動機
 <img src= "https://user-images.githubusercontent.com/72371336/99922881-2f6d1180-2d76-11eb-8f82-2cab2aff505c.png" width="400" >
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture1.png" width="400" >
 あ！うんこがいるよ！消毒しなきゃ！
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture2.png" width="400" >
 君こっち来いよ！
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture3.png" width="400" >
 これで清潔なうんこになるんだ…
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture4.png" width="400" >
 <img src= "https://github.com/RobotDesign3-Team4-2020/interim_report/blob/master/img/picture5.png" width="400" >
 わーい！綺麗になったよ！
 こうしてcrane-x7くんは清潔なうんこくんと仲良く暮らしましたとさ
 
### 何が面白いか
- うんこが消毒される

### 使用する道具
- crane_x7
- RealSense
- ubuntu18.04(WSL/Desktop)
  - Gazebo
  - rviz
- Inventor
- うんこ
- アルコールスプレー

### システム構成    

<img src= "https://user-images.githubusercontent.com/71888687/99880229-8fb86200-2c55-11eb-99f5-825373c5c5c0.png" width="400" >
 
### プログラム動作
1． RealSenseで座標を読み取りうんこを掴む  
2． スプレーの噴射口の下にうんこを移動する  
3． うんこを置く  
4． スプレーの上部にアームを移動させる  
5． 垂直に任意の高さまでアームを下げ,アルコールを噴射させる  

### タスク
1. RealSenseの使い方の学習 
2. 発表資料作成

### 想定される問題について

- アームの移動  
  - 実機と仮想空間で座標に差が生じる  
    - 開発をTAと連携できる時間外におこなうことですり合わせの時間を確保する  
- 実機で調整するのが難しい
 
### スケジュール/担当
| 内容 | git学習　最終発表資料の作成 | プログラムコードにRealSenseを組み込む|
| :--: | :-------------: | :-----------: |
| 担当 | [Mitsuike](https://github.com/SomaMitsuike), [Nakajima](https://github.com/Isamu-Nakajima)| [Ikeda](https://github.com/ikeda-hitomi), [Sakamoto](https://github.com/Sakamoto-Takaya), [Kamioka](https://github.com/rlove1023), [Shu](https://github.com/shukouki)|Isamu-Nakajima)|
| 期日 | 12/21 | 12/7 |

なお担当の作業が終わり次第,次に近い期日の作業を手伝うこととする

### チームアップから第一週目のやったこと
- 最終発表計画資料の作成
- RealSenseの学習
