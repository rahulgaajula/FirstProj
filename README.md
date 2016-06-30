# FirstProj
import java.util.Scanner;

public class Test {

	public static String landing(int x1, int v1, int x2, int v2) {
		
		String val=null;

		if ((x1 <= 10000) || (v1 <= 10000) || (x2 <= 10000) || (v2 <= 10000)) {
			if ((x2 > x1) && (v2 > v1)) {
				val="No";
			} else {
			 while(x1!=x2){
				 x1=x1+v1;
				 x2=x2+v2;
			 }
			 if(x1==x2){
				 val="Yes";
			 }else{
				 val="No";
			 }
				

			}
		} else {
			val="Please enter the values to be less than equal to 10000";

		}
		return val;

	}

	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);

		System.out.println("Please enter the positions and velocities");

		int x1, v1, x2, v2;

		System.out.println("Enter the values between 1 and 10000 including");

		System.out.println(Test.landing(sc.nextInt(), sc.nextInt(), sc.nextInt(), sc.nextInt()));

	}

}
