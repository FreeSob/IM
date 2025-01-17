# **Qt期末專題初步構想書：Qt 互動遊戲「你畫我猜」**

---
## **組員**

- 50915109 莊捷森
- 50915110 陳霑汶
- 50915133 陳有臨

---

## **專案名稱**
你畫我猜（Qt 互動 AI 遊戲）

---

## **專案背景與目標**
### **背景**  
「你畫我猜」是基於圖像辨識的互動遊戲，靈感來源於 Google 的 Quick, Draw!。結合 Qt 平台與 AI 模型，開發一個可以進行即時圖像辨識的互動遊戲。

![image](https://github.com/user-attachments/assets/5c916ff0-a69d-47b3-97e0-5517a7675687)


### **目標**  
利用 Qt 的跨平台特性，實現一個結合畫布繪製與 AI 圖像分類的桌面應用程式。

---

## **核心功能**
1. **玩家繪圖功能**  
   - 提供一個畫布，允許玩家用滑鼠繪製圖像。
   - 支援清除畫布功能，便於重新繪製。
2. **AI 辨識功能**  
   - 使用預先訓練的模型（如 Quick, Draw! 的 `cat` 和 `dog` 模型）。
   - 當玩家完成繪圖後，將圖像傳送至 AI 模型進行分類，並返回結果。
3. **遊戲互動**  
   - 隨機生成題目，玩家需要繪製符合題目的圖案。
   - 顯示 AI 判斷結果，並根據正確與否提供反饋。


---

## **技術架構**
1. **前端：Qt
   - 使用 **QPainter** 提供畫布繪圖功能。
   - 界面元素使用 Qt Designer 設計，包括按鈕、標籤等。
2. **AI 模型**  
   - 使用 TensorFlow 訓練的分類模型（例如 `cat` 和 `dog`）。
3. **整合**  
   - 畫布數據轉換為二進制或圖片格式（如 PNG）。
   - 使用 HTTP 或文件共享方式將畫布數據傳送至 AI 推理模組。
4. **後端推理**  
   - 運行 Python (或javascript)的 AI 推理程式，回傳分類結果至 Qt 應用程式。

---

## **界面設計**
1. **主畫面**
   - 畫布區域：中心提供繪圖畫布。
   - 文字區域：顯示當前題目（如「請畫一隻貓」）。
   - 按鈕：包括「清除畫布」與「提交答案」。
2. **結果頁面**
   - 顯示 AI 辨識結果（正確或錯誤）。
   - 提供下一題按鈕。

---


## **開發工具**
1. **開發環境**  
   - Qt Creator 和 Visual Studio Code
2. **程式語言**  
   - C++（Qt Widgets） 或 Python 或 javascript
3. **AI 模型訓練與推理**  
   - Python (TensorFlow)
4. **版本控制**  
   - GitHub

---

## **預期成果**
 一個完整的「你畫我猜」桌面遊戲，支援即時圖像辨識。


---

https://github.com/jasonch15/Qt_quickdraw
