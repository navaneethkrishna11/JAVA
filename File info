import java.io.IOException;
import java.util.Scanner;
import java.io.File;

public class File_details {
	public static void main(String [] args)throws IOException
	{
		Scanner src =new Scanner (System.in);
		System.out.print("enter the file name : ");
		String n=src.nextLine();
		File f =new File(n);
		if(f.createNewFile())
		{
			System.out.println("file name : "+f.getName());
			
			System.out.println("file parent : "+f.getParent());
			
			System.out.println("file path : "+f.getPath());
			System.out.println("file space : "+f.getTotalSpace());
			
		}
		if(f.exists())
		{
			System.out.println("file readable : "+f.canRead());
			System.out.println("file writable : "+f.canWrite());


			
			System.out.println("file directory : "+f.isDirectory());


		}
	}

}

/**
 * OUTPUT
 * ------
 * enter the file name : RAF
file name : RAF
file parent : null
file path : RAF
file space : 324551045120
file readable : true
file writable : true
file directory : false
*/
