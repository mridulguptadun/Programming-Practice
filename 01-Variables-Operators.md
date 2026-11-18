Q1. Store and Display Student Information
Write a program to input a student's name, age, and percentage and display the information.

Sample Input
Rahul
21
85.5


Expected Output
Student Name: Rahul
Age: 21
Percentage: 85.5



<table>
<tr>
<th width="33%">Python</th>
<th width="33%">C</th>
<th width="33%">Java</th>
</tr>
<tr>
<td valign="top">
<pre><code>name = input("Enter name: ")

age = int(input("Enter age: "))

percentage = float(
    input("Enter percentage: ")
)

print("Student Name:", name)
print("Age:", age)
print("Percentage:", percentage)</code></pre>
</td>
<td valign="top">
<pre><code>#include &lt;stdio.h&gt;

int main()
{
    char name[50];
    int age;
    float percentage;

    printf("Enter name: ");
    scanf("%49s", name);

    printf("Enter age: ");
    scanf("%d", &amp;age);

    printf("Enter percentage: ");
    scanf("%f", &amp;percentage);

    printf("Student Name: %s\n", name);
    printf("Age: %d\n", age);
    printf("Percentage: %.2f\n", percentage);

    return 0;
}</code></pre>
</td>
<td valign="top">
<pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter name: ");
        String name = sc.nextLine();

        System.out.print("Enter age: ");
        int age = sc.nextInt();

        System.out.print("Enter percentage: ");
        double percentage = sc.nextDouble();

        System.out.println("Student Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Percentage: " + percentage);

        sc.close();
    }
}</code></pre>
</td>
</tr>
</table>




Q2. Perform Basic Arithmetic Operations
Write a program to input two numbers and calculate addition, subtraction, multiplication, division, and modulus.

Sample Input
First Number: 20
Second Number: 6


Expected Output
Addition: 26
Subtraction: 14
Multiplication: 120
Division: 3.3333
Modulus: 2



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code>a = float(input("First number: "))
b = float(input("Second number: "))

addition = a + b
subtraction = a - b
multiplication = a * b

division = a / b
modulus = a % b

print("Addition:", addition)
print("Subtraction:", subtraction)
print("Multiplication:", multiplication)
print("Division:", round(division, 4))
print("Modulus:", modulus)</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()
{
    int a, b;

    printf("First number: ");
    scanf("%d", &amp;a);

    printf("Second number: ");
    scanf("%d", &amp;b);

    int addition = a + b;
    int subtraction = a - b;
    int multiplication = a * b;

    float division = (float)a / b;
    int modulus = a % b;

    printf("Addition: %d\n", addition);
    printf("Subtraction: %d\n", subtraction);
    printf("Multiplication: %d\n", multiplication);
    printf("Division: %.4f\n", division);
    printf("Modulus: %d\n", modulus);

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("First number: ");
        int a = sc.nextInt();

        System.out.print("Second number: ");
        int b = sc.nextInt();

        int addition = a + b;
        int subtraction = a - b;
        int multiplication = a * b;

        double division = (double)a / b;
        int modulus = a % b;

        System.out.println("Addition: " + addition);
        System.out.println("Subtraction: " + subtraction);
        System.out.println("Multiplication: " + multiplication);
        System.out.printf("Division: %.4f%n", division);
        System.out.println("Modulus: " + modulus);

        sc.close();
    }
}</code></pre></td>
</tr>
</table>




Q3. Calculate Total, Average and Percentage
Write a program to input marks of five subjects and calculate total marks, average marks, and percentage. Each subject carries 100 marks.

Sample Input
Subject 1: 85
Subject 2: 90
Subject 3: 78
Subject 4: 88
Subject 5: 79


Expected Output
Total Marks: 420
Average Marks: 84.00
Percentage: 84.00%



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code>s1 = float(input("Subject 1: "))
s2 = float(input("Subject 2: "))
s3 = float(input("Subject 3: "))
s4 = float(input("Subject 4: "))
s5 = float(input("Subject 5: "))

total = s1 + s2 + s3 + s4 + s5

average = total / 5

percentage = (total / 500) * 100

print("Total Marks:", total)
print("Average Marks:", round(average, 2))
print("Percentage:", round(percentage, 2), "%")</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()

