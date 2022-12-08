# 函式 Function
---
>一段預先寫好的程式碼區段，需要它的時後才會呼叫它並且執行程式碼內容。

```python
def Hello(userName, age):
    print("Hello " + userName + "/" + str(age) + "歲")

Hello("Victor", 28)    #呼叫函式    
```

```python
def Add(num1, num2):
    return num1 + num2

total = Add(5, 15)    #得total = 20
```

```python
def Add(num1, num2):
    return None    #當沒有return時，系統預設會自動添加None

total = Add(5, 15)    #得total = None
```

[<< Back to ReadMe.md]

[<< Back to ReadMe.md]:https://github.com/VictorZhan-It/GrandmaTutorial_Python#Python