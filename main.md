
# 第一題


```python
def reverse_str(text):
    result = ""
    for a in range(0,len(text)):
        result += text[len(text)-a-1]
    return result
```


```python
reverse_str("abcd")
```




    'dcba'



# 第二題


```python
import math
```


```python
def count_3_5(number):
    a = math.floor(number / 5)
    b = math.floor(number / 3)
    c = math.floor(number / 15)
    print(number-a-b+c+1)
```


```python
count_3_5(15)
```

    9


# 第三題
打開看了其中一個後，  
假設是寫鉛筆、但是是原子筆，則我們知道   
1) 該袋是原子筆 2) 寫混合那袋一定不是混合、也一定不是原子筆，則一定是鉛筆 3) 剩下那袋一定是混合  
以此類推  
  
  
  
抽象來說，打開其中一袋發現寫 A、但為 B，  
1. 該袋為 B
2. 寫 C 的那袋不為 C、也不為 B，則一定為 A
3. A, B 都知道了，則剩下那袋一定為 C

# 第四題
因為當把 3 人的 300 元減掉 30 元（服務生退給她們的錢）時，得到的是一個「有折扣」的價格 ; 此時如果把這個數字 * 3 再加上服務生拿走的錢，得到的數字自然會是「有折扣（雖然不是全部折扣，因為服務生拿走了一些）」的價格，而非「原先的 900 元」
