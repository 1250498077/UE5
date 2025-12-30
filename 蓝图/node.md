


# 编辑完蓝图记得保存并编译
![alt text](image-7.png)



# 设置成蓝图之后要操控当前，要设置成玩家0
![alt text](image.png)




# 蓝图设置遵循物理碰撞
![alt text](image-1.png)



# 网格体被加载的时候，这个事件就会触发，当这个物体在场景中有多次的时候，就会被加载多次
![alt text](image-2.png)



# 获取图上的球体引用并打印球体的缩放程度
![alt text](image-3.png)
物体被加载就会被打印  
![alt text](image-4.png)



# 加载游戏的材质
![alt text](image-5.png)



# 构造器脚本几乎不用
构造器，就跟java构造器一样，主要用来初始化变量的
![alt text](image-6.png)
通过构造器写的逻辑，在没有开始游戏的时候就赋予了
![alt text](image-8.png)
构造器写的脚本逻辑打印只会出现在log里面，没有开始游戏也可以看到，拖动球体立即打印
![alt text](image-9.png)




# 每一帧都会被调用的函数
![alt text](image-10.png)
  
![alt text](image-11.png)
可以看到快速执行  
![alt text](image-12.png)





# 设置球体被触碰的时候会被调用的事件
先给球体添加碰撞检测  
![alt text](image-14.png)
![alt text](image-13.png)
碰上球体就会被打印
![alt text](image-15.png)




# 碰撞到的时候就销毁
实际情况下碰撞检测会产生多个重叠，一堆书，每个书都重叠，一重叠就销毁，很难控制
![alt text](image-17.png)



# 一般来说碰撞会使用这个
![alt text](image-19.png)
![alt text](image-16.png)
下面设置只允许和角色碰撞的时候才会被销毁  
![alt text](image-20.png)
other actor转换成功就设置就继续往下调用，不然就走cast failed
![alt text](image-21.png)






# 捡东西函数 ，只有第三人称蓝图才可以做这个事情
![alt text](image-22.png)
捡东西的时候打印这个  
![alt text](image-23.png)
捡东西自增1，这是第三人称的蓝图  
![alt text](image-24.png)
在捡到东西的时候，人物的移动速度会加快  
![alt text](image-25.png)
然后展示他的速度  
![alt text](image-26.png)



# 添加节点队列编排我们的代码执行流程
![alt text](image-27.png)
# 图片这样子写相当于红线
![alt text](image-28.png)





# 封装成函数
选中勾选这个  
![alt text](image-29.png)



# 将编码里面的移动速度设置成可变数字  
选中封装的函数，给他加入一个参数  
![alt text](image-30.png)
![alt text](image-31.png)
那么我们的外部参数就填入这个   
![alt text](image-32.png)
这是人物的，绑定到人物的自定义事件  
![alt text](image-33.png)
下面是物体的，在物体里面调用自定义事件并传入参数  
![alt text](image-34.png)
设置成变量  
![alt text](image-35.png)
下面是球体的蓝图，可以直接调用人物的引用里面的方法  
![alt text](image-36.png)
那么原来的人物方法就可以删掉了  
![alt text](image-37.png)








# 利用蓝图随机生成物体
新建普通蓝图类  
![alt text](image-39.png)

创建碰撞检测框   
![alt text](image-38.png)

获取到盒子的扩展并插入到此处  
![alt text](image-40.png)

每次开始游戏都会自动打印世界位置  
![alt text](image-41.png)






# 做一个区域内随机位置生成一个的逻辑
做一个区域
![alt text](image-51.png)

获得他的覆盖区域  
![alt text](image-50.png)

下面是从选择的类生成一个物体
![alt text](image-43.png)

下面可以随机生成一个物体，在地图上
![alt text](image-44.png)

可以切换视角的开始游戏
![alt text](image-45.png)

随机生成5个物体  
![alt text](image-46.png)
![alt text](image-47.png)





# 如果希望我们的实例可以被很多的人调用，生成的数量随机，那么设置这个就可以
![alt text](image-48.png)
被拖进世界的不同的物体可以设置不同的值
![alt text](image-49.png)




# 通过蓝图创建一个移动的对象
创建一个静态蓝图  
![alt text](image-52.png)

创建两个场景组件和一个正方体组件  
创建场景组件  
![alt text](image-53.png)
创建公告牌组件塞到场景组件里面标志一下，因为场景组件是全透明的  
![alt text](image-54.png)
设置公告牌组件位置跟随场景组件位置   
![alt text](image-55.png)
公告牌组件在游戏运行的时候就会销毁  


接下来控制方块移动  



# 添加时间轴节点
作用是创建一个时间轴，例如指定0秒一个变量的值是0，5秒的值变成1  
![alt text](image-56.png)  
双击打开编辑    
![alt text](image-57.png)  
加一个这个  
![alt text](image-58.png)  
右键创建这个  
![alt text](image-59.png)  
y轴代表变化大小，x轴代表变化速度  
![alt text](image-60.png)  
改成这个名字  
![alt text](image-61.png)  
可以看到这里有个名字  
![alt text](image-62.png)  
每次帧数刷新的时候都会调用这个方法  
![alt text](image-63.png)
启动游戏可以看到不断的打印这些东西  
![alt text](image-64.png)  
获取这两个场景的位置  
![alt text](image-65.png)  
图中画红线的节点，是一个算法工具，alphe 是0-1的数，节点输出的值是A轴x和B轴x之间的哪个数字，具体是哪个，由alphe根据比例来取值，例如x1=0，x2=10, alphe=0.5,那么这个节点输出的就是5.
![alt text](image-66.png)


接下来要做上下无限循环，我们希望它结束的时候再次启动时间轴，但是这次是从1到0  
下面就是我们想要做的，但是引擎不允许，  
![alt text](image-67.png)  
创建自定义事件  
![alt text](image-68.png)  

这个  
![alt text](image-69.png)  
但是还是没有实现我们的要求
 ![alt text](image-70.png)  
因为playstart只会被执行一次，下面那个会执行多次
![alt text](image-71.png)  
黄色节点是一个状态方法，交替执行不同的路径 
![alt text](image-72.png)  
名字这里ue要帮我们加一个空格，要小心
![alt text](image-73.png)  
电梯这里要小心，改下连线
![alt text](image-82.png)



# 继续完善游戏，构建这么个东西
![alt text](image-74.png)

放入场景之后放入这个东西来跳转旋转  
![alt text](image-75.png)
之前做电梯调整他的顶部位置可以控制电梯的上下
![alt text](image-76.png)


找到事件碰撞事件 
![alt text](image-77.png)

需要将另一个actor转换成第三人称  
![alt text](image-78.png)

根据玩家是否收集到5个产生不同的效果  
![alt text](image-79.png)
if的分支写法风格  
![alt text](image-80.png)



# 当玩家死亡的时候我们希望有些效果
设置特效位置
![alt text](image-83.png)


![alt text](image-84.png)
在特定的位置播放声音  
![alt text](image-85.png)
第三人称的销毁
![alt text](image-86.png)
这里拉出来
![alt text](image-87.png)
延迟两秒  
![alt text](image-88.png)
重新运行关卡  
![alt text](image-89.png)
在游戏关卡当中，只加载一次这个路径，避免反复触发
![alt text](image-90.png)