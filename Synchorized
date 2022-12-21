import java.util.*;
public class Sync { 
	public static void main(String[] args)
	{
    Scanner sc = new Scanner(System.in);
    System.out.println("Enter the Table you want to run by thread1 : ");
    int x1 = sc.nextInt();
    System.out.println("Enter the Table you want to run by thread2 : ");
    int x2 = sc.nextInt();
    System.out.println("Enter the Table you want to run by thread3 : ");
    int x3 = sc.nextInt();
    Table t = new Table();
    Thread t1 = new Thread1(x1,t);
    Thread t2 = new Thread1(x2,t);
    Thread t3 = new Thread1(x3,t);
    t1.start();
    t2.start();
    t3.start();
    sc.close();
}
}

class Table {
synchronized void printTable(int x) {
    System.out.println(x+"'s Table started");
    for (int i = 1; i <= 5; i++) {
        System.out.println(x + " * " + i + " = " + i * x);
    }
    System.out.println(x+"'s Table finished\n");
}
}

class Thread1 extends Thread {
int x;
Table t;
Thread1(int x,Table t) {
    this.t = t;
    this.x = x;
}
public void run() {
    t.printTable(x);
}



}

//OUTPUT
//--------
/*
 * Enter the Table you want to run by thread1 : 
4
Enter the Table you want to run by thread2 : 
43
Enter the Table you want to run by thread3 : 
6
43's Table started
43 * 1 = 43
43 * 2 = 86
43 * 3 = 129
43 * 4 = 172
43 * 5 = 215
43's Table finished

6's Table started
6 * 1 = 6
6 * 2 = 12
6 * 3 = 18
6 * 4 = 24
6 * 5 = 30
6's Table finished

4's Table started
4 * 1 = 4
4 * 2 = 8
4 * 3 = 12
4 * 4 = 16
4 * 5 = 20
4's Table finished

*/
