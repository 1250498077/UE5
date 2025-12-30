





- 创建材质，材质比较特殊，需要采样地面的纹理
- 设置采样的范围，只有在特定的范围才需要虚拟地面的纹理






# 纹理混合做法，先打开景观材质
![alt text](image.png)








# 打开景观材质节点

![alt text](image-1.png)


# 这个节点的作用就是从景观中捕获一些数据,并能够投影到世界的静态网格体上，达到混的的效果
![alt text](image-2.png)






# 我们需要获取材质像素的位置，也需要通过一个节点来是实现，
![alt text](image-4.png)

而且我们只想要z，所以需要节点过滤一下
![alt text](image-5.png)




# 成品
![alt text](image-6.png)




# 还需要创建一个虚拟纹理存储这些数据，在content右键创建虚拟纹理
![alt text](image-7.png)

再复制一份，一个存储高度，一个存储材质
![alt text](image-8.png)




# 确保使用虚拟纹理和写成10000
![alt text](image-9.png)

双击  
![alt text](image-10.png)
设置成世界高度，另一个保持原样   
![alt text](image-11.png)



# 提示景观材质需要重建
![alt text](image-12.png)


但是我们可以先关闭光照，不然就会把光照烘焙。强制关掉光照烘焙
![alt text](image-13.png)


![alt text](image-14.png)


现在就可以build level了


# 现在需要规定虚拟纹理从景观中捕获的范围，用下面这个东西规定范围

![alt text](image-15.png)

包裹住我们材质的范围
![alt text](image-16.png)

# 然后我们给这个创建的出来的范围添加我们更改创建出来的两个虚拟材质

![alt text](image-17.png)

![alt text](image-18.png)
# 设置我们景观的虚拟纹理
![alt text](image-19.png)


# 打开石头的父级材质实例
![alt text](image-20.png)
![alt text](image-21.png)





# 拖动资产材质到上面
![alt text](image-23.png)

# 然后改成这样
![alt text](image-24.png)

# 双击进入功能材质团
![alt text](image-25.png)

# 将虚拟纹理作为材质输入到石头上面，说白了就是将我们的纹理放到材质上而已
![alt text](image-22.png)









