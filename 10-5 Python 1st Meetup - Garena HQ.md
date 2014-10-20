10/5 Python 1st Meetup @ Garena HQ
投影片：https://speakerdeck.com/balicantayao/lab317-python-playground-week-1

環境建置
Windows
電腦右鍵內容→系統→進階系統設定→進階→環境變數→系統變數→Path→新增python安裝目錄(ex: C:\python27\)
TODO: wanshu516@gmail.com
解決encode error output is not utf-8的問題
Sublime Text2：Preferences→Browse Package→Python→在Python.sublime-build檔案中加入"encoding": "utf-8"，如下所示。
{
        "cmd": ["python", "-u", "$file"],
        "file_regex": "^[ ]*File \"(...*?)\", line ([0-9]*)",
        "selector": "source.python",
        "encoding": "utf-8"
}
Mac
抓好裝好結束
Linux
Coding Style
註解
#
無多行註解
變數
_分隔
    member_ary
function
    def get_kekewu_girlfriend(id):
參數不可加型別
    def get_kekewu_girlfriend(int id): (X)
以縮排代替括號
    def get_kekewu_girlfriend(id):
        return girlfriends_obj[id]
Head
使用utf-8編碼
# -*- coding: utf-8 -*-
TODO: Bustta Tsai
sublime text 自動為py開頭檔名加上head
Knowledge and tips
create a file with .py extension
執行
ctrl + b (cmd + b in mac) to build in Sublime Text
python abc.py under cmd terminal

Print
print "Hello World!"
print "中文"
加入 # -*- coding: utf-8 -*- 於檔案開頭

變數
first_string = "Hello"
sec_string = "World"
space_string = " "
my_string = first_string + space_string + sec_string
print my_string

format string
format_string = "input number %d in string" % 6
print format_string

#ignore data type
my_var = "six"
format_any_type = "with any type %r, %d" % (my_var, 6)
print format_any_type

function
def function_one(one):
  print "function one %d", one

function_one(555)    #function call must after the definition

#multiple parameter
def parameter_list(*para):
  print para
  print para[0]
  first_para, sec_para, third_para = para
  print sec_para

parameter_list("one", "two", "three")

swap
a = 10
b = 20

a, b = b, a
print a
print b

tuple
(a, b) = (b, a)     #swap
(first_para, sec_para, third_para) = para
TODO: Dino Lai
解釋 Tuple, Array, List 三個差別，ex: order, memory
