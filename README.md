![image](https://github.com/Robotics-Aerial-Robots/Homework7/blob/master/Figures/LOGO%20%E4%B8%AD%E8%8B%B1%E6%96%87%E6%A9%AB.png)
# 108 年度 機器人學：多軸旋翼機 

### HW7
Deadline: 4/13
---
## 題目
請實踐從continuous-time的state space轉換到discrete-time的形式 \
作法可使用數值積分的方式實現，積分得出狀態後  \
因此能繪出 位置-時間圖 (可使用rqt_plot 或 PlotJuggler)
### 指令
```
	roscore
	rosrun HW7 hw7
	rosbag record -O hw7 /Position/data
	-------after recording------------------
	rosrun plotjuggler PlotJuggler
	(之後點file,Load data,點選你的bag file)
```
### hw7.cpp

輸入 ``u`` 為unit step 訊號(力)
輸出 ``y``(量測訊號) 為 位移
<img src="https://github.com/Robotics-Aerial-Robots/Homework7/blob/master/Figures/%E8%AA%AA%E6%98%8E.PNG" width="80%" height="40%">

\ ${x(k+1)}= {x(k)} + \dot{x}$ ${dt}$ \
使用上述形式可實作到你的code
### PlotJuggler
下載網址:https://github.com/facontidavide/PlotJuggler \
及操作

### 作業上傳
除了上傳作業的cpp檔外，先錄好bag, \
開啟PlotJuggler, 點選你的bag file \
用Kazam或其他可以錄螢幕畫面的軟體紀錄你的**動畫**, \
,**並將你的動畫影片連結附在你的Readme.md** \
**或gif檔都可以** \
<img src="https://github.com/Robotics-Aerial-Robots/Homework7/blob/master/Figures/plot.PNG" width="80%" height="40%">


