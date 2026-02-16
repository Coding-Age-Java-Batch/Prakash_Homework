class school {

     String schoolName = "Green Valley";

     void showschool(){

         System.out.println("School: "+ schoolName);
     }
}

class Teacher extends school{

     String teacherName = "Mr . Sharma ";

      void showTeacherDetails(){

          System.out.println("Teacher: "+ teacherName);
      }

      public static void main(String[]args){

          Teacher t = new Teacher();

          t.showschool();
          t.showTeacherDetails();
      }
}