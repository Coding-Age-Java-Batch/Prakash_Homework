class course {
String courserName = "Java programing";

    void Showcourse (){
        System.out.println(" Course Name :" + courserName);
    }

}

class EnrolledStudent extends course{
String Name = "Arti";
int roll = 101;


    @Override
        void  Showcourse (){
            System.out.println(" Student Name :" + Name);
            System.out.println("Roll no :" + roll);
        }
    public static void main(String[]args){


            EnrolledStudent e = new EnrolledStudent();

            e.Showcourse();
    }

}
