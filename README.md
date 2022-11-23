# [GrandmaCan: 4小時初學者Python教學]

[GrandmaCan: 4小時初學者Python教學]:https://www.youtube.com/watch?v=zdMUJJKFdsU



### Python
---

+ 引入模組
  ```python
  from math import *
  ```

+ 不需要；符號做結束。
  ```python
  print("Hellow World)
  ```

+ 不需要宣告變數型態，直接給值即可。
  
  ```python
  name = "Victor"
  name = 100
  name = true
  ```

### 字串 string
---

+ 用"\n"進行換行
  ```python
    print("Hello\n world")
  ```

+ 用"印出雙引號
  ```python
    print("\"Hello\" world")
  ```

+ 字串轉成小寫
  ```python
    name.lower()
  ```

+ 字串轉成大寫
  ```python
    name.upper()
  ```

+ 取得指定位置的字串
  ```python
    name[0] #第0位的string
  ```

+ 取得指定字串的位置
  ```python
    name.index("V") #字串V在第幾位
  ```

+ 替換指定字串
  ```python
    name.replace("H", "A") #將字串H替換成字串A
  ```

### 數字 number
---
+ 四捨五入至個位數
  ```python
    round(8/5) #得2
  ``` 

+ 無條件捨去小數點
  ```python
    print(8//5) #得1
  ``` 

+ 用%取餘數
  ```python
    print(8%5) #得3
  ``` 

+ 用str()將數值轉成字串
  ```python
    value = 100
    str(value) #得"100"

    #字串與數值不得直接相加
  ``` 

+ 用abs()取絕對值
  ```python
    abs(-8) #得8
  ``` 

+ 用pow()取次方值
  ```python
    pow(2, 4) #2的4次方得16
  ``` 

+ 用max()取最大值
  ```python
    max(2, 4, 5, 7, 10) #得10
  ``` 

+ 用min()取最小值
  ```python
    min(2, 4, 5, 7, 10) #得2
  ``` 

+ **需要import math模組**
    + 無條件捨去小數點()
        ```python
        floor(4.6) # 得4
        ```

    + 無條件進位至個位數()
        ```python
        ceil(4.1) # 得5
        ```

    + 開根號()
        ```python
        sqrt(36) # 得6
        ```

### 基本計算機
---

+ input()得到使用者的輸入值"字串"
  ```python
  name = input("請輸入名字：")
  print(name) 
  age = input("請輸入年齡：")
  print(age) 
  ```

+ int()將字串轉換成整數
  ```python
  int("100") #得100
  ```

+ float()將字串轉換成浮點數
  ```python
  float("13.5") #得13.5
  ```

### 列表list
---
```python
scores = [100, 34, 60, 80, 49]
name = ["Victor", "Avrial", "Peter"]

#可以儲存多個不同型的的值
combine = ["Victor", 90, true]
```
+ 取得指定位置的值
  ```python
    # 從index:1開始取值，取到index:3
    scores[1:4]    #得34, 60, 80
  ```


