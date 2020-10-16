# 1.Python 模組(Module)
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
# 導|載入模組
import support
 
# 現在可以調用模組裡包含的函數了
support.print_func("MyFriends")
```
## support.py
```
def print_func( par ):
   print("Hello : ", par)
   return
```

# 2.撰寫一個Python套件(package|包)
```
my_module:
包含底下程式
__init__.py
Nice_to_meet_you.py
support.py
```
### Nice_to_meet_you.py
```
def Nice_to_meet_you( par ):
   print("Hello : ", par," ! Nice to meet you! ")
   return
```
###
```
上傳檔案到google drive
將google drive mount到Colab 
執行底下程式
```

```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
# 導|載入模組
import my_module.Nice_to_meet_you as haha2
 
# 現在可以調用模組裡包含的函數了
haha2.Nice_to_meet_you("MyFriends")
```

```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
# 導|載入模組
import my_module.support as haha
 
# 現在可以調用模組裡包含的函數了
haha.print_func("MyFriends")
```
