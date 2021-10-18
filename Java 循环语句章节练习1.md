Java 循环语句章节练习1

```java
package chapterrlearn;
import java.util.Scanner;
public class ChapterLearn{
	public static void main(String[] args){
		System.out.println("请输入一个整数（1-7）");
		Scanner s= new Scanner(System.in);
		int n = s.nextInt();
		if(n<=10){
			int b=1;
			for(int i=1;i<=n;i++){
				 b=i*b;
			}
			System.out.println(b);
		}
	}
}
class BaiQianMaiJi{
	public static void main(String [] args){
		for(int b=0;b<=33;b++){
			int c=(100-b*3)/2;
			for(int a=0;a<=c;a++){
				int d=100-b-a;
				if(d%3!=0){continue;}
				 int e=b*3+a*2+d/3;
					if(e==100){
					System.out.println(b+" "+a+" "+d);
					}
			}
		}
	}
}
class BanZhuan{
	public static void main(String[] args){
		for(int a=0;a<7;a++){
			int b=(36-a*4)/3;
				/* if(b%3!=0){continue;} */
			for(int c=0;c<=b;c++){
						int d=36-a-c;
						if(d%2!=0){continue;}
						int e=a*4+c*3+d/2;
						if(e==36){
							System.out.println("男人有"+a+"个 "+"女人有"+c+"个 "+"小孩有"+d+"个");
				}
			}
		}
	}
}
class Daffodil{
	public static void main(String []args){
		for(int i=100;i<1000;i++){
			int sd=i%10; //个位数
			int td=(i%100)/10; //十位数 
			int hd=i/100; //百位数
			int dal=sd*sd*sd + td*td*td +hd*hd*hd;
				if(dal==i){
					System.out.println(i);
				}	
		}
	}
}
```

java 循环语句的章节练习2

```java
package chapter2;
import java.util.*;
public class Chapter2{
	public static void main(String [] args){
			int a=1;
			while (a<=100){
			System.out.println("好好学CoreJava,将来拿高薪");
			a++;
		}
		System.out.print(a);
	}
}
class While1{
	public static void main(String[]args){
		int a=1;
		int b=0;
		while(a<=100){
			b=a+b;
			a++;
		}
		System.out.print(b);
	}
}
class doWhile1{
	public static void main(String [] args){
		int a=1;
		int b=0;
		do{
			b=a+b;
			a++;
		}while(a<=100);
		System.out.print(b);
	}
}
class forLoop{
	public static void main(String[]args){
		int a=0;
		for(int i=1;i<=100;i++){
			if(i%2==0){
				a=a+i;
			}
		}
		System.out.println(a);
	}
}
class For2{
	public static  void main(String[] args){
		int a=0;
		for(int i=1;i<=100;i++){
			if(i%5==0&&i%10!=0){
				a=a+i;
			}
		}
		System.out.print(a);
	}
}
class ifElse1{
	public static void main(String [] args){
		Scanner s=new Scanner(System.in);
		int number=s.nextInt();
		if(number<60&& number>0){
			System.out.print("不及格");
		}
		else if(number>=60&&number<=70){
			System.out.print("及格");
		}
		else if(number>70&&number<=90){
			System.out.print("良好");
		}
		else{
			System.out.print("优秀");
		}
	}
}
class ifElse2{
	public static void main(String [] main){
		Scanner s=new Scanner(System.in);
		int number=s.nextInt();
		if(number<=6 && number>0){
			System.out.print("儿童");
		}
		else if(number<=17&&number>6){
			System.out.print("少年");
		}
		else if(number>=18&& number<=40){
			System.out.print("青年");
		}
		else if(number>=41&&number<=65){
			System.out.print("中年");
		}
		else {
			System.out.print("老年");
		}
	}
}
class Weeks{
	public static void main(String[]args){
		Scanner s =new Scanner(System.in);
		int nu=s.nextInt();
		switch(nu){
			case 1:System.out.print("星期一");break;
			case 2:System.out.print("星期二");break;
			case 3:System.out.print("星期三");break;
			case 4:System.out.print("星期四");break;
			case 5:System.out.print("星期五");break;
			case 6:System.out.print("星期六");break;
			case 7:System.out.print("星期日");break;
			default :System.out.print("输出有误，请重新输入（1-7）");
		}
	}
}
class Years{
	public static void main(String[] args){
		Scanner s=new Scanner(System.in);
		int yr=s.nextInt();
		if(yr%4==0 && yr%100!=0){
			System.out.print(yr+"是闰年");
		}
		 else if(yr%100==0 && yr%400==0){
			System.out.print(yr+"是闰年");
		}
		else{
			System.out.print(yr+"不是闰年");
		}
	}
}

```

