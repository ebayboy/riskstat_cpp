
TODO:
- 增加异常处理try catch finally
- snippet code 增加C++模板类（包含exception的处理、构造函数等/类自定义异常, 继承异常类）
- snippet code上传到git hub上。
- 集成日志模块

#### 处理流程：
- 接收sub信息
- 读取redis数据
- 计算
    + 中缀表达式转后缀表达式（最小堆或二叉树实现）、计算
- 输出
- 多线程架构

- compute 数学表达式解析计算
    + SUM/AVG(ip, total, 5)  map + funccall 
        + start_end();  sep: ,
        + val ip_total_5m
    + EQ|GE|LE|GT|LT (ip_total_5m/all_total_5m,0.1)   sep:
        + 参数解析: ip_total_5m, all_total_5m, 0.1(LAST)
        + start_end (); sep: ,  sep2 + / - *
        + var: ip_total_5m, all_total_5m
        + 获取变量的value
        + 计算ret = ip_total_5m/all_total_5m => 输入数据到参数中
        + 计算 GT => ret > 0.1
    + and (vector<int> rules)

- output
    + 输出结果到redis

WillDo:
- noexcept shared_ptr

Done:
#### libs:
- cpp redis
- cpp json lib
- add libevent

- json to struct

#### 处理流程：
- 接收sub信息
- 读取redis数据
- 计算
- 输出
- 多线程架构