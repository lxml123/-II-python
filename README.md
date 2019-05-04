＃二级python须知 #P8

#33个保留字
and as assert await break class continue def 
del elif else except False finally for from global
if import in is lambda None nonlocal not or 
pass raise return Ture try while with yield

#引用程序调用以外库，一般用import保留字
 1.全命名引用
 import<库的名称>
 2.具体函数引用
 from<库名称>import<函数名称>
 3.全函数引用
 from<库名称>import *
 4.别名引用
 import<库名称>as<库名>
 
 #四种进制形式  以前面的符号为记
 十进制：生活中常用
 二进制：0b或0B
 八进制：0o或0O
 十六进制：0x或0X
 
 #数字运算、内置运算函数 P11
 x/y：就是数学运算
 x//y：取最大整数
 x%y:取余数 （也称模运算）
 abs(x) = 数学中的绝对值
 pow(x,y) = 数学中的幂运算
 pow(x,y,z) 先是幂运算再模运算
 
 
 #类型间的转换
 int（x）:x转换为整数，x可以是浮点数或字符串
 float（x）：X转换为浮点数，.....
 str(x):将X转换为字符串，.....
 chr(x):返回Unicode编码X对应的单字符
 str.lower（）：返回字符串的副本，全部小写
 
 
#程序异常处理框架
import requests
def grtHTMLText(url):
    try:
        r = requests.get(url,...)
        r.raise_for_status()
        r.encoding = r,appent_encoding
        return r.text
    except:
if_name_=='_main_':
        url = "......"
 
 
 ＃变量    P15
 局部变量指在函数内部使用的变量，仅在函数内部有效，当函数退出时变量将不再存在。
 全局变量指在函数之外定义的变量，在程序执行全过程有效。全局变量在函数内部使用时，需要提起使用保留字global声明.
 global<全局变量>
 
 
 #组合数据类型
 集合类型：一个元素集合，元素之间无序，各元素在集合中唯一存在。
 序列类型：一个元素向量，元素之间存在先后关系，通过序号访问，元素之间不排他。序列类型包括：字符串类型，元组类型，列表类型。
 映射类型：是'键-值'数据项的组合，每一个元素是一个键值对，表示为（key,value）。影视类型是典型的字典类型
 元组采用小括号（）表示，集合采用大括号{}表示，列表采用[]表示
 
 
 #列表的方法
 list(x):将x转换成列表类型
 ls.append(x):在列表后面增加一个元素x
 ls.insert(x):在列表ls第i位置增加元素x
 ls.pop(x):将ls中的i元素取出并删除
 ls.remove(x)：移除ls中的第一个元素
 ls.reverse（x）将ls反转
 
 
