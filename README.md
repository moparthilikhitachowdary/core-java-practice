# core-java-practice
import java.util.Scanner;
public class armstrong {
	public static void main(String[] args) {
		
		Scanner s=new Scanner(System.in);
		System.out.println("Enter a number ");
		int num=s.nextInt();
		int temp=num;
		int rem=0,digits=0,sum=0;
		while(temp!=0) {
			temp=temp/10;
			digits++;
		}
		temp=num;
		while(temp!=0) {
			rem=temp%10;
			
			sum=sum+(int)Math.pow(rem,digits);
			temp=temp/10;
		}
		System.out.println(sum);
		System.out.println(num);
		if(sum==num) {
			System.out.println("armstrong");
		}
		else {
			System.out.println("not armstrong");
		}
	}	
}
