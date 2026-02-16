class Account {
double Balance = 1000;

    void showBalance(){

        System.out.println("Balance"+ Balance);
    }
}

class SavingAccount extends account{

    double Interestrate =  5;

    @Override
    void showBalance() {
        double updateBlance = Balance+ (Balance * Interestrate /100);
        System.out.println("Balance with interest:"+ updateBlance);
    }

    public static void main(String[]args){

        SavingAccount sa = new SavingAccount();
        sa.showBalance();
    }
}

