# NVIDIA Jetson Orin Nano 感測器影像調適繁中教學站

把 Jetson Orin Nano 上的 sensor 影像調適（Argus/V4L2 堆疊 / GMSL serdes / NVIDIA ISP / 影像品質調校）做成**中英對照**的 16 單元分層教學，以 OmniVision OV9281 / OV5640 為主要實例。

- 目標讀者：相機 / 影像 / AI 邊緣工程師、學生
- 單元數：16（含 5 個影像調校專章 + 跨平台比較）
- 授權：本站內容 CC-BY-4.0
- 網站：https://shumingyang-opencode.github.io/jetson-orin-nano-sensor-isp-zh-tw/

## 單元一覽

| # | 單元 | 內容 |
|---|------|------|
| 01 | 平台相機生態總覽 | CSI/GMSL、Argus/V4L2 |
| 02 | 影像感測器基礎 | Bayer、global shutter |
| 03 | 感測器通訊介面 | I2C/SCCB、register |
| 04 | 相機框架與驅動 | tegracam、DTB overlay |
| 05 | 第一個鏡頭跑起來 | argus_camera / v4l2-ctl |
| 06 | Sensor Bring-up 與除錯 | serdes、register dump |
| 07 | ISP 管線深入 | libnvivp、ISP 區塊 |
| 08 | RAW 擷取與資料格式 | RAW、bayer、Argus raw |
| 09 | 各平台 ISP 架構差異 | NVIDIA vs 其他 |
| 10 | 曝光與自動曝光（AE） | Argus 曝光控制 |
| 11 | 白平衡與色彩（AWB/CCM） | NVIDIA AWB/CCM |
| 12 | 鏡頭陰影校正（LSC） | NVIDIA LSC |
| 13 | 雜訊與降噪 | NVIDIA NR |
| 14 | 清晰度/HDR/調校工作流 | NVIDIA tuning 流程 |
| 15 | 四平台影像調校比較 | Orin Nano 視角 |
| 16 | 多感測器與實作案例 | GMSL 多相機 |

## 開發

純靜態 HTML，無建置步驟。

```sh
python3 -m http.server 8000 -d .
```

## 相關連結

- 學習路徑建議服務：[learning-path-advisor](https://shuming-yang.github.io/learning-path-advisor/) — 依角色推薦教學網站學習路徑
