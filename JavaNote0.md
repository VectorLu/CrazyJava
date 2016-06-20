**编码规范**：
1. 类名、接口名、枚举、注解，每个单词首字母大写
2. 常量每个字母大写，单词之间加“_”
3. 包名单词全部小写
4. 变量名第一个单词小写，camel命名


1. 变量：
    1. 以字母、_、$为开头，仅数字不能作为开头
    2. 不能与Java关键字重名
    3. 局部变量方法内部声明；生命周期随方法的调用必须要有初始值（否则会造成编译错误）
    4. 全局变量（成员变量）：类的内部方法的外部声明，生命周期随对象的产生而产生，随对象的消亡而消亡，有默认的初始值

2. 数据类型：
    1. 基本数据类型（8种）：byte、short、int、long(L)、float（f/F小数点后7位)、double；char；boolean
    > 涉及到钱，使用BigDecimal类型，精确数据类型

3. 数据类型转换
    1. 自动转换```long lon2 = 12;```
    2. 强制类型转换```long lon3 = (long) 12.0f;```

4. 运算符
    1. “+” 连接运算（左边或者右边是字符串）；算数运算（左右均为数字）
    ```
    System.out.println(1 + 'a')；
    //
    ```
    2.
    ```
    boolean flag = true;
    if (flag = false)
    {
        //赋值后返回true
        //这段代码打印 1
        System.out.println(1);
    }
    else
    {
        System.out.println(2);
    }
    ```
    3.
    ```
    short s = 1;
    s += 1;
    s = s + 1; //1为int类型，做完这一步之后会自动转换为int类型，有这种性质的还有byte类型

4. 控制语句
    1. switch，表达式变量的数据类型：int char byte short string(1.7)
    2. for; while; do...while; for each

5. Java认为数据都是危险的，需要进行封装
6.
