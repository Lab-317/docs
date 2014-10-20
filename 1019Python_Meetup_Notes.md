#Boolean, captical with upper-case
``` python
myBool = True or False
print myBool
```

#range vs. xrange
``` python
print range(1, 10, 2)
print xrange(1, 1000000000) #use for big numerous range
```

#if statement
``` python
var_for_if = 6
if var_for_if > 5:
  print "Statement 1"
elif var_for_if < 3:
  print "Statement 2"
else:
  print "Statement 3"
```

#list and join
``` python
my_list = ["aaa", "bbb", "ccc"]
print ",".join(my_list)

list_part = my_list[1: 2]
print list_part

my_obj = {"one": "one1", "two": "two2", "three": "three3"}
print my_obj.get("one")
print my_obj["two"]
print my_obj.get("undefined", "this key is undefined")  #second para as default value
```

#module
 * 同資料夾下
``` python dir\aaa.py
def print_in_aaa(from_file_name):
  print "print_in_aaa {0}".format(from_file_name)
```
``` python dir\bbb.py
import aaa
print aaa.print_in_aaa()
```

 * 不同資料夾
``` python differentDir\aaa.py
def print_in_aaa(from_file_name):
  print "print_in_aaa {0}".format(from_file_name)
```
``` python dir\bbb.py
from differentDir import aaa
print aaa.print_in_aaa()
```

#Class

 * 一般宣告與使用
``` python HomeClassFile.py
  class Home(object):
    def __init__(self, arg):  #constructor
      super(Home, self).__init__()
      self.var_in_class = arg

  my_home = Home("home@Taipei")
  print my_home.var_in_class
```

* 使用其他.py的Class
``` python notHome.py
from HomeClassFile import Home
#或
from HomeClassFile import *
```