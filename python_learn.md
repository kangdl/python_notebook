#1、python 类
##1.1 作用域
##1.2 类
###1.2.1 类的定义
类定义的语法为：\
class class_name：\
&emsp; <statement-1>\
&emsp; ...\
&emsp; <statement-n>\

当进入类定义时，将创建一个新的命名空间，并将其用作局部作用域，
因此，所有对局部变量的赋值都是在这个新命名空间之内。 特别的，
函数定义会绑定到这里的新函数名称。
当（从结尾处）正常离开类定义时，将创建一个类对象。
###1.2.2类对象
类举例：
class my_class：\
“”“A simple example class”“” \
&emsp; i=12345 \
&emsp; def f(self): \
&emsp;&emsp;return 'hello class' \
**有效属性:**
有效的属性名称是类对象被创建时存在于类命名空间中的所有名称。
在类my_class中，my_class.i和my_class.f都是有效的属性引用，
将分别返回一个整数和一个函数对象。