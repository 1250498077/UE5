





















# 004 Creating a C++ Class



# 005 Live Coding


如果我们更改.h文件，关闭visual 再重新打开是最好的选择，如果更改.cpp文件，那么即可
这是重新编译  
![alt text](image-1.png)
但是我们最好保证每天都进行一次重新生成按钮  


更改代码之后点击这个，就可以进行编译了  
![alt text](image.png)



# 006 Variables and Data Types


# 007 Logging Variables
打印变量  
![alt text](image-2.png)
打印浮点数  
![alt text](image-3.png)

# 008 Number Operations



# 009 Operator Precedence


# 010 Member Variables

这个注解可以让ue识别到他，在.h文件    
![alt text](image-4.png)


在.cpp文件随便使用  
![alt text](image-5.png)


在ue展示，但是不允许更改  
![alt text](image-6.png)


# 011 Structs

向量类型  
![alt text](image-8.png)


![alt text](image-9.png)

创建向量并更改  
![alt text](image-10.png)


定义向量  
![alt text](image-12.png)
![alt text](image-11.png)


# 012 SetActorLocation
在ue的c++里面这里添加一系列的东西  
![alt text](image-13.png)


动态设置位置  
![alt text](image-14.png)

# 013 Tick

每一帧都会调用这个方法， 这里做了个简单的物体移动  
![alt text](image-15.png)


# 014 Comments


# 015 GetActorLocation
让方块不断的移动  
![alt text](image-16.png)


# 016 Delta Time

这个值代表的是渲染一帧需要的时间，快的电脑需要0.01秒，慢的电脑需要0.1秒  

为了适应不同的帧数都移动相同的距离，这里需要乘以帧数 
![alt text](image-17.png)



# 017 Velocity

向量相加是这样子加  
![alt text](image-18.png)





向量相乘  
![alt text](image-19.png)





# 019 Function Parameters
定义方法要在前面  


# 020 Member Functions


创建类方法，比之前多一个动作就是需要在.h文件里面定义  

![alt text](image-21.png)
![alt text](image-20.png)







# 021 Classes And Instances
这里说明了我创建了一个蓝图类，然后再场景有很多的实例， 修改蓝图类里面代码，会影响到所有的实例  





# 022 Blueprint Child Classes


![alt text](image-22.png)
子类的概念  
![alt text](image-23.png)

这可以让不同的模型，拥有同样的动画，因为可以在父类里面写动作方法，蓝图里面使用不同的模型     
以一个我们创建的c++类，然后创建一个子蓝图类，子蓝图类会继承父c++的方法  
在内容区创建蓝图类的时候选择这个c++类即可  
![alt text](image-24.png)

子蓝图可以看到父类的方法  
![alt text](image-25.png)


# 023 Distance Between Vectors

举了例子，获取两个actor之间的距离  

计算开始位置和当前位置之间的距离   
![alt text](image-26.png)

.h文件定义
![alt text](image-27.png)

可以看到这个值在动态变化  
![alt text](image-28.png)


# 024 If Statements

PlatformVelocity 的意思是向某个地方一段距离  

![alt text](image-29.png)

![alt text](image-30.png)

# 025 Overshoot Problem

# 025 Overshoot Problem

防止偏离用的，因为游戏实际运行的时候，物体移动距离肯定会超出一点点，那么物体在反方向移动的时候， 要将这点超出
的距离补偿回去。
![alt text](image-31.png)


# 027 Function Return Values
![alt text](image-32.png)

# 028 Rotating Platforms
![alt text](image-33.png)



# 029 Importing Assets

fab下载导入即可  
![alt text](image-34.png)
创建蓝图类，把材质拖进去，就可以使用我们的c++了 


# 031 Movement & Physics.mp4


![alt text](image-35.png)



# 032 Level Design



# 033 Packaging The Game











