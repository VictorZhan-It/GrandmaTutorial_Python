[GrandmaCan: 4小時初學者Python教學]
---

[GrandmaCan: 4小時初學者Python教學]:https://www.youtube.com/watch?v=zdMUJJKFdsU

[>> Python基礎教程]

[>> Python基礎教程]:https://www.runoob.com/python/python-tutorial.html

大綱
- [GrandmaCan: 4小時初學者Python教學](#grandmacan-4小時初學者python教學)
  - [Python](#python)
  - [元組tuple (類似於列表List)](#元組tuple-類似於列表list)
  - [字典Dictionary](#字典dictionary)
  - [for 迴圈 (for與foreach結合為for迴圈)](#for-迴圈-for與foreach結合為for迴圈)
- [檔案讀寫](#檔案讀寫)
- [模組 Module](#模組-module)
- [類別Class與物件Object](#類別class與物件object)
- [其它](#其它)


### Python

---

+ 引入模組
  
  ```python
  from math import *
  ```

+ 不需要；符號做結束。
  
  ```python
  print("Hellow World")
  ```

+ 不需要宣告變數型態，直接給值即可。
  
  ```python
  name = "Victor"
  name = 100
  name = true
  ```

+ input("標題") 得到使用者的輸入值
  
  ```python
  name = input("請輸入名字：")
  print(name) 
  age = int(input("請輸入年齡："))
  print(age) 
  ```

[<< Top](#大綱)

<br/>

### 元組tuple (類似於列表List)
---
`創建後無法再新增、修改、刪除內容 (唯讀)`
+ 元組是防止資料被意外的修改
+ 元組是用小括號 ( ... )
+ 列表是用中括號 [ ... ]
+ 取值一樣用中括號 [ x ]
  
```python
scores = (90, 80, 70, 60)
print(scores[0])    #得90

len(scores)    #取得長度 = 4
```
[<< Top](#大綱)

<br/>

### 字典Dictionary
---
`鍵跟值的比對`

```python
dictionary = {"蘋果":"Apple", "香蕉":"Banana", "貓":"Cat"}

numDict = {0:"Apple", 1:"Banana", 2:"Cat"}

dictionary["香蕉"] #得Banana

numDict[2] #得Cat
```
[<< Top](#大綱)

<br/>

### for 迴圈 (for與foreach結合為for迴圈)

```python
for letter in "Hello World":
    print(letter)    #得每一個string

for num in [1, 2, 3, 4]
    print(num)    #得1到4

for num in range(4)    
    print(num)    #得1到4

for num in range(2, 7)    
    print(num)    #得2到7

#二維陣列
list = [
    [0,1,2],
    [3,4,5],
    [6,7,8],
    [9]
]
for row in list:
    for col in row:
        print (col)
#印出 0~9
```

[<< Top](#大綱)

<br/>

## [檔案讀寫](https://youtu.be/zdMUJJKFdsU?t=11421)

---

```python
#檔案開啟
file  = open( "路徑", mode = "開啟模式", encoding="utf-8")

...

file.close()
```

```python
#精簡寫法 ( 不需要file.close() )
with open( "路徑", mode = "開啟模式", encoding="utf-8") as file:
    ...
```


+ 路徑：相對 / 絕對路徑 `斜線"\\"需改為"/" `
+ mode
  + r：讀取
  
    ```python
    file = open("assets/123.txt", mode = "r", encoding="utf-8")
    
    #檔案讀取
    print(file.read())
    
    #檔案只讀取一行
    print(file.readline())
    
    #用迴圈印出每一行
    for line in file:
        print(line)
    
    #每一行資料放入陣列裡
    ary = file.readlines()    #得[A\n, B\n, C\n, D\n]
    
    #檔案關閉，釋放系統資源
    file.close()
    ```

  + w：覆寫整個檔案內容
  
    ```python
    file = open("assets/123.txt", mode = "w", encoding="utf-8")
    
    file.write("Hello")    #內容變 Hello
    
    #檔案關閉，釋放系統資源
    file.close()
    ```

  + a：在原先的資料後新增內容
  
    ```python
    file = open("assets/123.txt", mode = "a", encoding="utf-8")
    
    #檔案讀取
    print(file.read())
    
    file.write(" World")    #內容變 Hello World

    file.write("你好")
    
    #檔案關閉，釋放系統資源
    file.close()
    ```

[<< Top](#大綱)

<br/>

## [模組 Module](https://youtu.be/zdMUJJKFdsU?t=12269)
---

>引入其它py檔案，就可以使用檔案內的變數成員或函式。

```python
# tool.py
def LogMsg(msg):
    print("LogMsg: " + msg)
```

```python
# math.py
def GetRandMultiple(num):
    return rand() * num
```

```python
# main.py
import tool        # 引入tool.py模組
import math as mh  # 引入math.py模組並改名為mh

tool.LogMsg("Hello World")

value = mh.GetRandMultiple(10)
```

```python
import sys
print(sys.path)    #得到內建模組py檔的路徑 (lib資料夾)
```

pip套件管理系統

```python
#console裡鍵入
pip install {模組名稱}
```

[Python內建模組](https://docs.python.org/3/py-modindex.html)

[<< Top](#大綱)

<br/>

## [類別Class與物件Object](https://youtu.be/zdMUJJKFdsU?t=12894)

```python
#類別
class Character:
    def __init__(self, name, health, mana, isNPC)
        self.name = name
        self.health = health
        self.mana = mana
        self.isNPC = isNPC

#實例化
player = Character("Victor", 150, 60, false)
print(player.name)    #得到 Victor

npc = Character("Village", 30, 5, true)
print(npc.name)    #得到 Village
```

[<< Top](#大綱)

<br/>

## 其它

---

[>> 字串 string]

[>> 字串 string]:https://github.com/VictorZhan-It/GrandmaTutorial_Python/blob/master/string.md

[>> 數字 number]

[>> 數字 number]:https://github.com/VictorZhan-It/GrandmaTutorial_Python/blob/master/number.md

[>> 列表 list]

```python
 myList = ["Victor", 90, true]    #可存不同型態        
```

[>> 列表 list]:https://github.com/VictorZhan-It/GrandmaTutorial_Python/blob/master/list.md

[>> 函式 function]

[>> 函式 function]:https://github.com/VictorZhan-It/GrandmaTutorial_Python/blob/master/function.md

```python
def MyFunction(name, value):
    return name + "/" + str(value)

msg = MyFunction("Victor", 28)    #呼叫函式
```

[>> if 判斷句]

[>> if 判斷句]:https://github.com/VictorZhan-It/GrandmaTutorial_Python/blob/master/if_statements.md\

```python
if value > 0:
    print("A")
elif value != 0:
    print("B")
elif value < 0 and not(value<-10):
    print("C")
```

[>> while 迴圈]

[>> while 迴圈 ]:https://github.com/VictorZhan-It/GrandmaTutorial_Python/blob/master/while.md

```python
while value < 10:
    value += 1
```

[<< Top](#大綱)

<br/>