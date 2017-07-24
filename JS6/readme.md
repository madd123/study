#一.预解析   
               浏览器
               "js解析器"
                  一.预解析
                      1.找一些东西： var function 参数
                          a = 1

##变量预解析
## 所有变量在正式运行之前，都会被赋一个值，未定义 var a= undefined;

所有的函数，正式运行之前，都是这个函数快

遇到重名的，只留一个;

变量和函数重名了，就留下函数

# 二.逐行执行代码
                     表达式 ： = + - * / %

         // 案例1

         // alert(a);   //function a(){alert(4);}
         // var a = 1;
         // alert(a);   // 1
         // function a(){alert(2);}
         // alert(a);   //  1
         // var a = 3;
         // alert(a);   // 3
         // function a(){alert(4);}
         // alert(a);   //3


         var a = 1;
         function fun(){
            alert(a);   // 未定义
            var a = 2;
         }
         fun();
         alert(a);  //  1


##作用域
                域：空间、范围、区域
               作用：读 写

                全局变量  全局函数
                自上而下

                函数内部也是一个域
                由内而外


          