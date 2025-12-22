
# 使用别处的材质

# 1.直接拖动图片给软件

![alt text](image.png)

# 2.ue5有点聪明，可以根据颜色识别哪些是法线贴图
![alt text](image-1.png)


# 法线贴图关键配置
![alt text](image-2.png)


# 确保sRGB打开
![alt text](image-3.png)


# 遮罩层确保去掉
![alt text](image-4.png)


# 创建一个人行道材质
![alt text](image-5.png)


# 双击打开材质，然后选择三个纹理直接拖进去
![alt text](image-6.png)



# 颜色贴图自动设置成color
![alt text](image-7.png)



# 这里是线性color
![alt text](image-8.png)



# 蓝色默认是法线模式
![alt text](image-9.png)



# 放到地板上我们发现很密集
![alt text](image-10.png)




# 我们希望可以创建一些参数  
允许用户去调整贴图的长宽，TexCoord 永远只输出两个数字 (U, V)
![alt text](image-11.png)
用一个参数控制材质的参数细节
![alt text](image-12.png)




# 1.法线图转换：Blender使用OpenGL法线图，而Unreal Engine使用DirectX法线图。
2.转换方法：通过翻转绿色通道来转换法线图，确保阴影和法线方向正确。
![alt text](image-13.png)




# 进一步优化，横向坐标和纵向坐标都可以设置材质大小
![alt text](image-14.png)



# 控制贴图的位置
![alt text](image-15.png)



# 继续优化，增强法线的凹凸强度
![alt text](image-16.png)



# 调整贴图颜色
![alt text](image-17.png)



# 将贴图全部转换成参数
![alt text](image-18.png)



# 金属材质
![alt text](image-19.png)
勾选就可以设置材质
![alt text](image-20.png)