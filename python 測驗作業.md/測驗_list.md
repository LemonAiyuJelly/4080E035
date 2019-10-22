# Python小測驗2.md

### list資料型態

```
很像陣列(array)的list(清單|列表)
x = [11, 22, 33,44,55]

但list可以儲存不同資料型態的元素
x = [6, "Dragon", [10, 21, 32]]
```
### List 的indices(索引)
```
 若x = ["first", "second", "third", "fourth"]
 則下列分別為何?哪一個會出錯?
 ```
 ```
 x[1]
 ```
 'second'
 ```
 ```
 x[3]
 ```
 ```
 'fourth'
 ```
 ```
 x[5]
 ```
 ```
 ---------------------------------------------------------------------------
IndexError                                Traceback (most recent call last)
<ipython-input-56-585a9828f882> in <module>()
      1 x = ["first", "second", "third", "fourth"]
----> 2 x[5]
      3 

IndexError: list index out of range
```
```
 x[-1]
 ```
 ```
 'fourth'
 ```
 ```
 x[-2]
```
```
'third'
```
```
 x[1:3]
 ```
 ```
 ['second', 'third']
 ```
 ```
 x[:3]
 ```
 ```
 ['first', 'second', 'third']
 ```
 ```
 x[1:-1]
 ```
 ```
 ['second', 'third']
 ```
 ```
 x[:]
```
```
['first', 'second', 'third', 'fourth']
```


### enumerate() 函數
```
enumerate() 函數用於將一個可遍歷的資料物件(如清單、元組或字串)組合為一個索引序列，同時列出資料和資料下標
一般用在 for 迴圈當中。
Python 2.3. 以上版本可用，2.6 版本添加 start 參數。

函數語法: enumerate(sequence, [start=0])

參數說明：sequence -- 一個序列、反覆運算器或其他支援反覆運算物件。 start -- 下標起始位置。

返回值:返回 enumerate(枚舉) 物件(object, instance)
```
```
底下程式輸出結果為何?
seasons = ['Spring', 'Summer', 'Fall', 'Winter']
list(enumerate(seasons))
list(enumerate(seasons, start=11))    


len(seasons)
```
```
4
```
```
i = 0
seq = ['one', 'two', 'three']

for element in seq:
       print(i, seq[i])
       i +=1
```
```
0 one
1 two
2 three
```
```
seq = ['one', 'two', 'three']
enumerate(seq)

seq = ['one', 'two', 'three']
list(enumerate(seq))
```
```
[(0, 'one'), (1, 'two'), (2, 'three')]
```
```
seq = ['one', 'two', 'three']
for i, element in enumerate(seq):
     print(i, element)
```
```
0 one
1 two
2 three
```
