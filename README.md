import java.util.Scanner;
public class CurrencyConverter {
    // Exchange rates
    static double USD_TO_EUR = 0.85;
    static double EUR_TO_USD = 1.18;
    static double USD_TO_GBP = 0.75;
    static double GBP_TO_USD = 1.33;
    static double EUR_TO_GBP = 0.88;
    static double GBP_TO_EUR = 1.14;

    // Convert from USD to other currencies
    public static double convertUsdToEur(double amount) {
        return amount * USD_TO_EUR;
    }

    public static double convertUsdToGbp(double amount) {
        return amount * USD_TO_GBP;
    }

    // Convert from EUR to other currencies
    public static double convertEurToUsd(double amount) {
        return amount * EUR_TO_USD;
    }

    public static double convertEurToGbp(double amount) {
        return amount * EUR_TO_GBP;
    }

    // Convert from GBP to other currencies
    public static double convertGbpToUsd(double amount) {
        return amount * GBP_TO_USD;
    }

    public static double convertGbpToEur(double amount) {
        return amount * GBP_TO_EUR;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Currency Converter");
        System.out.println("1. USD to EUR");
        System.out.println("2. USD to GBP");
        System.out.println("3. EUR to USD");
        System.out.println("4. EUR to GBP");
        System.out.println("5. GBP to USD");
        System.out.println("6. GBP to EUR");
System.out.print("Choose an option: ");
int choice = scanner.nextInt();
System.out.print("Enter the amount: ");
double amount = scanner.nextDouble(
double convertedAmount = 0;
switch (choice) {
case 1:
convertedAmount = convertUsdToEur(amount);
System.out.println("Converted amount in EUR: " + convertedAmount);
break;
case 2:
convertedAmount = convertUsdToGbp(amount);
System.out.println("Converted amount in GBP: " + convertedAmount);
break;
case 3:
convertedAmount = convertEurToUsd(amount);
System.out.println("Converted amount in USD: " + convertedAmount);
break;
case 4:
convertedAmount = convertEurToGbp(amount);
System.out.println("Converted amount in GBP: " + convertedAmount);
break;
case 5:
convertedAmount = convertGbpToUsd(amount);
System.out.println("Converted amount in USD: " + convertedAmount);
break;
case 6:
convertedAmount = convertGbpToEur(amount);
System.out.println("Converted amount in EUR: " + convertedAmount);
break;
default:
System.out.println("Invalid choice");
}       
scanner.close();
    }
}
