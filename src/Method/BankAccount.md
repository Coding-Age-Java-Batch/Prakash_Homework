public class BankAccount {

    String accountHolderNAme;
    String acountNumber;
    double Balacne;

    void setAccountDetails(String name , String accno , double balacne){
        accountHolderNAme = name;
        acountNumber = accno;
        Balacne = balacne;

    }
    void depodit(double amount){
        Balacne += amount ;


    }

    void withdraw(double amount) {
        if (Balacne - amount >=0) {
             Balacne -= amount ;

        }
        else{
            System.out.println("Insufficient balacne.");
        }

    }

    void displayAccountInfo(){
        System.out.println("Holder:" +accountHolderNAme);
        System.out.println("Account NO:"+acountNumber);
        System.out.println("Current Balance :" +Balacne );

    }

    public static  void main(String[]args) {

        BankAccount b = new BankAccount();
        b.setAccountDetails("Praksh kumar", "49476964", 5546);
        b.depodit(786);
        b.withdraw(457);
        b.displayAccountInfo();


    }



}
