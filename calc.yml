import java.util.Scanner;

public class Calculator {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("Simple Calculator");
        System.out.println("-----------------");

        while (true) {
            System.out.print("Enter first number: ");
            double num1 = input.nextDouble();

            System.out.print("Enter an operator (+, -, *, /): ");
            char operator = input.next().charAt(0);

            System.out.print("Enter second number: ");
            double num2 = input.nextDouble();

            double result;

            switch (operator) {
                case '+':
                    result = num1 + num2;
                    break;
                case '-':
                    result = num1 - num2;
                    break;
                case '*':
                    result = num1 * num2;
                    break;
                case '/':
                    if (num2 == 0) {
                        System.out.println("Cannot divide by zero.");
                        continue;
                    }
                    result = num1 / num2;
                    break;
                default:
                    System.out.println("Invalid operator.");
                    continue;
            }

            System.out.println("Result: " + result);

            System.out.print("Do you want to continue? (yes/no): ");
            String choice = input.next();
            if (!choice.equalsIgnoreCase("yes")) {
                break;
            }
        }

        System.out.println("Thank you for using the calculator!");
        input.close();
    }
}
