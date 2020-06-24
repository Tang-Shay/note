# Python简答题（小甲鱼）



## 第1讲



### 1. Python是什么类型的语言？

  脚本语言Scripting language，以简单的方式快速完成某些复杂的事情通常是创造脚本语言的重要原则。

### 2. IDLE是什么？

  IDLE是一个Python Shell，即外壳，也就是一个通过键入文本与程序交互的途径，利用IDLE这个shell和Python进行互动。



## 第2讲



### 1. 什么是BIF？Python3提供了多少个？

  Built-in Function 内置函数，为了方便程序员快速编写脚本程序，只需要直接调用即可。

  在Python中输入`dir(__builtins__)`即可以看到列表，共有68个

### 2. 用Python编写1~10中有几个奇数？

```# 1~10中有几个奇数
i = 1
num = 0
for i in range(11):
    if i % 2 == 0:
        continue
    else:
        num = num+1
print("1~10中有{}个奇数".format(num))
```



## 第4讲



### 游戏改进

- 要求一：猜错时，程序提示用户猜大了还是小了。

  使用`if...elif...else...`

- 要求二：应提供多次机会给用户猜测。（限制次数）

  即循环，使用`while` 和`and`逻辑操作符

- 要求三：每次运行程序时，答案应该随机。

  引入外援：`random`模块，里面有一个`randint()`，返回一个随机的整数

  使用：random.randint(1,10)

- 要求四：延迟输出两个语句？



## 第5讲



编写程序前的流程：

    加载背景音乐
    播放背景音乐
    我方飞机诞生
    
    小飞机出现时间间隔
    interval = 0
    
    while True:
        if 用户是否点击了关闭按钮：
            退出程序
            
        interval += 1
        if interval == 50:
            interval = 0
            小飞机诞生
    
        小飞机移动一个位置
        屏幕刷新
    
        if 用户鼠标是否移动：
            我方飞机中心位置 — 用户鼠标位置
            屏幕刷新
    
        if 我方飞机与小飞机是否发生碰撞：
            我方挂，播放挂机音乐
            修改我方飞机图案
            打印"Game Over"
            停止背景音乐（淡出）



## 第6讲：列表和元组



