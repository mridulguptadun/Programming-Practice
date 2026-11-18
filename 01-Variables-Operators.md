

# Topic 01: Variables and Operators

## Question 1: Add Two Numbers

**Question:**

Write a program to input two numbers and calculate their sum.

**Sample Input:**

    Enter first number: 10
    Enter second number: 20

**Expected Output:**

    Sum = 30

## Python | C | Java

<table>
<tr>
<th>Python</th>
<th>C</th>
<th>Java</th>
</tr>
<tr>
<td valign="top">

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

sum = a + b

print("Sum =", sum)
```

</td>
<td valign="top">

```c
#include <stdio.h>

int main()
{
    int a, b, sum;

    printf("Enter first number: ");
    scanf("%d", &a);

    printf("Enter second number: ");
    scanf("%d", &b);

    sum = a + b;

    printf("Sum = %d", sum);

    return 0;
}
```

</td>
<td valign="top">

```java
import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        int a, b, sum;

        System.out.print("Enter first number: ");
        a = sc.nextInt();

        System.out.print("Enter second number: ");
        b = sc.nextInt();

        sum = a + b;

        System.out.println("Sum = " + sum);

        sc.close();
    }
}
```

</td>
</tr>
</table>
