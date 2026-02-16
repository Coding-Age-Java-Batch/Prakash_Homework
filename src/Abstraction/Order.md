interface Order {
void processOrder();
}

class OnlineOrder implements Order {
private int orderId;
private String status;

    public OnlineOrder(int orderId) {
        this.orderId = orderId;
    }

    public void processOrder() {
        status = "Online Order Processed Successfully";
        System.out.println("Order ID: " + orderId + " | Status: " + status);
    }
}

class OfflineOrder implements Order {
private int orderId;
private String status;

    public OfflineOrder(int orderId) {
        this.orderId = orderId;
    }

    public void processOrder() {
        status = "Offline Order Processed Successfully";
        System.out.println("Order ID: " + orderId + " | Status: " + status);
    }
}

public class Main {
public static void main(String[] args) {
Order online = new OnlineOrder(101);
Order offline = new OfflineOrder(202);

        online.processOrder();
        offline.processOrder();
    }
}