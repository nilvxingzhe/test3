# 计G191 2019322032 张胜
# 一、实验目的
1.掌握字符串String及其方法的使用
2.掌握异常处理结构
# 二、实验要求
利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。达到如下功能：
1.	每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
2.	允许提供输入参数，统计古诗中某个字或词出现的次数
3.	考虑操作中可能出现的异常，在程序中设计异常处理程序
4.	输入的内容，利用main方法中的args数组传递
# 三、实验流程
## 为《长恨歌》加标点符号并且按输出要求格式输出
```java
int count = 1;
         String wenben = "汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸………";
     char[] d = wenben.toCharArray();  			  //字符串对象转到字符数组中
     for (int i = 0; i < wenben.length(); i++) {   //for循环   wenben.length（）是字符串长
     System.out.print(d[i]);	
       if (i % 7 == 6) {						  //if 7个字符加符号	
           if (count % 2 == 1) {				       //if 判断加什么符号
           System.out.print("，");
        } else {
        System.out.print("。");
        System.out.println("");}
            count += 1;}}	
```
##输入参数，统计《长恨歌》中某个字或词出现的次数
```java
System.out.println("输入要查找的某字");
            Scanner input=new Scanner(System.in);   //输入字
                int count2=0;
            String in=input.next();				    //把input中的空格去掉
            char c=in.charAt(0);						//提取in里的第0个元素给c
            for (int i = 0; i < d.length; i++) {		//for循环   
            if (c==d[i]) {					
            count2++;}}
            System.out.println("某字出现的次数："+count2);}   //输出结果
```
## 设计异常处理程序
```java
try{}
catch (Exception e) {							//异常处理 
e.printStackTrace();}}
```
# 四、流程图
![image](https://github.com/nilvxingzhe/test3/blob/master/7.png)
# 五、实验结果
![image](https://github.com/nilvxingzhe/test3/blob/master/批注%202019-11-14%20210747.png)
# 六、编程感想
通过本次Java编程实验课，让我熟练的掌握了字符串String，length（）、charAt()、toCharArray()等方法。掌握异常处理结构，并且自己构造了异常处理。理解了程序中的逻辑关系。还复习了for循环和if的运用。在实验中我发现自己程序中的不足，通过网络和老师的帮助使我更好的改进了自己的程序，这次实验跟让我了解了自己的不足，我会在课下补足自己知识的盲点勤加练习，为之后的编程打下坚实的基础。
