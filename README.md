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
    首先，需要建立一个package命名为“src”。建立一个class名为“CPU”，在class中定义speed为int型。调用setspeed方法，获取speed的值。
    再建立一个class名为“HardDisk”。在HardDisk中定义amount为int型。调用setAmount方法，获取amount的值。
    再建立一个class名为“Text”。调用static方法，给speed和amount赋值。
    再建立一个class名为“PC”。调用方法获取cpu，HD的值，然后用System.out.println函数输出信息。

##核心代码
CPU.java

package src;

public class CPU {
	private int speed; 
	   int getSpeed() {
	      return speed;
	   }
	   public void setSpeed(int speed) {
	      this.speed = speed;
	   }
	}
  
HardDisk.java

package src;

public class HardDisk {
	private int amount; 
	   int getAmount() {
	      return amount;
	   }
	   public void setAmount(int amount) {
	      this.amount = amount;
	   }
	}
  
PC.java

package src;
import src.CPU;
import src.HardDisk;

public class PC {
	CPU cpu;
    HardDisk HD;
    void setCPU(CPU cpu) {
        this.cpu = cpu;
    }
     void setHardDisk(HardDisk HD) {
        this.HD = HD;
    }
    void show(){
       System.out.println("CPU速度:"+cpu.getSpeed());
       System.out.println("硬盘容量:"+HD.getAmount());
    }
}

Text.java

package src;

import src.CPU;
import src.HardDisk;
import src.PC;

public class Test {
	public static void main(String[] args) {
	       CPU cpu = new CPU();
	       HardDisk HD=new HardDisk();
	       cpu.setSpeed(2200);
	       HD.setAmount(200);
	       PC pc =new PC();
	       pc.setCPU(cpu);
	       pc.setHardDisk(HD);
	       pc.show();
	    }
}

##实验结果
![image](https://github.com/2018310736smy/Java-/blob/main/jieguo.jpg)
CPU速度:2200
硬盘容量:200

##实验感想
    对于我这个初学者而言，把Java、python与基础的C语言相比，如果说python重在对于库的调用，那么Java可能重在对于father的类、属性、方法的继承。所以，在编程的开始，我们要考虑清楚编程对象的需求，考虑清楚个体所具备的属性，并寻找他们的共性。同时还要考虑清楚如何筛选或者聚集相同类或者不同类的个体。
    此外，Java的简洁性在于它像一棵树，father是主干，而其他的class像是分支，即使不同于主干，却依旧能获得与主干相同的属性，继承到主干的类、方法、属性。
