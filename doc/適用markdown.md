# 文件主題
## 大章節
### 小節
### 小節
## 大章節

這是一段文字。

這是另一段文字。

- 安裝 ROS 2
- 啟動 Micro XRCE-DDS Agent
* 測試 topic

1. 先開 PX4 SITL
2. 再開 Agent
3. 最後啟動 ROS 2 node

- 測試項目
  - topic 是否存在
  - setpoint 是否持續發布
  - offboard 是否成功切換

**重要**

*補充說明*

***非常重要***

目前問題不是 ROS 2 topic 本身，而是 **offboard 切換條件未滿足**。

請檢查 `ros2 topic list` 的輸出。

```python
def main():
    print("hello")
```

> (引用) PX4 在進入 offboard mode 前，通常需要先持續收到 setpoint。

[PX4 官方文件](https://docs.px4.io/)

![圖片說明](image.png)

![系統架構圖](figures/system_architecture.png)
docs/
├─ figures/
├─ devlog/
└─ test-results/

---
分隔號

| 項目 | 狀態 | 備註 |
|---|---|---|
| ROS 2 安裝 | 完成 | Jazzy |
| XRCE Agent | 完成 | 可啟動 |
| Offboard 切換 | 失敗 | 還要檢查條件 |

- [x] 安裝 ROS 2
- [x] 啟動 PX4 SITL
- [ ] 測試 offboard mode
- [ ] 驗證實機連線

升力可寫成 $L=\frac{1}{2}\rho V^2 S C_L$

$$
L=\frac{1}{2}\rho V^2 S C_L
$$