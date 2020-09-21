# Basic6
Ganesh Pattern

Take as input N, an odd number (>=5) . Print the following pattern as given below for N = 7.           
 
 

*  ****

*  *

*  *

*******

   *  *
   
   *  *
   
****  *

Input Format

Enter value of N ( >=5 )



Constraints

5 <= N <= 99


Output Format

Print the required pattern.


Sample Input

7

Sample Output

*  ****

*  *


*  *

*******

*  *

*  *



****  *

Explanation

Catch the pattern for the corresponding input and print it accordingly.



Solution




import java.util.*;

public class Main {

public static void main(String args[]) {

Scanner scn = new Scanner(System.in);



int n = scn.nextInt();

PattenG(n);

}



public static void PattenG(int n) {



int nsp = n / 2 - 1;

int rows = 1;

int nst = n / 2;



while (rows <= n) {



if (rows <= n / 2 + 1) {



if (rows <= n / 2) {

System.out.print("*");



int csp = 1;

while (csp <= nsp) {

System.out.print(" ");

csp++;

}

} else {

int cst = 1;

while (cst <= nst) {

System.out.print("*");

cst++;

}

}



if (rows == 1 || rows == n / 2 + 1) {



int cst = 0;

while (cst <= nst) {

System.out.print("*");

cst++;

}

} else {

System.out.print("*");

}

} else {



if (rows < n) {

int csp = 0;

while (csp <= nsp) {

System.out.print(" ");

csp++;

}

} else {

int cst = 1;

while (cst <= nst) {

System.out.print("*");

cst++;

}

}



System.out.print("*");



int csp = 1;

while (csp <= nsp) {

System.out.print(" ");

csp++;

}



System.out.print("*");



}

System.out.println();

rows++;

}

}

}



















