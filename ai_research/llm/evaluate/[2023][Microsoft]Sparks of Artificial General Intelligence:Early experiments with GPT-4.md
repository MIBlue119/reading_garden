# [2023][Microsoft]Sparks of Artificial General Intelligence:Early experiments with GPT-4
- Ref: https://arxiv.org/pdf/2303.12712.pdf

人類與AGI的第一次接觸？

微軟研究團隊在GPT-4開發階段就先開始研究他的潛力。這篇通過幾個面向(Coding/數學能力/工具使用/2d,3d,GUI生成/反向工程)，並以ChatGPT以及GPT-4的比較，來評量GPT-4的Intelligence，並覺得GPT-4的能力往AGI邁進了一大步。

- GPT-4在開發優化的過程中畫獨角獸的能力進步XDD
- GPT-4通過Leetcode上的mock technical interview，可以聘請他當軟體工程師
- 具備常識來推理
    - 範例問題：一個獵人向南走一英里，向東走英里，向北走一英里，最後回到起點。獵人看到一隻熊並射殺他。熊是什麼顏色？
    - GPT-4可以基於常識推估那邊是北極，並且再基於北極得出有北極熊，因此熊應該是白色。而chatGPT是躺平放棄。
- 可以解讀assembly code
    - 微軟示範了用在把一個需要密碼的執行檔透過lldb取得的訊息，經由GPT-4的輔助來找出可以繞過密碼檢測漏洞的方式。
- AGI compiler: 可以執行 pseudo code，展現GPT-4在理解程式與執行正確的能力，同時也代表我們未來有能力進展到透過自然語言直接來寫程式
- pre-alignment前的模型，具備強大的錯誤訊息生產能力。微軟他們示範讓GPT-4生成說服父母不要讓小孩打疫苗的企劃，並且可以指定目標族群(生活在加州追求健康飲食的媽媽們)，以及設定結論(導到相信會造成自閉症)

但為什麼基於gradient descent,大規模的transformer以及超大量的資料就能讓他有這樣的intelligence，也是尚待探究的問題。


![](https://i.imgur.com/NVPuaAd.png)
![](https://i.imgur.com/DQ779y5.png)
![](https://i.imgur.com/ORo9mx7.jpg)
![](https://i.imgur.com/HQaBol3.png)
![](https://i.imgur.com/CPjhTxq.png)
![](https://i.imgur.com/oHy35ij.png)
![](https://i.imgur.com/U7wMV83.png)
![](https://i.imgur.com/zSo7cFL.png)
