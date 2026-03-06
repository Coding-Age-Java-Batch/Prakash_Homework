interface Notifier {
void sendNotification(String msg);
}

class EmailNotifier implements Notifier {
public void sendNotification(String msg) {
System.out.println("Email Sent: " + msg);
}
}

class SMSNotifier implements Notifier {
public void sendNotification(String msg) {
System.out.println("SMS Sent: " + msg);
}
}

class PushNotifier implements Notifier {
public void sendNotification(String msg) {
System.out.println("Push Notification: " + msg);
}
}