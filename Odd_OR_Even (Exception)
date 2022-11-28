import java.util.Scanner;

class EvenNumberException extends Exception
{
	EvenNumberException(String msg)
	{
		super(msg);
	}
}
class OddNumberException extends Exception
{
	 OddNumberException(String msg)
	{
		super(msg);
	}
}
public class Exceptiom {

	public static void main(String[] args) {
		int n;
		Scanner src=new Scanner(System.in);
		System.out.println("enter the number :  ");
		n=src.nextInt();
		
		try
		{
			 if(n%2==0) throw new EvenNumberException("even");
			 {
				 
			 } throw new OddNumberException("odd");
			 
				 
			 
		}
		catch(EvenNumberException e)
		{
			System.out.println(e.getMessage());
		}
		catch(OddNumberException e)
		{
			System.out.println(e.getMessage());
		}
		

	}

}

/*
OUTPUT
------

enter the number :  
4
even

*/
