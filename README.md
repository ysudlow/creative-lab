#import java.util.Scanner;

public class UserInputScript {
    public static void main(String[] args) {
        // Create a Scanner object to read user input
        Scanner scanner = new Scanner(System.in);

        // Prompt the user for input
        System.out.print("Please enter your name: ");

        // Read the user's input as a string
        String userName = scanner.nextLine();

        // Display a greeting using the user's input
        System.out.println("Hello, " + userName + "!");
        
        System.out.println("Do you prefer cats or dogs? ");

        // Read the user's input as a string
        String petPreference = scanner.nextLine();
        
        // Compare the user's input (case-insensitive) and provide a response
        if (petPreference.equalsIgnoreCase("dog")) {
            System.out.println("Woof!");
        } else if (petPreference.equalsIgnoreCase("cat")) {
            System.out.println("Meow!");
        } else {
            System.out.println("I'm not sure what sound that animal makes.");
        }
        
        System.out.print("How many " + petPreference + "s do you have? ");
        // Read the user's input as an integer
        int petCount = scanner.nextInt();
        
        // Provide a response based on the number of pets
        if (petCount == 1) {
            System.out.println("You have " + petCount + " " + petPreference + ".");
        } else if (petCount == 2) {
            System.out.println("You have " + petCount + " " + petPreference + "s.");
        } else if (petCount > 2) {
            System.out.println("You have " + petCount + " " + petPreference + "s.");
        } else {
            System.out.println("I'm not sure how many " + petPreference + "s you have.");
        }

        // Close the scanner to release resources
        scanner.close();
    }
} creative-lab