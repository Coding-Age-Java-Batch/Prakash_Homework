interface Logger {
void log(String message);
}

class ConsoleLogger implements Logger {
public void log(String message) {
System.out.println("Console Log: " + message);
}
}

class FileLogger implements Logger {
public void log(String message) {
System.out.println("File Log: " + message);
}
}

class DatabaseLogger implements Logger {
public void log(String message) {
System.out.println("Database Log: " + message);
}
}