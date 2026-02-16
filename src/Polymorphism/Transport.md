public class Transport {

    void travelMode(String bus){
        System.out.println("Travelling by bus ");
    }

    void travelMode(String train , String fligth){
        System.out.println("Travelling by trian");
        System.out.println("Travelling by flight");
    }

    public static void main(String[]args){

        Transport t = new Transport();
        t.travelMode(",");
        t.travelMode("," , ",");
    }

}
