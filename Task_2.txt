/*Task 2: Student Grade Calculator
 
1.Input: Take marks obtained (out of 100) in each subject.
2.Calculate Total Marks: Sum up the marks obtained in all subjects.
3.Calculate Average Percentage: Divide the total marks by the total number of subjects to get the
average percentage.
4.Grade Calculation: Assign grades based on the average percentage achieved.
5.Display Results: Show the total marks, average percentage, and the corresponding grade to the user
 */

package task_2;
import java.util.*;

public class Grade_Calculator {

	public static void main(String[] args) {
		
       Scanner s= new Scanner(System.in);
       
       int math,phy,chem,bio,it;
       
       System.out.print("Enter marks obtained (out of 100) in Mathematics: ");
       math = s.nextInt();
       
       System.out.print("Enter marks obtained (out of 100) in Physics: ");
       phy = s.nextInt();
       
       System.out.print("Enter marks obtained (out of 100) in Chemistry: ");
       chem = s.nextInt();
       
       System.out.print("Enter marks obtained (out of 100) in Biology: ");
       bio = s.nextInt();
       
       System.out.print("Enter marks obtained (out of 100) in  Information Technology: ");
       it = s.nextInt();
       
       int total = math+phy+chem+bio+it;

       int subjects = 5;
       
       double percentage = (total/subjects);

       String Grade ;
       
       if(percentage<=100 && percentage>=90 )
       {
    	   Grade= "O" ;
       }
       else if(percentage<=89 && percentage>=80)
       {
    	   Grade= "A" ;
       }
       else if(percentage<=79 && percentage>=70)
       {
    	   Grade= "B" ;
       }
       else if(percentage<=69 && percentage>=60)
       {
    	   Grade= "C" ;
       }
       else if(percentage<=59 && percentage>=50)
       {
    	   Grade= "D" ;
       }
       else if(percentage<=49 && percentage>=40)
       {
    	   Grade= "E" ;
       }
       else
       {
    	   Grade="Fail";
       }
       System.out.println("Students Academic Information:");
       System.out.println("Total Marks: "+total+"\nAverage Percentage: "+percentage+"\nGrade: "+Grade); 
       s.close();
	}
}
