# 第十节

### 定义一个普通类

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

### 成员方法使用的变量

1. 成员方法可使用任何 ***成员变量*** 。
2. 成员方法可使用本方法 ***参数列表中的变量*** 。
3. 成员方法可使用本方法 ***局部变量*** 。



