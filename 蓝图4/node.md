


# 09 演员 09 Actor演习
使用定时器动态在场景中生成actor  
![alt text](image.png)


使用定时器删除  
![alt text](image-1.png)


将数组中的元素随机改变大小  
![alt text](image-2.png)







# 10 蓝图沟通 01 蓝图沟通

# 10 蓝图沟通 02 直接沟通

门  
创建蓝图类  
![alt text](image-3.png)  

创建网格体  
![alt text](image-4.png)  

这个名字后面可以绑定
![alt text](image-5.png)

第三人称蓝图，创建一个门的类型，类似于java的自定义类型  
![alt text](image-6.png)

将我们的第三人称角色拖动到蓝图，设置成角色0，就从我们创建的角色开始游戏。
![alt text](image-7.png)


我们在角色当中使用了门这个类型，那么需要绑定一个实例，所以还需要选择上门  
![alt text](image-8.png)

角色蓝图
![alt text](image-9.png)



# 10 蓝图沟通 03 特性


地板方块的事件触发器，获得人类触发之后，便能获取到人类这个引用，然后调用这个引用的开门关门方法  
![alt text](image-10.png)


这是人类内部的自定义事件，暴露给外部使用  
![alt text](image-11.png)



# 10 蓝图沟通 04 蓝图界面-基础
使用相同的输入，创造不同的交互  

给网格设置碰撞体  
![alt text](image-12.png)

选中石头，将石头转换成蓝图类
![alt text](image-13.png)

默认设置 
![alt text](image-14.png)



人物蓝图设置，这里是按下e键，然后在人物的前端放置一个东西

![alt text](image-15.png)
生成一个椭圆形球体
![alt text](image-16.png)

![alt text](image-17.png)

![alt text](image-18.png)

![alt text](image-19.png)
按下e发现生成了个东西
![alt text](image-20.png)






创建蓝图接口  
![alt text](image-21.png)


双击打开 
![alt text](image-22.png)

在这个接口类创建方法  
![alt text](image-23.png)


在仙人掌和石头蓝图里面实现这个接口  
![alt text](image-24.png)



在人类生成的球体里面 
![alt text](image-25.png)


这里是人类生成球体所触发的所有事情  
![alt text](image-26.png)


这里是碰撞到谁传给谁   
![alt text](image-27.png)



在石头和仙人掌蓝图里面创建接受事件
![alt text](image-28.png)


# 10 蓝图沟通 05 蓝图界面-输入


给接口传播创建输输入输出  
![alt text](image-29.png)


在仙人掌和石头就可以接收这些值  
![alt text](image-30.png)





# 10 蓝图沟通 07 事件调度  


这里说明的是，当人类执行一个逻辑的时候，想先执行其他蓝图里面的逻辑，其他蓝图里面的逻辑执行完，人类才继续往下执行。  



在第三人称角色上创建角色调度器  
![alt text](image-31.png)
将事件调度器放入到自己想要的逻辑当中  
![alt text](image-34.png)



其他蓝图要和人来蓝图的事件调度器链接才行  
![alt text](image-35.png)




这个就是将其他蓝图事件注册到人类蓝图的完整步骤。 
![alt text](image-36.png)



额外知识，这个不是是self，因为这是相对位置偏移，只能是蓝图类中特定的元素，self就是顶层节点，顶层节点禁止设置相对位置偏移  
![alt text](image-37.png)


这块代码是按下U会接触绑定  
![alt text](image-38.png)



额外知识：要设置石头移动才可以变化
![alt text](image-39.png)




这里不是很懂???????? 
![alt text](image-40.png)







