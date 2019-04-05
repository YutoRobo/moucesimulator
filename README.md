# moucesimulator

ROSが動作する環境で使用してください

操作方法
1: MouceSimulatorを開く
2: ROS上で
    roslaunch rosbridge_server rosbridge_websocket.launch
   コマンドを起動
3: MouceSimulator上で、白いブロックをクリックすると赤く色が変わる
    使いたいブロックを赤くしておく
4: Enterキーを押すと白いブロックが消滅する
5: 右上のテキストボックスにros側のURLを記述する
    UbuntuでMouceSimulatorを使用している場合、
    ws://localhost:9090
    を記述すればよい
6: ros側から、geometry_msgs::Vector3型の/cmd_velに対して、.xに左側モータの速度[deg/s]、.yに右側モータの速度[deg/s]を入れて送信すると動く
