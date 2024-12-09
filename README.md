## 執行方法：
1. 確保主辦方提供的訓練集和測試集都在。
2. 確保有按照 AICUP_PG_FINAL.ipynb 的順序執行，並在“接下來把 complete_Training_Data文件夾 輸入到微氣候數據處理程序 產出 CompleteAVG 和 CompleteIncompleteAVG 兩個文件夾”這行出現時把整合好儲存在 complete_Trainning_Data 文件夾的訓練集資料輸入到微氣候數據處理程序。
3. 確保 CompleteAVG 和 CompleteIncompleteAVG 兩個文件夾放在位置上。
4. 確保氣象局資料有在 data 文件夾裡（C0Z100 和 466990）。
5. 以上步驟所需的資料以及輸出皆已上傳到 github 上，因此可以直接到第六步。
6. 執行 AICUP_PG_FINAL.ipynb 檔案。

## 環境：
作業系統：Ubuntu 22.04.4 LTS（在Ubuntu裡使用anaconda建置環境）
程式語言：Python(3.9.18)
套件(函式庫)版本：依照github 上 的requirement.txt 安裝。
以下列出一些重要套件的版本：
keras==3.6.0
lightgbm==4.5.0
numpy==1.26.4
scikit-learn==1.5.2
tensorflow==2.17.0
xgboost==2.1.3
所使用的額外數據集——氣象局資料：
•	數據集來自Raingel的台灣歷史氣象觀測資料庫專案：https://github.com/Raingel/historical_weather。
o	他是將中央氣象局建置之氣象觀測站以及農委會之農業氣象觀測網的資料每一天更新到 data 文件夾裡。
o	其中每一小時能得到的資料類別和CODiS 氣候觀測資料查詢服務（https://codis.cwa.gov.tw/StationData）能查詢到的是一樣的。
o	由於作者是逐日更新，因此會有過去每天每小時的數據。
o	因此使用上述專案的資料比起 Codis 網站能省下逐日下載數據的麻煩。
o	使用了其中的兩個檔案：466990_2024.csv 和 C0Z100_2024.csv
