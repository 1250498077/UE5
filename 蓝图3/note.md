






# 函数、事件和宏 08 宏

# 函数、事件和宏 10 宏程序库

怎么创建宏库
![alt text](image.png)


这里可以创建很多的宏
![alt text](image-1.png)


创建多个宏，写一些简单的逻辑，有输入输出
![alt text](image-2.png)


随便打开一个蓝图，就可以看到我们创建的宏  
![alt text](image-3.png)


# 什么是枚举变量 01 枚举变量解释

枚举器最重要的地方就是游戏任何地方都可以访问的了


# 什么是枚举变量 02 获取和设置

创建自定义枚举文件夹  
![alt text](image-4.png)


创建一系列的枚举变量  
![alt text](image-5.png)



在蓝图中可以直接搜索出来，选择绑定的枚举变量
![alt text](image-6.png)


![alt text](image-7.png)




# 什么是枚举变量 04 比较枚举变量的值
通过这样子的方式将枚举这个变量融入到  
![alt text](image-8.png)

创建自定义枚举的时候，可以选择使用switch选择不同的交互逻辑
![alt text](image-9.png)


# 类 01. 游戏结构
![alt text](image-10.png)





# 08 类 03. 组件

网格体可以放在网格体里面，子网格体随着父网格体移动而移动
![alt text](image-11.png)




# 类 04. 游戏模式

去到世界设置  
![alt text](image-12.png)

怎么改变游戏模式，右键点击这里设置蓝图类  
![alt text](image-13.png)

![alt text](image-14.png)

创建一个游戏模式  
![alt text](image-15.png)

拖动  
![alt text](image-16.png)

默认pawn类被修改成default  
![alt text](image-18.png)

如果我想选择我的第三人称角色  
![alt text](image-17.png)




# 08 类 05. Pawn

Pown 是我用控制器控制的东西，或者你使用pown来被AI控制，记住pown具有位置 ，旋转和缩放
Pown 也是我们角色的代表， 它如何在环境中移动以及谁控制它
pown 是一个可以被控制器接收输入的 actor， pown 不能自动分配给控制器，我需要在游戏开始前做这件事. 


![alt text](image-19.png)

![alt text](image-20.png)

这是pown的细节  
![alt text](image-21.png)

如何将pown设置为场景的默认值  
![alt text](image-22.png)
什么都没有，我们只有一个固定的摄像机  
![alt text](image-23.png)

如果想返回使用的pown类，直接拖回去即可
![alt text](image-24.png)


![alt text](image-25.png)

































