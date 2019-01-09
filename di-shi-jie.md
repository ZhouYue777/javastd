# 第十节
[教学视频](https://ke.qq.com/webcourse/index.html#cid=346559&term_id=100412055&taid=2589843804998079&vid=r1428qz6y1f)

## 定义一个普通类

```text
class Person{
    int height=180;

    void eat{
        System.out.print("I'm eating.");
    }

    int fallinlove(String girlName){
        System.out.print("I'm dating with"+girlName);
        return 2;
    }

}
```

| 类的元素 | 示例 |
| :--- | :--- |
| 成员变量 | int height |
| 返回值类型 | void和int |
| 方法名称 | eat和fallinlove |
| 参数列表 | String girlName |
| 方法体 | System.out........ |

## 成员方法使用的变量

1. 成员方法可使用任何 _**成员变量**_ 。
2. 成员方法可使用本方法 _**参数列表中的变量**_ 。
3. 成员方法可使用本方法 _**局部变量**_ 。
4. 局部变量：定义在方法体内，只在本方法体内有效。

### 生成类型为Person对象的方式

```text
Person person    =     new Person();
类名    引用名称（随便）   new+类名+()
```

### 访问对象的成员变量和成员方法

凭证+“.”

例子：

* Person kobe=new Person\(\);
* kobe.age;
* kobe.height;
* kobe.lovenum;   访问成员变量
* kobe.eat\(\);
* kobe.fallinLove\("Fanbingbing"\)  访问成员方法

