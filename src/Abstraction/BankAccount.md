abstract class BankAccount {

    protected double balance;

    // Constructor
    public BankAccount(double balance) {
        this.balance = balance;
    }

    // Deposit method
    public void deposit(double amount) {
        balance += amount;
        System.out.println("Deposited: ₹" + amount);
        System.out.println("Current Balance: ₹" + balance);
    }

    // Abstract withdraw method
    abstract void withdraw(double amount);
}
class SavingsAccount extends BankAccount {

    public SavingsAccount(double balance) {
        super(balance);
    }

    public void withdraw(double amount) {
        if (amount <= balance) {
            balance -= amount;
            System.out.println("Withdrawn: ₹" + amount);
        } else {
            System.out.println("Insufficient balance! No overdraft allowed.");
        }
        System.out.println("Current Balance: ₹" + balance);
    }
}
class CurrentAccount extends BankAccount {

    private double overdraftLimit = 10000;

    public CurrentAccount(double balance) {
        super(balance);
    }

    public void withdraw(double amount) {
        if (amount <= balance + overdraftLimit) {
            balance -= amount;
            System.out.println("Withdrawn: ₹" + amount);
        } else {
            System.out.println("Overdraft limit exceeded!");
        }
        System.out.println("Current Balance: ₹" + balance);
    }
}
public class Main {
public static void main(String[] args) {

        // Create accounts with 0 initial balance
        SavingsAccount savings = new SavingsAccount(0);
        CurrentAccount current = new CurrentAccount(0);

        System.out.println("----- Savings Account -----");
        savings.deposit(5000);
        savings.withdraw(6000);

        System.out.println("\n----- Current Account -----");
        current.deposit(5000);
        current.withdraw(6000);
    }
}