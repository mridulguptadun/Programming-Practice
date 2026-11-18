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
{
    float s1, s2, s3, s4, s5;

    printf("Subject 1: ");
    scanf("%f", &amp;s1);

    printf("Subject 2: ");
    scanf("%f", &amp;s2);

    printf("Subject 3: ");
    scanf("%f", &amp;s3);

    printf("Subject 4: ");
    scanf("%f", &amp;s4);

    printf("Subject 5: ");
    scanf("%f", &amp;s5);

    float total = s1 + s2 + s3 + s4 + s5;

    float average = total / 5;

    float percentage = (total / 500) * 100;

    printf("Total Marks: %.2f\n", total);
    printf("Average Marks: %.2f\n", average);
    printf("Percentage: %.2f%%\n", percentage);

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Subject 1: ");
        double s1 = sc.nextDouble();

        System.out.print("Subject 2: ");
        double s2 = sc.nextDouble();

        System.out.print("Subject 3: ");
        double s3 = sc.nextDouble();

        System.out.print("Subject 4: ");
        double s4 = sc.nextDouble();

        System.out.print("Subject 5: ");
        double s5 = sc.nextDouble();

        double total = s1 + s2 + s3 + s4 + s5;

        double average = total / 5;

        double percentage = (total / 500) * 100;

        System.out.printf("Total Marks: %.2f%n", total);
        System.out.printf("Average Marks: %.2f%n", average);
        System.out.printf("Percentage: %.2f%%%n", percentage);

        sc.close();
    }
}</code></pre></td>
</tr>
</table>

Q4. Swap Two Variables Using a Third Variable
Write a program to input two numbers and swap their values using a third temporary variable.

Sample Input
Enter A: 10
Enter B: 20


Expected Output
Before Swapping:
A = 10
B = 20

After Swapping:
A = 20
B = 10



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code>a = int(input("Enter A: "))
b = int(input("Enter B: "))

print("Before Swapping:")
print("A =", a)
print("B =", b)

# Swap using temporary variable

temp = a
a = b
b = temp

print("After Swapping:")
print("A =", a)
print("B =", b)</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()
{
    int a, b, temp;

    printf("Enter A: ");
    scanf("%d", &amp;a);

    printf("Enter B: ");
    scanf("%d", &amp;b);

    printf("Before Swapping:\n");
    printf("A = %d\n", a);
    printf("B = %d\n", b);

    // Swap using temporary variable

    temp = a;
    a = b;
    b = temp;

    printf("After Swapping:\n");
    printf("A = %d\n", a);
    printf("B = %d\n", b);

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        int a, b, temp;

        System.out.print("Enter A: ");
        a = sc.nextInt();

        System.out.print("Enter B: ");
        b = sc.nextInt();

        System.out.println("Before Swapping:");
        System.out.println("A = " + a);
        System.out.println("B = " + b);

        // Swap using temporary variable

        temp = a;
        a = b;
        b = temp;

        System.out.println("After Swapping:");
        System.out.println("A = " + a);
        System.out.println("B = " + b);

        sc.close();
    }
}</code></pre></td>
</tr>
</table>




Q5. Swap Two Variables Without a Third Variable
Write a program to input two integer numbers and swap their values without using a third variable. Use arithmetic operators.

Sample Input
Enter A: 15
Enter B: 25


Expected Output
Before Swapping:
A = 15
B = 25

After Swapping:
A = 25
B = 15



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code>a = int(input("Enter A: "))
b = int(input("Enter B: "))

print("Before Swapping:")
print("A =", a)
print("B =", b)

# Swap without third variable

a = a + b
b = a - b
a = a - b

print("After Swapping:")
print("A =", a)
print("B =", b)</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()
{
    int a, b;

    printf("Enter A: ");
    scanf("%d", &amp;a);

    printf("Enter B: ");
    scanf("%d", &amp;b);

    printf("Before Swapping:\n");
    printf("A = %d\n", a);
    printf("B = %d\n", b);

    // Swap without third variable

    a = a + b;
    b = a - b;
    a = a - b;

    printf("After Swapping:\n");
    printf("A = %d\n", a);
    printf("B = %d\n", b);

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter A: ");
        int a = sc.nextInt();

        System.out.print("Enter B: ");
        int b = sc.nextInt();

        System.out.println("Before Swapping:");
        System.out.println("A = " + a);
        System.out.println("B = " + b);

        // Swap without third variable

        a = a + b;
        b = a - b;
        a = a - b;

        System.out.println("After Swapping:");
        System.out.println("A = " + a);
        System.out.println("B = " + b);

        sc.close();
    }
}</code></pre></td>
</tr>
</table>



Note: Arithmetic swapping can overflow for large integer values. It is useful for understanding operators, but a temporary variable is generally safer.

Q6. Calculate Area and Circumference of a Circle
Write a program to input the radius of a circle and calculate its area and circumference.

Formula
\[
Area = \pi r^2
\]

\[
Circumference = 2\pi r
\]

Sample Input
Enter radius: 7


Expected Output
Area = 153.94
Circumference = 43.98



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code>import math

# Input radius

radius = float(input("Enter radius: "))

# Calculate area

area = math.pi * radius ** 2

# Calculate circumference

circumference = 2 * math.pi * radius

# Display results

print("Area =", round(area, 2))
print("Circumference =", round(circumference, 2))</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()
{
    float radius;
    float area, circumference;

    const float PI = 3.14159265;

    // Input radius

    printf("Enter radius: ");
    scanf("%f", &amp;radius);

    // Calculate area

    area = PI * radius * radius;

    // Calculate circumference

    circumference = 2 * PI * radius;

    // Display results

    printf("Area = %.2f\n", area);
    printf("Circumference = %.2f\n", circumference);

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        final double PI = Math.PI;

        // Input radius

        System.out.print("Enter radius: ");
        double radius = sc.nextDouble();

        // Calculate area

        double area = PI * Math.pow(radius, 2);

        // Calculate circumference

        double circumference = 2 * PI * radius;

        // Display results

        System.out.printf("Area = %.2f%n", area);
        System.out.printf("Circumference = %.2f%n", circumference);

        sc.close();
    }
}</code></pre></td>
</tr>
</table>




Q7. Calculate Simple Interest
Write a program to input the principal amount, annual interest rate, and time in years. Calculate simple interest and total amount.

Formula
\[
SI = \frac{P \times R \times T}{100}
\]

\[
Total = P + SI
\]

Sample Input
Principal Amount: 10000
Interest Rate: 5
Time: 2


Expected Output
Simple Interest = 1000.00
Total Amount = 11000.00



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code># Input details

principal = float(input("Principal Amount: "))
rate = float(input("Interest Rate: "))
time = float(input("Time in years: "))

# Calculate simple interest

simple_interest = (
    principal * rate * time
) / 100

# Calculate total amount

total_amount = principal + simple_interest

# Display results

print(
    "Simple Interest =",
    round(simple_interest, 2)
)

print(
    "Total Amount =",
    round(total_amount, 2)
)</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()
{
    float principal, rate, time;
    float simple_interest, total_amount;

    // Input details

    printf("Principal Amount: ");
    scanf("%f", &amp;principal);

    printf("Interest Rate: ");
    scanf("%f", &amp;rate);

    printf("Time in years: ");
    scanf("%f", &amp;time);

    // Calculate simple interest

    simple_interest =
        (principal * rate * time) / 100;

    // Calculate total amount

    total_amount = principal + simple_interest;

    // Display results

    printf("Simple Interest = %.2f\n", simple_interest);
    printf("Total Amount = %.2f\n", total_amount);

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        // Input details

        System.out.print("Principal Amount: ");
        double principal = sc.nextDouble();

        System.out.print("Interest Rate: ");
        double rate = sc.nextDouble();

        System.out.print("Time in years: ");
        double time = sc.nextDouble();

        // Calculate simple interest

        double simpleInterest =
            (principal * rate * time) / 100;

        // Calculate total amount

        double totalAmount = principal + simpleInterest;

        // Display results

        System.out.printf("Simple Interest = %.2f%n", simpleInterest);
        System.out.printf("Total Amount = %.2f%n", totalAmount);

        sc.close();
    }
}</code></pre></td>
</tr>
</table>




Q8. Convert Celsius to Fahrenheit
Write a program to input temperature in Celsius and convert it into Fahrenheit.

Formula
\[
F = (C \times \frac{9}{5}) + 32
\]

Sample Input
Enter temperature in Celsius: 37


Expected Output
Temperature in Fahrenheit = 98.60



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code># Input temperature

celsius = float(
    input("Enter temperature in Celsius: ")
)

# Convert Celsius to Fahrenheit

fahrenheit = (celsius * 9 / 5) + 32

# Display result

print(
    "Temperature in Fahrenheit =",
    round(fahrenheit, 2)
)</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()
{
    float celsius, fahrenheit;

    // Input temperature

    printf("Enter temperature in Celsius: ");
    scanf("%f", &amp;celsius);

    // Convert Celsius to Fahrenheit

    fahrenheit = (celsius * 9.0 / 5.0) + 32;

    // Display result

    printf(
        "Temperature in Fahrenheit = %.2f\n",
        fahrenheit
    );

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        // Input temperature

        System.out.print("Enter temperature in Celsius: ");
        double celsius = sc.nextDouble();

        // Convert Celsius to Fahrenheit

        double fahrenheit =
            (celsius * 9.0 / 5.0) + 32;

        // Display result

        System.out.printf(
            "Temperature in Fahrenheit = %.2f%n",
            fahrenheit
        );

        sc.close();
    }
}</code></pre></td>
</tr>
</table>




Q9. Convert Seconds into Hours, Minutes and Seconds
Write a program to input total seconds and convert them into hours, minutes, and remaining seconds using arithmetic operators.

Sample Input
Enter total seconds: 3675


Expected Output
Hours: 1
Minutes: 1
Seconds: 15


Logic
- Hours = Total Seconds // 3600
- Remaining Seconds = Total Seconds % 3600
- Minutes = Remaining Seconds // 60
- Seconds = Remaining Seconds % 60

<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code># Input total seconds

total_seconds = int(
    input("Enter total seconds: ")
)

# Calculate hours

hours = total_seconds // 3600

# Calculate remaining seconds

remaining_seconds = total_seconds % 3600

# Calculate minutes

minutes = remaining_seconds // 60

# Calculate final seconds

seconds = remaining_seconds % 60

# Display results

print("Hours:", hours)
print("Minutes:", minutes)
print("Seconds:", seconds)</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;

int main()
{
    int total_seconds;
    int hours, minutes, seconds;
    int remaining_seconds;

    // Input total seconds

    printf("Enter total seconds: ");
    scanf("%d", &amp;total_seconds);

    // Calculate hours

    hours = total_seconds / 3600;

    // Calculate remaining seconds

    remaining_seconds = total_seconds % 3600;

    // Calculate minutes

    minutes = remaining_seconds / 60;

    // Calculate final seconds

    seconds = remaining_seconds % 60;

    // Display results

    printf("Hours: %d\n", hours);
    printf("Minutes: %d\n", minutes);
    printf("Seconds: %d\n", seconds);

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        // Input total seconds

        System.out.print("Enter total seconds: ");
        int totalSeconds = sc.nextInt();

        // Calculate hours

        int hours = totalSeconds / 3600;

        // Calculate remaining seconds

        int remainingSeconds = totalSeconds % 3600;

        // Calculate minutes

        int minutes = remainingSeconds / 60;

        // Calculate final seconds

        int seconds = remainingSeconds % 60;

        // Display results

        System.out.println("Hours: " + hours);
        System.out.println("Minutes: " + minutes);
        System.out.println("Seconds: " + seconds);

        sc.close();
    }
}</code></pre></td>
</tr>
</table>




Q10. Demonstrate Different Data Types
Write a program to declare and initialize variables of different data types: integer, floating-point, character, string, and boolean. Display their values.

Sample Input

No user input required.

Expected Output
Integer: 100
Float: 25.5
Character: A
String: Programming
Boolean: True



<table>
<tr><th>Python</th><th>C</th><th>Java</th></tr>
<tr>
<td valign="top"><pre><code># Declare variables

integer_value = 100
float_value = 25.5
character_value = 'A'
string_value = "Programming"
boolean_value = True

# Display values

print("Integer:", integer_value)
print("Float:", float_value)
print("Character:", character_value)
print("String:", string_value)
print("Boolean:", boolean_value)</code></pre></td>
<td valign="top"><pre><code>#include &lt;stdio.h&gt;
#include &lt;stdbool.h&gt;

int main()
{
    // Declare variables

    int integer_value = 100;
    float float_value = 25.5;
    char character_value = 'A';
    char string_value[] = "Programming";
    bool boolean_value = true;

    // Display values

    printf("Integer: %d\n", integer_value);
    printf("Float: %.1f\n", float_value);
    printf("Character: %c\n", character_value);
    printf("String: %s\n", string_value);
    printf("Boolean: %s\n",
           boolean_value ? "True" : "False");

    return 0;
}</code></pre></td>
<td valign="top"><pre><code>public class Main
{
    public static void main(String[] args)
    {
        // Declare variables

        int integerValue = 100;
        float floatValue = 25.5f;
        char characterValue = 'A';
        String stringValue = "Programming";
        boolean booleanValue = true;

        // Display values

        System.out.println("Integer: " + integerValue);
        System.out.println("Float: " + floatValue);
        System.out.println("Character: " + characterValue);
        System.out.println("String: " + stringValue);
        System.out.println("Boolean: " + booleanValue);
    }
}</code></pre></td>
</tr>
</table>


