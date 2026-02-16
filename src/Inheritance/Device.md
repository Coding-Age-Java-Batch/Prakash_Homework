class Device {

    String deviceName = "Samsung Galaxy";

    void showInfo(){
        System.out.println("Device Name :" + deviceName);
    }
}

class Mobile extends  Device{

    String os = "Android";



    void showInfo(){

        System.out.println("Operating System :"+ os);
    }

    public static void main(String[]args){

        Mobile m = new Mobile();

        m.showInfo();
    }
}
