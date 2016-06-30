# FirstProj
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {
   
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int x1 = in.nextInt();
        int v1 = in.nextInt();
        int x2 = in.nextInt();
        int v2 = in.nextInt();
        String val=null;

		if ((x1 <= 10000) || (v1 <= 10000) || (x2 <= 10000) || (v2 <= 10000)) {
			if ((x2 > x1) && (v2 > v1)) {
				val="NO";
			} else {
			 while(x1!=x2){
				 x1=x1+v1;
				 x2=x2+v2;
			 }
			 if(x1==x2){
				 val="YES";
			 }else{
				 val="NO";
			 }
				

			}
		} else {
			val="Please enter the values to be less than equal to 10000";

		}
		System.out.println(val);
        
    }
}

