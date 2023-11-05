import java.util.Scanner;
import java.util.Random;

public class NumberGuessingGame {

    public static void main(String[] args) {
        // Create a Scanner object to get user input
        Scanner scanner = new Scanner(System.in);

        // Create a Random object to generate random numbers
        Random random = new Random();

        // Define the range of the numbers to be guessed
        int min = 1;
        int max = 100;

        // Generate a random number within the range
        int number = random.nextInt(max - min + 1) + min;

        // Initialize the number of guesses and the user's guess
        int guesses = 0;
        int guess = 0;

        // Print the welcome message and the instructions
        System.out.println("Welcome to the Number Guessing Game!");
        System.out.println("I have chosen a number between " + min + " and " + max + ".");
        System.out.println("You have to guess what it is in as few attempts as possible.");

        // Loop until the user guesses the correct number or quits
        while (true) {
            // Prompt the user to enter a guess or type 0 to quit
            System.out.print("Enter your guess (or 0 to quit): ");
            guess = scanner.nextInt();

            // If the user enters 0, break the loop and end the game
            if (guess == 0) {
                System.out.println("You have quit the game. The number was " + number + ".");
                break;
            }

            // Increment the number of guesses
            guesses++;

            // Check if the user's guess is correct, too high, or too low
            if (guess == number) {
                // If correct, congratulate the user and print the number of guesses
                System.out.println("Congratulations! You have guessed the number in " + guesses + " guesses.");
                break;
            } else if (guess > number) {
                // If too high, tell the user and give a hint
                System.out.println("Your guess is too high. Try a lower number.");
            } else {
                // If too low, tell the user and give a hint
                System.out.println("Your guess is too low. Try a higher number.");
            }
        }

        // Close the scanner object
        scanner.close();
    }
}
