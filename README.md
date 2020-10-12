# Java-
Java课程作业项目仓库

##实验目的
  用类描述计算机中CPU的速度和硬盘的容量。要求Java应用程序有4个类，名字分别是PC、CPU、HardDisk 和Test,其中Test是主类。
其中，CPU类要求getspeed()返回speed的值，要求setSpeed(int m)方法将参数m的值赋值给speed;
     HardDisk 类要求getAmount()返回amount的值，要求setAmount(int m)方法将参数m的值赋值给amount;
     PC类要求setCPU(CPU c)将参数c的值赋值给CPU,要求setHardDisk(HardDisk h)方法将参数h的值赋值给HD,
     要求show()方法能显示CPU的速度和硬盘的容量。
●主类Test的要求
(1) main方法中创建一个CPU对象cpu,cpu将自己的speed设置为2200。
(2) main方法中创建一个HardDisk对象disk,disk将自己的amount设置为200。
(3) main方法中创建一个PC对象pc。
(4) pc调用setCPU(CPU c)方法，调用时实参是cpu.
(5) pc调用setHardDisk(HardDisk h)方法，调用时实参是disk。
(6) pc调用show（）方法。

##实验过程
    首先，需要建立一个package命名为“src”。建立一个class名为“CPU”，在class中定义speed为int型。使用get获得speed，使用set给speed赋值。
    再建立一个class名为“HardDisk”。调用Majorattribute方法，获取姓名、编号、上课地点、时间、学分的值。然后用toString方法打印出课程的属性。
建立一个class名为“students”。“students”继承“xuankexitong”的类、方法。通过toString方法打印出 "Students(学生信息):  姓名：" + Name + "学号：" + Num + "性别："+ Sex + "所选课程"+a。然后定义set函数用于修改名字。
建立一个class名为“Teachers”。“Teachers”继承“xuankexitong”的类、方法。通过toString方法打印出 "Teachers(老师信息):  姓名：" + Name + "工号：" + Num + "性别："+ Sex + "教授课程"+lesson。
Test。增加一个学生和一个教师的，分别使用System.out.println(students.toString())System.out.println(teachers.toString())输出信息。

##核心方法

##实验结果

##实验感想
