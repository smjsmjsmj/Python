# Matplotlib
	在深度学习中，绘制图形是经常用到的功能，Matplotlib 是一个很简单的画图类库
## 绘制简单图形
	eg：
	import numpy as np
	import matplotlib.pyplot as plt
	x = np.arange(0,5,0.2) # 绘制X轴 0-5 间隔0.2
	y = np.sin(x)
	plt.plot(x,y) #绘制图形
	plt.show() # 显示图形
## 了解plot
	1. 添加X，Y轴 label
		eg:plt.xlabel("labelName")
		   plt.ylabel("labelName")
    2. 设置标题
    	eg:plt.title("title")
    3. 设置曲线的属性
    	eg:plt.plot(x,y,label="sin")
    	   plt.plt(x,y,linestyle="--",label="cos")
    eg:
    import numpy as np
	import matplotlib.pyplot as plt
	x = np.arange(0,5,0.2) # 绘制X轴 0-5 间隔0.2
	y = np.sin(x)
	y2 = np.cos(x)#cos图像
	plt.plot(x,y,label="sin") #绘制图形
	plt.plot(x,y2,linestyle="--",label="cos")
	plt.xlabel("x")
	plt.ylabel("y")
	plt.title("sin&cos")
	plt.legend()
	plt.show() # 显示图形
## 显示图像image
	使用imread 进行读取本地图片
	eg:
	from matplotlib.image import imread
	import matplotlib.pyplot as plt
	img = imread('图片地址')
	plt.imshow(img)
	plt.show()