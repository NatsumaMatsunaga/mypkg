# mypkg
 * このリポジトリはROS2のパッケージである。

 ## ノード
  * talker.py
   * パブリッシャを担うノードであり、数字をカウントしトピック/countupを通じてlistener.pyに送信する。
   
 * listener.py
   * サブスクライバを担うノードであり、トピック/countupからメッセージをもらい、talker.pyがカウントした数字を表示する。
 
 
 ## 実行方法
 * 端末を二つ開く
   * 端末1
   
      `` $ ros2 run mypkg talker ``
     
   * 端末2
   
      `` $ ros2 run mypkg listener ``
     
 * 実行例
 ``` 
 [INFO] [1672248072.470772772] [listener]: Listen: 57 
 [INFO] [1672248072.970641864] [listener]: Listen: 58 
 [INFO] [1672248073.470732241] [listener]: Listen: 59  
 [INFO] [1672248073.970678738] [listener]: Listen: 60     
 [INFO] [1672248074.471214290] [listener]: Listen: 61 
 ・・・
 ```
 
 ## 必要なソフトウェア
 * テスト済み: Python 3.7~3.10
 
 ## テスト環境
 * Ubuntu 20.04.5 LTS
 
 ## LICENSE
 * このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
 * © 2022 Ryuichi Ueda
