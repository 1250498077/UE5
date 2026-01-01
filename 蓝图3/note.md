






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
游戏模式，也是一个蓝图类，例如第三人称也算是一个游戏模式


去到世界设置  
![alt text](image-12.png)

![alt text](image-26.png)

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




# 08 类 06 角色类
![alt text](image-27.png)

![alt text](image-28.png)

![alt text](image-29.png)

![alt text](image-30.png)

这里可以调整人物动作所有的参数，例如移动速度

![alt text](image-31.png)


骨骼动画
![alt text](image-32.png)

胶囊控制器，控制两个物体的碰撞  
![alt text](image-33.png)  


摄像机和摄像机吊杆
![alt text](image-34.png)



# 08 类 07 控制器



![alt text](image-35.png)

![alt text](image-36.png)


![alt text](image-37.png)

![alt text](image-38.png)


![alt text](image-39.png)

![alt text](image-40.png)


# 09 演员 01 静态网格


网格体和actor不是一个东西



# 09 演员 02 变换
获取自己在世界场景中的位置，也可以获取自己在actor里面的相对位置，
世界偏移+actor内部相对偏移 = 叠加偏移


![alt text](image-41.png)

![alt text](image-42.png)


![alt text](image-43.png)

1980

![alt text](image-44.png)


![alt text](image-45.png)


获取旋转，
![alt text](image-46.png)


# 09 演员 03 Actor的创建与消除

创建一个变量  
![alt text](image-49.png)

![alt text](image-48.png)


创建和销毁节点，按0不断的切换
![alt text](image-47.png)



# 09 演员 04 IsValid校验
确保仙人掌被销毁的方式，获取这个仙人掌的坐标发现获取不到  
![alt text](image-50.png)


按下x检查场景中的actor是否被生成  
![alt text](image-51.png)



# 09 演员 05 获取所有Actor信息


![alt text](image-52.png)

返回一个数组，然后创建一个这样类型的变量获取值
![alt text](image-53.png)



![alt text](image-55.png)





# 09 演员 06 骨架网格

![alt text](image-56.png)

静态网格和骨架网格的区别  

找到第三人称蓝图  
![alt text](image-57.png)

这里有一个骨架
![alt text](image-58.png)

找到网格本身  
![alt text](image-59.png)


骨骼网格长这样  
![alt text](image-60.png)

左边是所有的骨骼
![alt text](image-61.png)


选中所有的骨骼，可以旋转  
![alt text](image-62.png)


展示所有的骨头  
![alt text](image-63.png)


所有的骨架  
![alt text](image-64.png)


在场景中生成第三人称角色  
![alt text](image-65.png)



# 09 演员 07 触发器

触发就是碰撞检测  
![alt text](image-66.png)  

触发器默认是关闭的，所以想看到的话就去掉  
![alt text](image-67.png)

触发器事件  
![alt text](image-68.png)

当出现触发器的离开和碰撞    
![alt text](image-70.png)


# 09 演员 08 网格标签

下面图的逻辑是按下0，就删除数组的第0个元素

获取一堆数组，筛选出指定tag的元素
判断数组第0个是否有元素
有就删除
没有啥也不干
![alt text](image-71.png)




































































