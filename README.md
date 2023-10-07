 Reset some default styles */
body, h1, h2, ul, p {
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
}

/* Header styles */
header {
    background-color: #333;
    color: #fff;
    padding: 10px 0;
    text-align: center;
}

header h1 {
    font-size: 36px;
}

nav ul {
    list-style-type: none;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav a {
    text-decoration: none;
    color: #fff;
    font-weight: bold;
}

/* Hero section styles */
.hero {
    background-image: url('your-hero-image.jpg');
    background-size: cover;
    text-align: center;
    padding: 100px 0;
}

.hero h2 {
    font-size: 48px;
    margin-bottom: 20px;
}

.hero p {
    font-size: 24px;
    margin-bottom: 40px;
}

.cta-button {
    display: inline-block;
    background-color: #ff6600;
    color: #fff;
    padding: 10px 20px;
    text-decoration: none;
    font-weight: bold;
    font-size: 18px;
    border-radius: 5px;
}

/* Products section styles */
.products {
    /* Add styles for your product listings */
}

/* Footer styles */
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px 0;
}
Ques 1. WAP to swap first and last digit of any number.
#include <iostream>
using namespace std;
int main() {
    int number, originalNumber, firstDigit, lastDigit, swappedNumber = 0, divisor = 1, multiplier = 1;
        cout<<"\nAryan";
    cout<<"\n03713702022";
    cout << "\nEnter a number: ";
    cin >> number;
    originalNumber = number; 
    lastDigit = number % 10;
    number /= 10;
    while (number > 0) {
        divisor *= 10;
        firstDigit = number % 10;
        number /= 10;
    }
    swappedNumber = lastDigit * divisor + originalNumber % (divisor / 10);
    swappedNumber += firstDigit * multiplier;
    cout << "Original number: " << originalNumber << endl;
    cout << "Number after swapping first and last digits: " << swappedNumber << endl;    
    return 0;
}
Output:  

Ques 2. WAP to print gender according to given by user
#include <iostream>
#include <string>
using namespace std;
int main() {
    string gender;
    cout <<"\nAryan";
    cout <<"\n03713702022";
    cout <<"\nPlease enter your gender (male/female/other): ";
    cin >> gender;
    if (gender == "male" || gender == "Male" || gender == "MALE") {
        cout << "You are a male." << std::endl;
    } else if (gender == "female" || gender == "Female" || gender == "FEMALE") {
        cout << "You are a female." << std::endl;
    } else {
        cout << "You identified as: " << gender << std::endl;
    }

    return 0;
}
Output: 
 




Ques 3. WAP to find hcf of two numbers
#include <iostream>
using namespace std;
int findHCF(int a, int b) {
    while (b != 0) {
        int temp = b;
        b = a % b;
        a = temp;
    }
    return a;
}
int main() {
    int num1, num2;
    cout<<"\nAryan";
    cout<<"\n03713702022";
    cout << "\nEnter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    int hcf = findHCF(num1, num2);
    cout << "The HCF of " << num1 << " and " << num2 << " is " << hcf << std::endl;
    return 0;
}
Output:
 

Ques 4.  Wap to find maximum number using friend function
#include <iostream>
using namespace std;
int main() {
    int n;
    cout << "\nAryan";
    cout << "\n03713702022";
    cout << "\nEnter the number of elements: ";
    cin >> n;
    if (n <= 0) {
        cout << "Invalid input. Please enter a positive number of elements." << endl;
        return 1; 
    }
    int maxNum, num;
    cout << "Enter the first number: ";
    cin >> maxNum;
    for (int i = 1; i < n; ++i) {
        cout << "Enter the next number: ";
        cin >> num;
        if (num > maxNum) {
            maxNum = num;
        }
    }
    cout << "The maximum number is: " << maxNum << endl;
    return 0;
}
OUTPUT:
 
Ques 5. Define a class counter which contains an int variable count defined as static and a static function Display() to display the value of count. Whenever an object of this class is created count is incremented by 1. Use this class in main to create multiple object of this class and display the value of count each time.
#include <iostream>
using namespace std;
class Counter {
public:
    static int count; 
    Counter() {
        count++; 
    }
    static void Display() {
        cout << "Count: " << count << std::endl;
    }
};
int Counter::count = 0;
int main() {
    cout << "\nAryan";
    cout << "\n03713702022\n";
    Counter::Display();
    Counter obj1;
    Counter::Display(); 
    Counter obj2; 
    Counter::Display();
    Counter obj3;
    Counter::Display();
    return 0;
}
OUTPUT:
 AIM: Write the meaning and significance of SPSS

MEANING :
For data management, sophisticated analytics, multivariate analysis, corporate intelligence, and criminal investigation, IBM created the statistical software suite SPSS Statistics. It was long manufactured by SPSS Inc. before being purchased by IBM in 2009. Software updates since 2015 have gone under the name IBM SPSS Statistics.
The software's initial name, which reflected its target market, was Statistical Package for the Social Sciences (SPSS), which was eventually modified to Statistical Product and Service Solutions.
SPSS is a popular program for statistical analysis in social science is. Market researchers, health researchers, survey firms, the government, marketing groups, researchers in education, and others also utilize it. 
One of "sociology's most influential books" has been called the original SPSS manual (Nie, Bent & Hull, 1970) because it made it possible for regular researchers to conduct their own statistical analysis. 
The base software also includes tools for statistical analysis, data management (case selection, file reshaping, and producing derived data), and data documentation (a metadata dictionary is saved in the data file).
Two viewpoints on the graphical user interface can be switched in between:
•	'Data View' In contrast to spreadsheets, data cells can only store text or numbers; formulas cannot be put in data cells. 
•	The 'Variable View' shows the metadata dictionary, with each row denoting a variable and displaying its name, variable label, value label(s), print width, measurement type, and a number of additional details. 

IMPORTANCE:
•	Prepare and analyze data through an intuitive user interface without having to write code using drag-and-drop.
•	Integrated with open source
•	Enhance SPSS syntax with R and Python using a library of extensions or by building your own.
•	Comprehensive
•	Run descriptive statistics and regression analyses, view patterns of missing data and summarize variable distributions with an integrated interface.
•	 Easy to use 



INTERFACE:

•	This is the basic screen view the user first gets to see .
 


•	This the data view where the data is received from the user 

 

•	Then is the variable view where all the headers are entered and their values are stored 
 


•	Then comes the different scale and their uses 
 

•	First is the nominal scale :

 

•	A nominal scale is one in which a variable represents a value with no intrinsic ranking.
•	Example : region, zip code, gender 

•	Next is the ordinal scale

 

•	It is used for those data which can be ranked like for level of satisfaction, level of service 
Q1. Write a program to find simple interest ?
Ans. #include<stdio.h>
        #include<conio.h>
        void main()
        { int a,b,c,d;
        clrscr();
        printf("Enter Principle amount :");
        scanf("%d",&a);
       printf("Enter Rate : ");
       scanf("%d",&b);
       printf("Enter Time Duration : ");
       scanf("%d",&c);
       d=(a*b*c)/100;
       printf("Simple Intrest :%d ",d);
       getch();
       }
 

Q2. To perform arithmetic operation on two numbers ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
{ int a,b;
clrscr();
printf("Enter a no. : ");
scanf("%d",&a);
printf("Enter another no. : ");
scanf("%d",&b);
a=a+b;
b=a-b;
a=a-b;
printf("%d, %d",a, b);
getch();
}
  
Q3. To find area and circumference of circle ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
{ float a,b,c;
clrscr();
printf("Enter the raius of the circle : ");
scanf("%f",&a);
b=6.28*a;
c=3.14*a*a;
printf("Circumference :%f\n",b);
printf("Area :%f\n",c);
getch();
}
 


Q4. Write a program to find total percentage of four subjects of a student ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
int A,B,C,D,E,F;
clrscr();
printf("ENTER 1ST SUBJECT MARKS :"); scanf("%d", &A);
printf("ENTER 2ND SUBJECT MARKS :");
scanf("%d", &B);
printf ("ENTER 3RD SUBJECT MARKS :"); scanf("%d", &C);
printf("ENTER 4TH SUBJECT MARKS :");
scanf ("%d", &D);
E=A+B+C+D;
F-E-100/400;
printf("SUM OF A,B,C AND D=zd \n",E); printf ("PERCENTAGE OF E=%d",F);
getch();
}
 	
Q5. Write a program to multiply two floating numbers ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
{ float a,b,c;
printf("Enter a no. : ");
scanf("%f",&a);
printf("Enter another no. : ");
scanf("%f",&b);
c=a*b;
printf("Product of a and b = %f",c);
getch();
}
 

	



Q7. Write a program to find size of int, float, double and char ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
{ int a;
float b;
char c;
double d;
clrscr();
printf("int size = %d\n",sizeof(int));
printf("float size = %d\n",sizeof(float));
printf("char size = %d\n",sizeof(char));
printf("double size = %d\n",sizeof(double));
getch();
}
 


Q8. Write a program to find ASCII value of character ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
{ char ch;
clrscr();
printf("Enter the character : ");
scanf("%c",&ch);
printf("ASCII value of %c is %d",ch,ch);
getch();
}
 





Q9. Write a program to print area & perimeter of rectangle ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
{ int a,b,c,d;
printf("Enter length : ");
scanf("%d",&a);
printf("Enter breadth : ");
scanf("%d",&b);
c=2*(a+b);
d=a*b;
printf("Area of the rectangle : %d\n",d);
printf("Perimeter of the rectangle : %d\n",c);
getch();
}
 

Q10. Write a program to swap two no’s with and without using third variable ?
Ans. #include<stdio.h>
#include<conio.h>
void main()
{ int a,b;
clrscr();
printf("Enter a no. : ");
scanf("%d",&a);
printf("Enter another no. : ");
scanf("%d",&b);
a=a+b;
b=a-b;
a=a-b;
printf("%d, %d",a, b);
getch();
}
 
	With 3rd variable
void main()
{ int a,b,c;
clrscr();
printf("Enter a no. : ");
scanf("%d",&a);
printf("Enter another no. : ");
scanf("%d",&b);
c=a;
a=b;
b=c;
printf("%d, %d",a, b);
getch();
}
 
	

Q11. Write a program to find compound interest ?
Ans. #include <math.h>
#include <stdio.h>
#include<conio.h>
void main()
{ int p,r,t,a;
clrscr();
printf("Enter principle amount : ");
scanf("%d",&p);
printf("Enter rate : ");
scanf("%d",&r);
printf("Enter Time duration : ");
scanf("%d",&t);
a=p*(pow((1+r/100),t));
printf("The Compound Intrest is :%d\n ",a);
getch();
}





