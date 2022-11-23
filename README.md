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


[字串 string]

[字串 string]:https://github.com/VictorZhan-It/GrandmaTutorial_Python/blob/master/string.md


<details>
<summary>字串 string</summary>

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

[<<TOP](#Python)

</details>

<details>
<summary>數字 number</summary>

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


 + int()將字串轉換成整數
    ```python
    int("100") #得100
    ```

+ float()將字串轉換成浮點數
  ```python
  float("13.5") #得13.5
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
    
    + input()得到使用者的輸入值"字串"
      ```python
      name = input("請輸入名字：")
      print(name) 
      age = input("請輸入年齡：")
      print(age) 
      ```

[<<TOP](#Python)
    
</details>

<details>
<summary>列表 list</summary>

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

+ 取得指定位置之後的所有值
  ```python
    # 從index:1開始取值
    scores[1:]    #得34, 60, 80, 49
  ```

+ 取得指定位置之前的所有值
  ```python
    # 從index:4開始取前面的值
    scores[:4]    #得100, 34, 60, 80
  ```

+ extend()兩個列表相連接
  ```python
    scores = [1,2,3]
    words = ["a","b","c"]

    print(scores.extend(words))    #得[1,2,3,"a","b","c"]
  ```

+ append()列表後加值
  ```python
    scores = [1,2,3]
    print(scores.append("ABC"))    #得[1,2,3,"ABC"]
  ```

+ insert()指定位置加入值
  ```python
    scores = [1,2,3]
    print(scores.instert(2, "ABC"))    #得[1,2,"ABC",3]
  ```

+ remove()將指定值刪掉
  ```python
    scores = [1,2,3]
    print(scores.remove(2))    #得[1,3]
  ```

+ pop()將最後一位移除
  ```python
    scores = [1,2,3]
    print(scores.pop())    #得[1,2]
  ```

+ sort()將列表做由小到大的排序
  ```python
    scores = [3,1,2]
    print(scores.sort())    #得[1,2,3]
  ```

+ reverse()將列表排序反轉
  ```python
    scores = [3,1,2]
    print(scores.reverse())    #得[2,1,3]
  ```

+ index()取得指定值的index
  ```python
    scores = [3,1,2]
    print(scores.index(2))    #得2
  ```

+ count()計算列表中有幾個指定值
  ```python
    scores = [30,10,20,30]
    print(scores.count(30))    #得2
  ```

[<<TOP](#Python)

</details>


### 元組tuple
---