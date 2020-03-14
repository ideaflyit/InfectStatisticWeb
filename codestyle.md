​	代码规范来源：https://github.com/chjw8016/alibaba-java-style-guide

- 变量命名采用lowerCamelCase驼峰命名法，代码中的命名均不能以下划线或美元符号开始，也不能以下划线或美元符号结束，严禁使用拼音与英文混合的方式，更不允许直接使用中文的方式。

  ```
  正例：String[] strArr={};
  反例：String shengfenArr={};
  ```

- 每行最多字符数

  每行字符数一般控制在50字符左右。如果超过则会换行并对齐。

  ```
  if(!(args[i].equals("-log")||args[i].equals("-out")
  ||args[i].equals("-date")||args[i].equals("-type"))) 
  ```

  换行是遵循以下原则：

  - 后面的行相对第一行对齐。
  - 运算符与下文一起换行。
  - 方法调用的点符号与下文一起换行。
  - 在多个参数超长，逗号后进行换行。
  - 在括号前不要换行。

- 函数最大行

  根据函数实现的功能，一般尽量不超过50行

  运算符与下文一起换行。

  方法调用的点符号与下文一起换行。

  在多个参数超长，逗号后进行换行。

  在括号前不要换行。

  ```
  StringBuffer sb = new StringBuffer();
  sb.append("a").append("b")...
  	.append("c")...
  	.append("d")...
  	.append("e");
  ```

- 函数类命名

  函数命名使用lowerCamelCase驼峰命名法。类命名使用UpperCamelCase驼峰命名法如：

  ```
  正例：
  boolean isNumber(String str) {
  	........
  	return false;
  }
  class Dog {
  	private:
  		............
  	public:
  		............
  }
  反例：
  boolean IsNumber(Stirng str) {
  	.........
  }
  ```

- 常量命名

  通常使用全大写英文，单词之间使用下划线隔开，如：

  ```
  正例：#define PI 3.14   #define USER_NUMBER
  ```

- 空行规则

  类与之间空行，类与函数，函数与函数，循环结构，判断结构直接空一行至两行。如：

  ```
  正例：
  class Dog {
  	private:
  		............
  	public:
  		............
  }
  
  class Cat {
  	private:
  		............
  	public:
  		........
  		.........
  }
  ```

- 注释规则

  - 类、类属性、类方法的注释必须使用Javadoc规范，使用/\*内容\*/格式，不得使用//方式。

  - 方法内部单行注释，在被注释语句上方另起一行，使用//注释。方法内部多行注释使用/* */注释，注意与代码对齐。

  ```
  正例：
  int num;  //计算数目
  /*判断是否为数字*/
  boolean isNumber() {
  	........
  }
  /*
  狗类
  创建者：cybin007
  */
  class Dog {
  	int age;  /*年龄*/
  }
  ```

- 操作符前后空格

  左大括号前加空格，其余符号如：+-*/=不加

  ```
  for(int i=0;i<10;i++) {
  	if(i==0) {
  		......
  	}
  }
  ```

- 大括号的使用约定。

  如果是大括号内为空，则简洁地写成{}即可，不需要换行；如果是非空代码块则：

  - 左大括号前不换行。
  - 左大括号后换行。
  - 右大括号前换行。
  - 右大括号后还有else等代码则不换行；表示终止右大括号后必须换行。

  ```
  正例：
  if(i==0) {
  	return 0;
  } else {
  	return 1;
  }
  ```

- 缩进

  一般采用一个tab键或者4个空格实现缩进

  ```
  if(i==0) {
  	i++;
  }
  
  ```