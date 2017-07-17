#八进制   0---7    以0开头；  0=8进制   	console.log(017)=15;  0x8^2+1x8^1+7x8^0=15;
##十六进制   0---9  a---f  以0x开头；   0x=16进制  	console.log(0xf)=15;   
###允许使用e来表示乘以10的几次幂：console.log(5e5); //500000   
####总结一下，数字字面量有整数字面量（十进制、16进制、八进制），浮点数字面量（要记住e），Infinity，NaN
基本类型5种
	number 		数字类型	
	string		字符串类型
	undefined 	undefined类型，变量未定义时的值，这个值自己是一种类型
	boolean 	    布尔类型，仅有两个值true和false，讲if语句时我们细说
	null 		null类型，这个值自己是一种类型，遇见时我们细说

is not defined    js报错(代码写错了)
undefined    未定义值-----数据类型
null    object类型的一个特殊值
NaN     number类型的一个特殊值-----不是数字   

#alert(“哈哈”);
#prompt(“请输入数字”,”默认值”);   例如：  var a =prompt("请输入摄氏温度"); alert("哈哈，你的华氏温度是" + (9/5*a+32));
#console.log(“哈哈”);
#parseInt(“123”,8);
#parseFloat(“123”);
#Math.pow(3,4);
#Math.sqrt(81);

#####parseInt()和parseFloat()

#parseInt就是将一个string转为一个整数，不四舍五入，直接截取整数部分。如果这个string有乱七八糟的东西，那么就截取前面数字部分。
parseInt()不仅仅能够进行一个转为整数，更能进行一个进制的转换，把任何进制的数字，都换为10进制。

##parseFloat就是将字符串转为浮点数
尽可能的将一个字符串转为浮点数，浮点数之后如果有乱七八糟的内容，直接舍弃。