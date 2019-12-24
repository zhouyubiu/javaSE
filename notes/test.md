#hello

```java
package bsaic;

import sun.lwawt.macosx.CSystemTray;

import java.util.Scanner;

public class Java_01 {
    public Java_01() {
        System.out.println("构造函数");
    }
    public int[] test(int []list){
        int [] a=new int[list.length];
        int count = 0;
        for (int i:list){
            System.out.println(i);
            System.out.println(list.length);
            a[count++]=i++;
        }
        return a;
    }

    public static void main(String[] args) {
        System.out.println("heelo,world");
        Java_01 obj = new Java_01();
        int a=1,b=1;
//        b=a++;
        b = ++a;
        System.out.println(a);
        System.out.println(b);


        int []arry=new int[5];
        arry[1]=3;
        System.out.println(arry[2]);
        System.out.println(arry.length);
//        for (int i=0;i<arry.length;i++){
//            System.out.println(arry[i]);
//        }
        for(int i:arry){
            System.out.println(i+"lllllllllllll");
        }
        Java_01 J = new Java_01();
        int []p=J.test(arry);
        System.out.println(p[2]);

        Scanner scan = new Scanner(System.in);
        if (scan.hasNext()) {
            String str1 = scan.next();
            System.out.println("输入的数据为：" + str1);
        }
        scan.close();
    }
}

```