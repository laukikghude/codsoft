import java.util.*;

class Operations 
{

    Scanner sc=new Scanner(System.in);
    double amount;
    
    void amounts(){
        System.out.println("Enter the Amount in Account: ");
         amount=sc.nextDouble();
    }

    void deposit(){
        System.out.println("Enter the Amount you want to Deposit:");
                double deposit =sc.nextDouble();
                amount=amount+deposit;
                System.out.println("Your New Balance is :"+amount);
     }

     void withdraw()
     {
        System.out.println("Enter the Amount you want to Withdraw:");
                    double withdraw=sc.nextDouble();

                    if(amount>withdraw)
                    {
                        amount=amount-withdraw;
                        System.out.println("Your New Balance is :"+amount);
                    }
                       
                    
                    else if(amount<withdraw)
                    {
                        System.out.println( "Sorry! You don't have enough Balance");
                        System.out.println("Available Balance: "+amount);
                    }
    }

    void checkBalance()
    {
        System.out.println("Balance:"+amount);
    }

   

    
}
class ATM extends Operations{
    public static void main(String[] args) {
       Scanner s=new Scanner(System.in);
       ATM atm= new ATM();
        atm.amounts();
        System.out.println("1.Deposit");
        System.out.println("2.Withdrawal");
        System.out.println("3.Check Balance");
        int choice=s.nextInt();

       

        switch(choice){
            case 1: atm.deposit();break;

            case 2: atm.withdraw();break;
                    
                      
            case 3: atm.checkBalance();break;
            
            
            default:
            System.out.println("Entered Something Wrong :( )");break;


        }
        s.close();

    }
}