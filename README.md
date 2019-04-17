# HomeWork-2

## 問題
### 冠狀動脈心臟疾病(coronary heart disease, CHD)風險預估

根據Prediction of Coronary Heart Disease Using Risk Factor Categories(Peter W. F. Wilson et al., 1998)這份研究論文指出的風險因子，
簡化後訂定出規則，並依此規則做出400筆數據，之後再實作決策樹並測試。

## 特徵

血壓：收縮壓(Systolic blood pressure)及舒張壓(Diastolic blood pressure)，mmHg。

總膽固醇(Total cholesterol)：mg/dL。

低密度脂蛋白(LDL)：mg/dL。

高密度脂蛋白(HDL)：mg/dL。

背景資料(background)：抽菸與否(smoking)、是否有糖尿病(diabetes)、是否有家族病史(family history)。1為true，0為false。

## 規則
![](https://imgur.com/HOzaw4g.png)

## Dataset
根據前述規則，共做出400筆資料，其中前300用來training，後100用來test。
而為了模擬較常遇到情形，所以training data中CHD的0與1的數據有unbalance的情形，也就是CHD=1的數量多於CHD=0的數量。
而在testing data中為了個直覺的看出預測錯誤的數據，因此全部都是CHD=0的數據。

如附檔，下圖為前五筆資料。CHD那欄為解答(1為高風險，0為低風險)。

![](https://imgur.com/NNNcjQA.png)

## 決策樹
![](https://imgur.com/Sph4Tny.png)

## 討論
可以看到經由training data所做出來的決策樹跟預設的規則相差甚多，而利用此決策樹針對test data作預測的準確度有0.78，也算差強人意。


