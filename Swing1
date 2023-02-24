// program for incrementing and decrementing	
import java.awt.*;
import javax.swing.*;
import java.awt.event.*;
public class Swing1 implements ActionListener{
		JButton e3,e1,e2;
		JTextField t,t1;
		JPanel p;
		JFrame f;
		Swing1(){
			f=new JFrame();
			
			
			t1=new JTextField(10);
			t1.setBounds(200, 200, 50, 50);
			e1=new JButton("increment");
			e1.setBounds(300, 300, 50, 50);
			e2=new JButton("decrement");
			e2.setBounds(300, 320, 50, 50);
			e3=new JButton("clear");
			e3.setBounds(250,130,30,30);
			p=new JPanel();
			
			
			
			p.add(t1);
			p.add(e3);
			p.add(e1);
			p.add(e2);
			f.setContentPane(p);
			
			e1.addActionListener(this);
			e2.addActionListener(this);
			e3.addActionListener(this);
			f.setSize(200, 200);
			f.setVisible(true);
			f.setLayout(null);
			
		}
		
		public void actionPerformed(ActionEvent e) {
			// TODO Auto-generated method stub
			
			if(e.getSource()==e1)
			{
				String s=t1.getText();
				int n=Integer.parseInt(s);
				int sum=0;
			        sum=n+1;
				String r=Integer.toString(sum);
				t1.setText(r);
			}
			
			if(e.getSource()==e2)
			{
				String s = t1.getText();
				int r= Integer.parseInt(s);
				int sum=0;
				sum=r-1;
				String aa=Integer.toString(sum);
				t1.setText(aa);
			}
			
			if(e.getSource()==e3)
			{
				String s=t1.getText();
				int r=Integer.parseInt(s);
				r=0;
				String a=Integer.toString(r);
				t1.setText(a);
			}
			
		}
		
		

	public static void main(String[] args) {
		// TODO Auto-generated method stub
         new Swing1();
	}

}
