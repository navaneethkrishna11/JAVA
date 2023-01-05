import java.util.Random;

class Number1 extends Thread
{   public void run()
	{
	  Random r = new Random ();
	  for(int i=0;i<10;i++)
	  {
		  int res=r.nextInt(100);
		  System.out.println("Random number : "+res);
		  if(res%2==0)
		  {
			  Square1 s =new Square1(res);
			  s.start();
			  
		  }
		  else
		  {
			  Cube1 c= new Cube1(res);
			  c.start();
		  }
	  }
	  try
	  {
		  Thread.sleep(100);
	  }catch(Exception e)
	  {
		  System.out.println(e);
	  }
	}
	
}

class Square1 extends Thread
{
	int n;
	Square1(int x){
		n=x;
		
	}
	public void run()
	{
		
		System.out.println("Square : "+(n*n));
	}
}

class Cube1 extends Thread{
	int n;
	Cube1(int x){
		n=x;
	}
	public void run()
	{
		System.out.println("Cube : "+(n*n*n));
	}
}
public class Sample {	
public static void main(String[] args) {

  Number1 n = new Number1();
  n.start();
	
}
}


/**
OUTPUT
-------
Random number : 47
Random number : 17
Random number : 51
Cube : 103823
Cube : 4913
Random number : 29
Cube : 132651
Random number : 89
Cube : 24389
Random number : 5
Random number : 62
Cube : 704969
Cube : 125
Random number : 10
Square : 3844
Random number : 88
Random number : 94
Square : 7744
Square : 8836
Square : 100
*/
