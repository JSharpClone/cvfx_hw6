# CVFX HW6

```
Team #15
107062503 許博皓
107062513 鄭家鈞
107062566 黃鈺程
```

# Original Video
使用realsence RGB-D camera
![](https://i.imgur.com/bZwxGV5.png)

[VideoURL](https://drive.google.com/open?id=19mt-8dRRuxg5o_iATRKDyHof_RY6R5Sj)

# Results

## visual effects with ORB-SLAM2

### track points
需要更新相機參數，因為與原始repo的相機不同
![](https://i.imgur.com/mhSCIc6.png)

### result

## visual effects with Adobe After Effects
### track points
載入影片之後使用track camera產生track points
![](https://i.imgur.com/sKvtp7J.png)

### result
每3個track points 可以產生一個平面，可以在平面上生成想要的object，text object可以直接生成，另外有選擇null來放影片。而3D model的部分則是使用AE的plug-in, VIDEO COPILOT Element 3D, 並使用All3DP裡的Pokemon 3D model。
![](https://i.imgur.com/O1GlBmn.jpg)
[VideoURL](https://drive.google.com/open?id=1PCOtSMf9S2VvYhRYcMf3PMcs6NE5LhVq)

# Compare
從結果來看ORB-SLAM2取出來的點較多，After Effects較少。但以效果來說After Effects能做出的效果比較細緻，例如放大縮小、旋轉等。畢竟AE是一個產品，對於使用者來說相對較容易操作；另一方面，ORB-SLAM2依照取出來的points的positions來新增object，以text object來說其實只是有沒有寫code而已。
