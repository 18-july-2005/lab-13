import java.util.Scanner;

class BankAccount {
    String accountHolder;
    double balance;

    // Constructor
    BankAccount(String name, double initialBalance) {
        accountHolder = name;
        balance = initialBalance;
    }

    // Deposit money
    void deposit(double amount) {
        balance += amount;
        System.out.println("Amount deposited successfully.");
    }

    // Withdraw money
    void withdraw(double amount) {
        if (amount <= balance) {
            balance -= amount;
            System.out.println("Amount withdrawn successfully.");
        } else {
            System.out.println("Insufficient balance.");
        }
    }

    // Display account details
    void display() {
        System.out.println("Account Holder: " + accountHolder);
        System.out.println("Current Balance: " + balance);
    }
}

public class SimpleBankSystem {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter account holder name: ");
        String name = sc.nextLine();

        System.out.print("Enter initial balance: ");
        double balance = sc.nextDouble();

        BankAccount account = new BankAccount(name, balance);

        System.out.println("\n1. Deposit");
        System.out.println("2. Withdraw");
        System.out.println("3. View Balance");
        System.out.print("Choose option: ");
        int choice = sc.nextInt();

        if (choice == 1) {
            System.out.print("Enter amount to deposit: ");
            account.deposit(sc.nextDouble());
        } 
        else if (choice == 2) {
            System.out.print("Enter amount to withdraw: ");
            account.withdraw(sc.nextDouble());
        } 
        else if (choice == 3) {
            account.display();
        } 
        else {
            System.out.println("Invalid option.");
        }

        sc.close();
    }
}
