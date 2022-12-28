import java.util.*;
abstract class Shapes11
{
	abstract void print();
	
}

class Triangle11 extends Shapes11
{
	int length,height;
	Triangle11(int l,int h)
	{
		length=l;
		height=h;
		
	}
	void print()
	{
	  double result;
	  result= 0.5*length*height;
	  System.out.println("Area of Triangle : " +result);
	}
}

class Rectangle11 extends Shapes11
{
	int length,breadth;
	Rectangle11(int l,int h)
	{
		length=l;
		breadth=h;
	}
	void print()
	{
		int result2;
		result2=length*breadth;
		System.out.println("Area of Rectangle : "+result2);
	}
}
public class AbstractClass {

	public static void main(String[] args) {
		Scanner src =new Scanner (System.in);
		int op;
		do
		{
			System.out.println("choose 1.Triangle 2.Rectangle");
			op=src.nextInt();
			switch(op)
			{
			case 1 :
				System.out.println("enter the height");
				int h=src.nextInt();
				System.out.println("enter the base");
				int b=src.nextInt();
				Triangle11 tri =new Triangle11(h,b);
				tri.print();
				break;
			case 2:
				System.out.println("enter the length");
				int l1=src.nextInt();
				System.out.println("enter the breadth");
				int b1=src.nextInt();
				Rectangle11 rec =new Rectangle11(l1,b1);
				rec.print();
				break;
			}
		}while(op==1||op==2);

	}

}

/* OUTPUT
 ------------
choose 1.Triangle 2.Rectangle
1
enter the height
3
enter the base
4
Area of Triangle : 6.0
choose 1.Triangle 2.Rectangle
2
enter the length
4
enter the breadth
9
Area of Rectangle : 36
*/
