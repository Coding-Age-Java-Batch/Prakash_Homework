interface PaymentGateway {
void pay(double amount);
}

class UPIPayment implements PaymentGateway {
public void pay(double amount) {
System.out.println("UPI Payment Successful: ₹" + amount);
}
}

class CreditCardPayment implements PaymentGateway {
public void pay(double amount) {
double finalAmount = amount + amount*0.02;
System.out.println("Credit Card Payment Successful: ₹" + finalAmount);
}
}

public class TestPayment {
public static void main(String[] args) {
PaymentGateway upi = new UPIPayment();
PaymentGateway card = new CreditCardPayment();

        upi.pay(1000);
        card.pay(1000);
    }
}