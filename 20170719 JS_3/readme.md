#循环语句   for循环-----很重要--认真学


    for(初始值 ; 范围 ; 步长){
        循环的语句---先输出,再计算步长.最后得出结果
    }
例如：	for(var i = 4 ;---第一步 i <= 10 ;----第二步 i+=2-----最后一步){
		console.log(i);----第三步	//4 6 8 10;
	             }

##for循环里每一个条件约束之间都要用;隔开
    当循环变量已经在外部定义了，并不需要在①号位上重新定义，写一个空的;
#可以不写，但是位置一定要空出来；
	var i = 8;
	for(; i<12;i++){
		console.log(i);
	}


#穷举法
###水仙花数
for(var i=100;i<=999;i++){
    var gewei =i%10;
    var shiwei=parseInt(i/10)%10;
    var baiwei=parseInt(i/100);
   
  
    if(Math.pow(baiwei,3)+Math.pow(shiwei,3)+Math.pow(gewei,3)==i){
         console.log(i);
    }
 }


###累加器


            var num = 0;
            for( var i = 1;i <=100;i++){
                num = num+i;
            }

            console.log(num);
            console.log(i);

           注释     //num =0 i =1  num =1
                //num =1 i =2  num =3
                //num =3 i =3  num =6
                //num =6 i =4  num =10


###累乘器


            var num = 1;
            for(var i =6;i>=1;i--){
                // num = num*i;
                num*=i;

                //num =1 i =6   num = 6
                //num =6 i =5   num = 30
                //num =30 i =4   num = 120
                //num =120 i =3   num = 360
                //num =360 i =2   num = 720
            }
            console.log(num);
            console.log(i);
        


#break语句 

    for(var i=1;i<=100;i++){
        console.log(i);
        if(i==5){
            break;
        }
    }


#continue语句 

   for(var i=1;i<=10; i++){
        if(i==5){
            continue;
        }
            console.log(i);
    }


#do while语句
        var i =1;
    do{
        console.log(i);
        i++;
    }while(i<=10)

for语句是主力语句，也就是说，for做不到的，do……while也同样做不到。do……while能做到的，for也一定能做到。
do……while语句中没有循环变量，适合没有循环变量的情况。经常地，它是个死循环。

