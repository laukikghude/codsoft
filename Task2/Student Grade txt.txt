import java.util.*;

class Studentgrade
{
    public static void main(String[] args) {

        Scanner sc=new Scanner(System.in);

        System.out.println("Enter the Student Name:");
        String name;
        name=sc.nextLine();

        System.out.println("Enter the Marks of Subject 1:");
        double marks1;
        marks1=sc.nextDouble();

        System.out.println("Enter the Marks of Subject 2:");
        double marks2;
        marks2=sc.nextDouble();

        System.out.println("Enter the marks of Subject 3:");
        double marks3;
        marks3=sc.nextDouble();

        System.out.println("Enter the marks of Subject 4:");
        double marks4;
        marks4=sc.nextDouble();

        System.out.println("Enter the Marks of Subject 5:");
        double marks5;
        marks5=sc.nextDouble();

        double totalMarks=marks1+marks2+marks3+marks4+marks5;
        double percentage=totalMarks/5;

        if(percentage>90 && percentage<100)
        {
            System.out.println("\n \nHey "+name);
            System.out.println("Your Result:)");
            System.out.println("Total Marks:"+totalMarks);
            System.out.println("Total Percentage:"+percentage+"%");
            System.out.println("Grade: A+");
        }

       else if(percentage>=85 && percentage<=90){
        System.out.println("Hey "+name);
        System.out.println("Your Result:)");
        System.out.println("Total Marks:"+totalMarks);
        System.out.println("Total Percentage:"+percentage+"%");
        System.out.println("Grade: A");

       }

       else if(percentage>=80 && percentage<85){
        System.out.println("Hey "+name);
        System.out.println("Your Result:)");
        System.out.println("Total Marks:"+totalMarks);
        System.out.println("Total Percentage:"+percentage+"%");
        System.out.println("Grade: B+");
       }

       else if(percentage>=70 && percentage<80){
        System.out.println("Hey "+name);
        System.out.println("Your Result:)");
        System.out.println("Total Marks:"+totalMarks);
        System.out.println("Total Percentage:"+percentage+"%");
        System.out.println("Grade: B");
       }

       else if(percentage>=60 && percentage<70){
        System.out.println("Hey "+name);
        System.out.println("Your Result:)");
        System.out.println("Total Marks:"+totalMarks);
        System.out.println("Total Percentage:"+percentage+"%");
        System.out.println("Grade: C");
       }

       else if(percentage>=50 && percentage<60){
        System.out.println("Hey "+name);
        System.out.println("Your Result:)");
        System.out.println("Total Marks:"+totalMarks);
        System.out.println("Total Percentage:"+percentage+"%");
        System.out.println("Grade: D");
       }

       else if(percentage>=40 && percentage<50){
        System.out.println("Hey "+name);
        System.out.println("Your Result:)");
        System.out.println("Total Marks:"+totalMarks);
        System.out.println("Total Percentage:"+percentage+"%");
        System.out.println("Grade : E");
       }

       else if(percentage>=35 && percentage<40){
        System.out.println("Hey dhfghs"+name);
        System.out.println("Your Result:)");
        System.out.println("Total Marks:"+totalMarks);
        System.out.println("Total Percentage:"+percentage+"%");
        System.out.println("Grade: P(Pass)");
       }

       else if(percentage>100 && percentage<0)
       {
        System.out.println("Enter Valid Marks:()");
       }

       else{
        System.out.println("Entered Something Wrong");
       }
       sc.close();

       System.out.println("Thankyou:) For using Student Grade Calculator");
    
    }
}