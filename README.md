# HW2：Test-time Steering 的回顧與延伸

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shihhsinwang0214/test-time-steering-hw2/blob/main/hw2_steering.ipynb)

這次的作業是 Test-time Steering Lab 的延伸，繳交期限是兩週（以 NTU COOL 公告為準）。

程式的部分，只需要把你在 lab 寫的方法貼進 [`hw2_steering.ipynb`](hw2_steering.ipynb) 的 `my_method`，再從頭跑到尾（[在 Colab 開啟](https://colab.research.google.com/github/shihhsinwang0214/test-time-steering-hw2/blob/main/hw2_steering.ipynb)，CPU 大約幾分鐘就跑完）。大部分的時間會花在報告上，整份作業預計 1–3 小時可以完成。

在自己的電腦跑也可以（需要 `torch numpy pandas matplotlib`），notebook 第一格會自動從這個 repo 下載需要的模型和資料。

## 要做的事

1. 打開 notebook，把 lab 的方法貼進 `my_method`，照 lab 當時的做法就好，先不要改進。跑 Part A。
2. 用同一個 `my_method` 跑 Part B。Part B 換成另一個已經 train 好的模型。
3. 寫報告，回答下面的問題。每一題寫幾句話就可以。

## 報告的問題

### Part A：Lab 的 1D 題目

**A1.** 用生活直覺的方式，寫下你在 lab 裡用的方法。可以想像是在跟沒修這門課的朋友解釋，不用公式。

**A2.** 具體的 algorithm 是怎麼做的？每一步具體化了你一開始的什麼想法？

**A3.** 在目前的測資中，跑出來的結果怎麼樣？請附上 notebook 畫的圖（真實分布和你 sample 出來的點）與數字表。符合你的預期嗎？

**A4.** 可以說出哪裡不符合預期嗎？可以想像為什麼嗎？

### Part B：換一個模型

**B1.** 在 Part B 的測資中，跑出來的結果怎麼樣？一樣附上圖與數字表。符合你的預期嗎？如果方法要修改才能在 Part B 跑，也說明改了什麼、為什麼要改。

**B2.** 可以說出哪裡不符合預期嗎？可以想像為什麼嗎？

### 最後

**C.** 最後想一想，你覺得可能可以怎麼修改你的方法？不需要實作，有實作的話可以附上結果。

## 規則

- 模型參數不能動；交出去的點要是模型 sample 出來的，不能直接用參考樣本，也不能自己手動產生點。
- 每次產生 2,000 個點，NFE 不超過 1,000,000（notebook 會幫你算）。
- 可以和同學討論，但程式和報告請自己完成。有使用 AI 工具的話，請在報告最後說明怎麼用的。

## 繳交（NTU COOL）

1. `hw2_<學號>.ipynb`：跑完並保留輸出的 notebook。
2. `hw2_samples.npz`：notebook 最後一格會產生這個檔案。
3. `hw2_<學號>.pdf`：報告，大約 2 頁（不含圖）。

交完之後的下一次上課，會用大家的結果分組討論。上課前我會先用你的 notebook 重跑一次，再把結果寄給你。
