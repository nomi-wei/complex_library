Complex 库
====================

* @author: `Otto Lu`
* @version: 0.002
* @description: `一个挫逼的简单的复数运算库`
* @license: WTFPL

---------------------------
###使用说明

直接 `include "complex.hpp";` 就 ok 了

----------------------------
###API文档

#### 声明

	`fcomplex` 为单精度浮点复数类型
	
	`dcomplex` 为双精度浮点复数类型

#### 支持运算符

	= ==
	+ - * / 
	+= -= *= /=
	<< >>
	()

#### 支持 math 库函数重载
	`pow()`

#### 提供函数
	`val()`         取出模值
	`real()`        取出实数部分
	`imag()`        取出虚数部分
	`real(type)`    为实数部分赋值
	`imag(type)`    为虚数部分赋值

#### 提供的部分语法糖
	
	// 例子
	fcomplex fc(1.0f, 1.0f);

	fc();              // 对变量名用(), 等价于 fc.val()
	fc(2.0f, 2.0f);    // 为变量赋新值, fc => 2.0 + 2.0i

	cout<<fc;          // 输出 2.0+2.0i
	cin>>fc;           // 当输入 3.0 3.0 时, fc => 3.0 + 3.0i

------------------------------

Hope U will like it!~