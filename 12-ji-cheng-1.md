# 12.继承1

* 成员变量的特点
  * 子类只能获取父类的非私有成员
  * 就近原则: 先用局部变量，然后子类成员变量，然后父类成员变量
  * super: 可以获取父类的成员  

```text
class Dad {
    String name = "Dad";
}

class Kid extends Dad {
    String name = "kid";
    void show() {
        String name = "kidlocal";
        System.out.println(name);
        System.out.println(this.name);
        System.out.println(super.name);
    }
} 
```



* 成员方法的特点

  * 方法的重写：子类的方法和父类的一样（名称，参数列表，返回值），只有返回值不同则报错。
  * 有重写调用子类的。 
  * 没重写调用父类的。
  * 注解：@override 修饰成员
  * private  不能重写私有方法。
  * 重写的父子类权限：子类大于等于父类。父类public  子类重写不能private

* 继承中构造方法

  * 创建子类对象，如果子类构造_**方法的第一行**_，没有调用父类构造方法，则会默认调用父类无参构造方法。
  * 在子类构造的第一行，用**super**调用父类，或用**this**调用子类的其他构造方法。其他方法再调用父类的构造方法。
  * 第一行的原因是一定要先初始化父类的成员。 因为子类可能会使用。

 

* this  和 super
  * this:  当前对象的引用
  * super : 子类对象的父类引用





