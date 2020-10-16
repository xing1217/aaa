

# 使用CSV套件
```
https://docs.python.org/3/library/csv.html
```
```
# ! /usr/bin/python
# -*- coding: utf-8 -*-

from __future__ import print_function
import csv

# 7.1.2
with open('csv_tutorial.csv', 'a') as fw:
    writer = csv.writer(fw)
    writer.writerow(["c1", 'c2', 'c3'])
    for x in range(10):
        writer.writerow([x, chr(ord('a') + x), 'abc'])
```
```
cat csv_tutorial.csv
```
```
# ! /usr/bin/python
# -*- coding: utf-8 -*-

from __future__ import print_function
import csv

# 7.1.1
with open('csv_tutorial.csv', 'r') as fr:
    rows = csv.reader(fr)

    for row in rows:
        print(row)
```
```
Python 讀取與寫入 CSV 檔案教學與範例
https://blog.gtwang.org/programming/python-csv-file-reading-and-writing-tutorial/
```
