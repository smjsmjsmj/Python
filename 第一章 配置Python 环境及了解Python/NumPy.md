# NumPy
   ·在深度学习中经常用到数组和矩阵的计算 ，所以我们常用NumPy 帮助我们计算
        eg：
        import numpy as np
        x = np.array([1,2,3,4,5])
        print (x)
   ·数组的运算：即数组每个元素的运算
       eg:
       import numpy as np
        x = np.array([1,2,3,4,5])
        y = np.array([6,7,8,9,10])
        print (x+y)# 加法
        print (x*y) #乘法
       print (x-y) #减法
       print (x/y) #除法
       注：数组间进行运算时，应保证数据的长度一致，否则将会出错
   ·多维数组
       import numpy as np
        x = np.array([[1,2],[3,4]])
        print (x)
    同理相同矩阵之间可以进行运算
   ·广播 
    当一个矩阵和一个标量进行运算时，会将标量扩充成矩阵相同维度进行运算
    eg:
        import numpy as np
        x = np.array([[1,2],[3,4]])
        print (x*10)