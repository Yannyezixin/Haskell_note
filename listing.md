#列表
- - -

1.列表是一种 单类型的数据结构

ep: let lostNumber = [4,8,15,16]

    PS: let 用来定义常量
ps: Haskell 中的字符串实际上就是一组字符组成的列表，"hello" 只是 ['h','e','l','l','o']
的语法糖。
what is 语法糖



2.拼接列表
ep: [1,2] ++ [3,4]

插入列表头部 运算符 ：  (ps:Cons运算符，来自lisp)
ep: 'a':" small cat" 
    a small cat

ps: [1,2] 实际上是=>  1:2:[]


3.访问列表中的元素
运算符： !!
ep: "abcdefg" !! 5
=>  f

4.嵌套列表
ep: [[3,3],[3,4]]

5.比较列表
ep: [3,4,4] == [3,4,5] 
按照字典顺序来进行比较

5.更多列表操作
ep: head [1,2,3,4]
=> 1
    tail [1,2,3,4]
=> [2,3,4]
    last [1,2,3,4]
=> 4
    init [1,2,3,4]
=> [1,2,3]

检查列表长度
ep: length [2,3]
=> 2

检查列表是否为空
    ep: null []
    => True
        null [1]
    => False

反转列表
ep: reverse [5,4,3,2,1]
=> [1,2,3,4,5]

取值take函数
ep: take 2 [1,2,3]
=> [1,2]
    PS:对应的则有drop

maximum 返回最大元素
ep: maximum [1,2,4,5]
=>  5
    PS: 对应的有minimum

sum函数，返回和
product,返回积

6.得州区间
[1..20]
表示1到20的列表
[1,3..21]
1到21的奇数


7.列表推导式--是一种过滤、转换或者组合列表的方法,类似数学中的集合
[x*2 | x <- [1,3..30]]
[x*2 | x <- [1,3..30], x*2 > 20]
[x+y | x <- [1..20] y <- [2,3..30]]



