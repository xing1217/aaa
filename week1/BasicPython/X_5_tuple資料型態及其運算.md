#
```
[1]元組(tuple)資料型態
[2]元組(tuple)的各種運算
  建立tuple
  使用索引(index)存取tuple元素
  使用for 迴圈存取tuple的每一個元素

[3]tuple內建函數：
　　count()	
　　index()
```
# tuple
```
A tuple is a collection which is ordered and unchangeable

tuple創建很簡單，只需要在括弧中添加元素，並使用逗號隔開即可。

tup1 = ('python', 'linux', 1997, 2020)
tup2 = (1, 2, 3, 4, 5 )
tup3 = "a", "b", "c", "d"
```
```
Python的元組與列表類似，不同之處在於元組的元素不能修改。

tuple使用小括弧，列表使用方括號。
```
# 
### 使用索引(index)存取tuple元素
```
tup1 = ('python', 'linux', 1997, 2020)
tup2 = (1, 2, 3, 4, 5 )
tup3 = "a", "b", "c", "d"
tup1[3]
tup2[1]
tup3[3]
```
### 使用for 迴圈存取tuple的每一個元素
```
thistuple = ("apple", "banana", "cherry")
for x in thistuple:
  print(x)
```
### 元組的元素不能修改|刪除元素==>這是甚麼意思?
```
thistuple = ("apple", "banana", "cherry")
thistuple[3] = "orange" 
print(thistuple)
```
### 元組的元素不能修改==>如何硬改??
```
x = ("apple", "banana", "cherry")
y = list(x)
y[1] = "kiwi"
x = tuple(y)

print(x)
```
### 加法運算
```
tuple1 = ("a", "b" , "c")
tuple2 = (1, 2, 3)

tuple3 = tuple1 + tuple2
print(tuple3)
```
# [3]tuple內建函數：
```
　　count()	
　　index()
 
1	cmp(tuple1, tuple2) 比較兩個元組元素。
2	len(tuple)計算元組元素個數。
3	max(tuple)返回元組中元素最大值。
4	min(tuple)返回元組中元素最小值。
5	tuple(seq)將列表轉換為元組。
```
```
tu1 = (123, ‘Teacher‘, ‘School‘, ‘Teacher‘, 123, ‘Teacher‘, ‘School‘, ‘Teacher‘, ‘School‘)
tu2 = (777, ‘iPhone‘, ‘Apple‘, ‘iPhone‘, 101, ‘Teacher‘, ‘School‘, ‘Apple‘, ‘Google‘)

print ("123 元素的個數 : ", tu1.count(123))
print ("Teacher 元素的個數 : ", tu1.count(‘Teacher‘))
print (tu1.cmp(tu1,tu2))
```
