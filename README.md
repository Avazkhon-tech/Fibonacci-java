//# Fibonacci-java
//Implementation of Fibonacci in Java programming language

//Implementing the Fibonacci sequence in Java is a classic programming exercise. The Fibonacci sequence is a series of numbers where each number is the sum //of the two preceding ones, typically starting with 0 and 1

//1, 1, 2, 3, 5, 8, 13, 21 and so on

import java.util.Scanner;

public class Fibonacci {
    public static void main(String[] args) {
        int num1 = 1;
        int num2 = 1;
        int num3 = 0;
        Scanner input = new Scanner(System.in);
        System.out.print("Enter a number: ");
//        the number for input decides how many fibonacci numbers to show
        int range = input.nextInt();

        for (int i = 0; i < range; i++) {
            System.out.println(num1);
            num3 = num1 + num2;
            num1 = num2;
            num2 = num3;
        }
    }
}
