# FACTORIAL-OF-A-NUMBER-USING-RECURSION
public class FactorialExample {
    // Method to find factorial using recursion
    public static int factorial(int n) {
        if (n == 0) {
            return 1; 
        }
        return n * factorial(n - 1); 
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int number = scanner.nextInt(); 
        if (number < 0) {
            System.out.println("Factorial is not possible for negative numbers.");
        } else {
            int result = factorial(number); 
            System.out.println("Factorial of " + number + " is " + result);
        }

        scanner.close(); 
    }
}

O/P
120

