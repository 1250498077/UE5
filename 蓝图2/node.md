











# 蓝图注释右键即可
![alt text](image.png)



# 修改细节
![alt text](image-1.png)


# 按住c也可以创建command，好像要按住鼠标左键还是右键



# 给创建的节点输入一个文本，执行的时候会经过
![alt text](image-2.png)



# 颜色分类
事件总是表示为红色
![alt text](image-3.png)

这是宏
![alt text](image-4.png)

多通道
![alt text](image-5.png)


get函数
![alt text](image-6.png)




# 不同蓝图的私有变量
子蓝图和其他蓝图都不就可获取别的蓝图的私有变量

![alt text](image-7.png)

如果是公有的。子蓝图可以直接获取。兄弟蓝图可以先获取蓝图实例，再获取变量
![alt text](image-8.png)

子蓝图使用父级变量直接用
![alt text](image-9.png)




# 如何暴露蓝图给外面的细节面板  
重点要勾选下方，每个变量都要勾选
![alt text](image-13.png)
也可以给变量加一个类别
![alt text](image-12.png)
![alt text](image-10.png)







# 通过蓝图在场景中动态生成actor
 
打开我们的关卡蓝图  
![alt text](image-14.png)  
这个方法允许我们在场景中动态生成actor    
![alt text](image-15.png)  

搜索我们的蓝图  
![alt text](image-16.png)  
创建一个变量定义我们生成的位置  
![alt text](image-18.png)  
生成之后可以在这里看到它  
![alt text](image-17.png)  



# 数组

创建变量并修改成数组
![alt text](image-19.png)
不断的创建元素
![alt text](image-20.png)




# 从数组中获取元素

数组拉出来
![alt text](image-21.png)

动态根据下标获取元素当中的元素
![alt text](image-22.png)




# 04 在数组中寻找项目

根据内容去检索
![alt text](image-23.png)



# 05 查找数组的长度

![alt text](image-24.png)


# 06 数组最后的索引


# 07 数组包含指定内容
![alt text](image-25.png)





# 学习数组 08 在数组中插入条目
![alt text](image-26.png)




# 删除数组，根据索引删除，根据内容删除
![alt text](image-27.png)




# 清除数组
![alt text](image-28.png)


# 检索array看到数组很多的操作方法

![alt text](image-29.png)




# 了解虚幻引擎的流程控制 01 Branches
前面控制true或者false走不同的分支，本质上大量if else
![alt text](image-30.png)



# 了解虚幻引擎的流程控制 02 Sequance
本质上是执行队列

![alt text](image-31.png)




# 了解虚幻引擎的流程控制 03 For Loop

![alt text](image-32.png)




# 了解虚幻引擎的流程控制 04 While Loop
![alt text](image-33.png)




# 了解虚幻引擎的流程控制 05 Do N

这条通公路只允许被执行4次
![alt text](image-34.png)




# 了解虚幻引擎的流程控制 06 Do Once
只允许被调用一次
![alt text](image-35.png)




# 了解虚幻引擎的流程控制 07 Flip Flop
每次执行这条通路会自动自动来回切换
![alt text](image-36.png)



# 05 了解虚幻引擎的流程控制 08 Gate

控制这条通路是否可以执行下去
![alt text](image-37.png)





# 05 了解虚幻引擎的流程控制 09 Multi Gate


多输出门，按一下G执行第一个，再按一下执行下一个，轮询执行
![alt text](image-38.png)



勾选这个就可以一直不断重复
![alt text](image-39.png)


随机选择一个执行
![alt text](image-40.png)


重置
![alt text](image-41.png)


# 函数、事件和宏 01 函数、事件和宏程序



# 选择节点，折叠节点
![alt text](image-42.png)



# 06 函数、事件和宏 02 折叠节点

![alt text](image-43.png)
折叠节点在这里可以看到
![alt text](image-44.png)


节点可以设置输入输出  

![alt text](image-45.png)



# 06 函数、事件和宏 03 事件




# 06 函数、事件和宏 04 自定义事件


![alt text](image-46.png)


![alt text](image-47.png)
找到我们的自定义函数
![alt text](image-48.png)

传参
![alt text](image-49.png)


# 函数、事件和宏 06 功能
ue的函数是纯工具方法的意思，不能在里面创建事件，但是可以调用事件，也不能调用延迟函数

函数也可以有输入输出
![alt text](image-50.png)






































