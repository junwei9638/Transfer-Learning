# AI Object Recognition Web App

## Scenario

### What?
利用 **Azure** 架設網站，並使用 **AI 技術辨識與分類物體**。

### How?
使用 **OpenCV.js** 與 **KNN-Classifier**，讓使用者可以：

- 開啟視訊鏡頭並記錄要分類的物品。  
- 對輸入的物品取得特徵點並分類。  
- 將分類完成的物品移至畫面中，即可輕鬆辨識物體類別。  
- 自行增加物品分類及定義物品標籤。

網站透過 **Azure** 與 **Docker** 技術上架到網路上，使用者可直接線上使用上述功能。

## Techniques

**Programming Languages:**  
HTML, CSS, JavaScript

**Tools & Libraries:**  

- **OpenCV.js** 與 **KNN-Classifier**：進行圖像分類與辨識  
- **OpenSSL**：生成自簽 SSL Certificate  
- **Docker + Nginx**：將 Web Application 架設至 Azure Server
