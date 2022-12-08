### 列表 list
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

+ extend() 兩個列表相連接
  ```python
    scores = [1,2,3]
    words = ["a","b","c"]

    print(scores.extend(words))    #得[1,2,3,"a","b","c"]
  ```

+ append() 列表後加值
  ```python
    scores = [1,2,3]
    print(scores.append("ABC"))    #得[1,2,3,"ABC"]
  ```

+ insert() 指定位置加入值
  ```python
    scores = [1,2,3]
    print(scores.instert(2, "ABC"))    #得[1,2,"ABC",3]
  ```

+ remove() 將指定值刪掉
  ```python
    scores = [1,2,3]
    print(scores.remove(2))    #得[1,3]
  ```

+ pop() 將最後一位移除
  ```python
    scores = [1,2,3]
    print(scores.pop())    #得[1,2]
  ```

+ sort() 將列表做由小到大的排序(升冪排序)
  ```python
    scores = [3,1,2]
    print(scores.sort())    #得[1,2,3]
  ```

+ reverse() 將列表排序反轉(降冪排序)
  ```python
    scores = [3,1,2]
    print(scores.reverse())    #得[2,1,3]
  ```

+ index() 取得指定值的位址
  ```python
    scores = [3,1,2]
    print(scores.index(2))    #得2
  ```

+ count() 計算列表中有幾個指定值
  ```python
    scores = [30,10,20,30]
    print(scores.count(30))    #得2
  ```

+ clear() 清空列表 
  
[<< Back to ReadMe.md]

[<< Back to ReadMe.md]:https://github.com/VictorZhan-It/GrandmaTutorial_Python#Python