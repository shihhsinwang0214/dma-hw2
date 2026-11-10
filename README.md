# HW2：Test-time Steering 的回顧與延伸

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shihhsinwang0214/test-time-steering-hw2/blob/main/hw2_steering.ipynb)

這次的作業是 Test-time Steering Lab 的延伸，繳交期限是兩週（以 NTU COOL 公告為準）。

程式的部分，只需要把你在 lab 寫的方法貼進 [`hw2_steering.ipynb`](hw2_steering.ipynb) 的 `my_method`，再從頭跑到尾（[在 Colab 開啟](https://colab.research.google.com/github/shihhsinwang0214/test-time-steering-hw2/blob/main/hw2_steering.ipynb)，CPU 大約幾分鐘就跑完）。大部分的時間會花在報告上，整份作業預計 1–3 小時可以完成。

在自己的電腦跑也可以（需要 `torch numpy pandas matplotlib`），notebook 第一格會自動從這個 repo 下載需要的模型和資料。

## 要做的事

1. 打開 notebook，把 lab 的方法貼進 `my_method`，照 lab 當時的做法就好，不需要特別改進，直接跑 Part A (跟上課一樣的資料集)。
2. 用同一個 `my_method` 跑 Part B。Part B 換成另一個在較高維度的資料集上訓練好的模型。
3. 回答下面的問題，寫成一份 pdf(請搭配你用 ipynb 跑出來的圖)，每一題寫下幾句你的想法 (上課討論的時候會用到)。

## 報告的問題

### Part A：Lab 的 1D 題目

**A1.** 用生活直覺的方式，寫下你在 lab 裡使用的方法 （也就是這份作業的 my_method）。可以想像你要跟沒修這門課的朋友解釋，甚至是你最親愛的親人們，嘗試用最直白的方法來比喻說明。

**A2.** 具體的 algorithm 是怎麼做的？每一步具體化了你一開始的什麼想法？

**A3.** 在目前的測資(Part A)中，跑出來的結果怎麼樣？請附上 notebook 畫的圖（真實分布和你 sample 出來的點）與數字表。結果符合你的預期嗎？

**A4.** 可以說出哪裡不符合預期嗎？是因為什麼原因造成的？

### Part B：換一個較高維度的情況

**B1.** 在 Part B 的測資中，跑出來的結果怎麼樣？一樣附上圖與數字表。結果符合你的預期嗎？如果方法要修改才能在 Part B 跑，也說明改了什麼、為什麼要改。

**B2.** 可以說出哪裡不符合預期嗎？是因為什麼原因造成的？

### 最後

**C.** 最後想一想，你覺得可能可以怎麼修改你的方法？不要求要完成實作，如果有嘗試的話，可以將實作結果放在藍色框框下的位置。

## 規則

- 模型參數不能動；交出去的點要是模型 sample 出來的，不能直接用參考樣本，也不能自己手動產生點。
- 每次產生 2,000 個點，NFE 不超過 1,000,000（notebook 會幫你算）。
- 可以和同學討論，但程式和報告請自己完成。有使用 AI 工具的話，請在報告最後說明怎麼用的。

## 繳交（NTU COOL）

1. `hw2_<學號>.ipynb`：跑完並保留輸出的 notebook。
2. `hw2_samples.npz`：notebook 最後一格會產生這個檔案。
3. `hw2_<學號>.pdf`：報告，大約 2 頁（不含圖）。

交完之後的下一次上課，會用大家的結果分組討論。我極有可能會在上課前，再用你的 code 跑一些其他的benchmarks，再把結果寄給大家。
