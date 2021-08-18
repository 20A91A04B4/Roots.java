package pack1;
import java.util.*;
public class Roots {

	public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
	double a,b,c;
	double root1,root2;
	System.out.println("Enter a,b and c values");
	a=sc.nextDouble();
	b=sc.nextDouble();
	c=sc.nextDouble();
	double determinent = b*b-4*a*c;
	if(determinent>0)
	{
		root1=(-b+Math.sqrt(determinent))/2*a;
		root2=(-b-Math.sqrt(determinent))/2*a;
		System.out.format("root1=%.2f and root2=%.2f",root1,root2);
		
	}
	else if(determinent==0)
	{
		root1=root2=-b/(2*a);
		System.out.format("root1=root2=%.2f;",root1);
	}
	else {
	double real=-b/(2*a);
	double imaginary=Math.sqrt(-determinent)/(2*a);
	System.out.format("root1=%.2f.%2fi",real,imaginary);
	System.out.format("\n root2=%.2f.%2fi",real,imaginary);
	}

}
}
