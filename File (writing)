import java.util.Scanner;
import java.io.*;
public class File_Two {

public static void main(String[] args)

{


Scanner sc=new Scanner(System.in);
File fi=new File("javaa.txt");
try
{


if(fi.createNewFile())
{
System.out.println("File Created");
fi.getName();
fi.canRead();
}
else
{
System.out.println("File creation Failed");
/**fi.getName();
fi.canRead();
fi.getTotalSpace();
*/}

String content;
System.out.println("Enter the content :  ");
content=sc.nextLine();
FileOutputStream FO=new FileOutputStream(fi,true);
FO.write(content.getBytes());
FO.flush();
FO.close();
System.out.println("SAVED!!!!!!!!!!!!!!!!");
}
catch(FileNotFoundException e) {

e.printStackTrace();
}
catch(IOException e)
{
e.printStackTrace();
}


try
{
FileInputStream IP=new FileInputStream(fi);
int len=(int)fi.length();
byte[] Bytes=new byte[len];
IP.read(Bytes);
String str=new String(Bytes);
       
System.out.println("Content of first file : "+str);

IP.close();
}

catch(IOException e)
{
e.printStackTrace();
}




// Second part---------------------------------------------------------


File fil=new File("Second__Samplee.txt");
try
{

if(fil.createNewFile())
{
System.out.println("File Created");
}
else
{
System.out.println("File creation Failed");
}







FileInputStream IP=new FileInputStream(fi);
FileOutputStream NOP=new FileOutputStream(fil);

int len=(int)fi.length();
byte[] Bytes=new byte[len];
IP.read(Bytes);
for(int i=0;i<len;i++)
{
NOP.write(Bytes[i]);
}
System.out.println("File copied");
int text;
IP.close();
NOP.close();

}

catch(IOException e)
{
e.printStackTrace();
}


try
{

FileInputStream NOP=new FileInputStream(fil);
int text;
System.out.print("Content of Second File :  " +fil.getName() +"\n");
while((text=NOP.read())!=-1)
{
System.out.print((char)text);
}
NOP.close();
}

catch(IOException e)
{
e.printStackTrace();
}


}
}


/**
 *
 * OUTPUT
 * -----
 * File Created
   Enter the content :  
   hi everyone...
   SAVED!!!!!!!!!!!!!!!!
   Content of first file : hi everyone...
   File Created
   File copied
   Content of Second File :  Second__Samplee.txt
   hi everyone...
   
   //file will be created in your eclipse folder.
 */
