# Eligibility-for-Admission

## Aim:
To write C# program to find the eligibility for admission to an engineering course

## Algorithnm:
## step1
Start by creating a new class.
## step2
Initiate the integer variables to assign the marks of Maths, Physics and Chemistry and a string variable to assign the name of the student; read the input from the user.
## step3
Calculate the first total that sums all the 3 subject marks; and the second total that sums maths and physics marks.
## step4
Based on the condition given, check whether the student is eligible for the engineering admission.
## step5
Display the output for the input read from the user.
## step6
Stop the execution.

## Program:
~~~
using System;
namespace eligible
{
    class marks
    {
        public static void Main(string[] args)
        {
            int mat, phy, chem, sum_of_three, sum_of_two;
            string name;
            Console.WriteLine("Enter the name");
            name = Console.ReadLine();
            Console.WriteLine("Enter the Math mark");
            mat = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter the Physics mark");
            phy = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter the Chemistry mark");
            chem = Convert.ToInt32(Console.ReadLine());
            sum_of_three = mat + phy + chem;
            sum_of_two = mat + phy;
            if ((mat >= 65) && (phy >= 55) && (chem >= 50))
            {
                if ((sum_of_three >= 180) || (sum_of_two >= 140))
                {
                    Console.WriteLine("{0} is Eligible for admission", name);
                }
                else
                {
                    Console.WriteLine("{0} is Not Eligible for admission", name);
                }

            }
            else
            {
                Console.WriteLine("{0} is Not Eligible for admission", name);
            }
        }
    }
}
~~~




## Output:
![image](https://github.com/Naveenvetrivel/Eligibility-for-Admission/assets/94165322/cd987e59-06d0-45b7-8d1f-cc1d3cbb1d52)
![image](https://github.com/Naveenvetrivel/Eligibility-for-Admission/assets/94165322/8bad74b9-62ab-4f12-adec-b11f38391ba6)





## Result:
Thus, a C# program to check the eligibility of a student on engineering admission has been executed successfully.
