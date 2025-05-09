        FIRST CODE:
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");// print hello word
    }
}



        SECOND CODE:
String a = new String("hi");
String b = new String("hi");

System.out.println(x == y);        // false: compares references
System.out.println(x.equals(y));   // true: compares string contents


        THIRD CODE:
import java.util.Scanner;

public class Addintegers{
    public static void main(String[] args) {
        int Sum=0;
        Scanner input = new Scanner(System.in);
        System.out.print("Enter first number: ");// input first number
        int num1= input.nextInt();
        System.out.print("Enter second number: ");// input second number
        int num2 = input.nextInt();
        Sum = num1 + num2;
        System.out.println("Sum is " +Sum);// display the sum of the two numbers 
    }
}


        FOURTH CODE:
int n = 20;
          if (n % 2 == 0) {
              System.out.println(n + " is       even");// display if n is even
         } else {
    System.out.println(n + " is odd");//  display if n is odd
}

        FIFTH CODE:
int a = 4, b = 6, c = 10;
           int max = a;
          if (b > max) max = b;
          if (c > max) max = c;
        System.out.println("Largest is " + max);// display the largest number



     SIXTH CODE:
import java.util.Scanner;
public class MultiplicationTable {
    public static void main(String[]args){
        int n = 2;
for (int i = 1; i <= 12; i++) {
    System.out.println(n + " x " + i + " = " + (n * i));
}

    }
}


         SEVENTH CODE:
public class Student {
 private String name;
    private String matricNo;
 private double score;
 public Student(String name, String matricNo, double score) {       this.name = name;
    this.matricNo = matricNo;
      this.score = score;
    }
public void displayInfo() {       System.out.println("Name: " + name);
     System.out.println("Matric No: " + matricNo);
       System.out.println("Score: " + score);
    }
}
// Usage:
// Student s = new Student("Alice", "A1234", 88.5);
// s.displayInfo();


       EIGHT CODE:
public class Calculator {
    public int add(int a, int b) { return a + b; }
    public double add(double a, double b) { return a + b; }
    public int add(int a, int b, int c) { return a + b + c; }
}



      NINTH CODE:
class Person {
    String name;
    public Person(String name) { this.name = name; }
    public void introduce() { System.out.println("I am " + name); }
}

class Teacher extends Person {
    String subject;
    public Teacher(String name, String subject) {
        super(name);
        this.subject = subject;
    }
    public void teach() {
        System.out.println(name + " teaches " + subject);
    }
}


    TENTH CODE:
// Bad: repeated tax calculation
double taxA = amountA * 0.05;
double taxB = amountB * 0.05;
// Good: extract method
double computeTax(double amount) {
    return amount * 0.05;
}
double taxA = computeTax(amountA);
double taxB = computeTax(amountB);


      ELEVENTH CODE:
@Test
void testAverage() {
    assertEquals(5.0, average(3, 5, 7, 4, 6));
    assertEquals(0.0, average(0, 0, 0, 0, 0));
}


      TWELVETH MONTH:
/**
 * Calculates the factorial of a non-negative integer.
 *
 * @param n the number to compute factorial for
 * @return 1 if n=0; otherwise n * factorial(n-1)
 * @throws IllegalArgumentException if n < 0
 */
public static long factorial(int n) {
    if (n < 0) throw new IllegalArgumentException("n must be >= 0");
    return (n <= 1) ? 1 : n * factorial(n - 1);
}





