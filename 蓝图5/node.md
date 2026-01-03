


# 11 创建第一人称角色 01 第一人称角色的基本设置
创建一个新关卡  
![alt text](image.png)


# 保存当前关卡到自己想要的文件夹
![alt text](image-1.png)

当我们开始游戏的时候， 我们发现还是默认的，这是因为我们没有创建我们自己游戏模式  
![alt text](image-2.png)
这里创建游戏模式  
![alt text](image-3.png)
![alt text](image-4.png)
![alt text](image-5.png)
会默认设置好这么多东西  
![alt text](image-6.png)

开始的时候可以看到只有一个摄像机  
![alt text](image-7.png)

这里也可以设置成第三人称游戏模式   

![alt text](image-8.png)

设置玩家从地图何处开始  
![alt text](image-9.png)

设置playstart的方向， 位置代表玩家在游戏开始时候的位置  
![alt text](image-10.png)

创建一个默认角色  
![alt text](image-11.png)

创建一个角色蓝图类  
![alt text](image-12.png)

创建一个播放器控制器  
![alt text](image-13.png)
拖动到这里  
![alt text](image-14.png)


三条线分别代表设置游戏模式，角色生成位置，角色相机朝向
![alt text](image-15.png)


![alt text](image-16.png)




# 11 创建第一人称角色 02 相机设置

双击  
![alt text](image-17.png)
角色控制器，这些是不能删除的，这个蓝图继承这个角色的这些类  
![alt text](image-18.png)


一些角色控制器的高度  
![alt text](image-19.png)

重命名我的相机为主相机，因为一个角色可以有很多的相机  
![alt text](image-20.png)

设置摄像机视野  
![alt text](image-21.png)



# 11 创建第一人称角色 03 鼠标 - 相机控制
加上之后，移动鼠标就可以转换左右视角  
![alt text](image-23.png)

![alt text](image-25.png)
![alt text](image-24.png)
我们的视角就饿可以切换了，但是有个点，我们的角色整体会随着视角变换也旋转视角，这是不对的，我们只希望旋转摄像机  

所以这个要关掉  
![alt text](image-26.png)

在摄像机的细节面板展示这个，而不是让角色整体旋转，顾名思义，摄像机跟随pawn去动  
![alt text](image-27.png)

# 11 创建第一人称角色 04 鼠标 - 相机控制映射

项目设置这里创建这两个东西
![alt text](image-29.png)

就可以在蓝图当中找到他  
![alt text](image-30.png)

鼠标视角转换控制  
![alt text](image-28.png)


# 11 创建第一人称角色 05 PS4 操纵杆 - 相机控制

加两个操纵杆   
![alt text](image-31.png)

蓝图长这样  
![alt text](image-32.png)



# 11 创建第一人称角色 06 键盘 - 运动

设置项目设置
![alt text](image-34.png)


![alt text](image-33.png)




# 11 创建第一人称角色 07 PS4 操纵杆-移动


继续创建操纵杆  
![alt text](image-35.png)



![alt text](image-36.png)




# 11 创建第一人称角色 08 用键盘和操纵杆跳跃和下蹲



控制代码  
![alt text](image-37.png)


切换  
![alt text](image-38.png)

这些蹲下跳跃动作都是这个第三人称角色
这是动作的细节  
![alt text](image-39.png)


# 11 创建第一人称角色 09 设置自定义步行和蹲下速度

设置移动速度    
![alt text](image-40.png)




# 11 创建第一人称角色 10 设置角色运动


![alt text](image-41.png)  


直接设置变量就可以影响角色移动速度  
![alt text](image-42.png)   


将移动速度提取为变量  
![alt text](image-43.png)  



# 11 创建第一人称角色 11 物体相互作用--球体投射


交互事件，在角色前方生成一个椭圆形球体  

![alt text](image-44.png)


设置  
![alt text](image-47.png)

![alt text](image-46.png)


设置debug
![alt text](image-45.png)



# 11 创建第一人称角色 12 抓取物体

添加这样子的东西，我的理解是让角色拥有和其他物体有物理交互的能力，因为实时计算大，所以需要手动开启   
![alt text](image-56.png)


这个是抓取组件  
![alt text](image-48.png)


关键点，设置一个空的场景组件，将抓取的物体设置到这个位置，然后每一帧都更新物体的位置  
![alt text](image-49.png)


所以要先获取被抓住的实例，然后实时更新被抓取的物体的位置为空的场景组件位置  
![alt text](image-51.png)

红圈的判断的是是否命中物体  
![alt text](image-50.png)

注意设置被移动物体是可以移动的
![alt text](image-52.png)


被抓去的物体还要唤醒刚体，这算是一个bug  
![alt text](image-53.png)

把物体放下的节点  
![alt text](image-54.png)

获取物体的时候设置为true  
![alt text](image-55.png)












