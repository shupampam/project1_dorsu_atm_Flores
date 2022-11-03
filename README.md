# project1_dorsu_atm_Flores
import java.util.Scanner;
public class Main {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("            Welcome to DOrSU banking system.");
		System.out.println('\n');
 System.out.println("                        ****");
 System.out.println('\n');
 System.out.println("        To start select from the following transaction:");
 System.out.println('\n'); 
 System.out.println("                      1- View Balance");
 System.out.println("                      2- Withdraw");
 System.out.println("                      3- Deposit");
 System.out.println("                      4- Exit");
System.out.println("      --------------------------------------------------");
System.out.println("      --------------------------------------------------");System.out.println('\n');
int balance = 10000;
int maintain=100;
 System.out.print("Enter transaction NO.: ");
 int ATM = sc.nextInt();
 
 switch (ATM){
   case 1:
    System.out.println("Your balance is: "+ balance);
    break;
    
   case 2:
    System.out.println("Please enter the amount");
     int amount = sc.nextInt();
     int remain = balance - amount;
     
     
     if(remain < maintain){System.out.println("make sure to check if the current balance will not be below 100.00");}
     else{ System.out.println("The transaction is done completely ");
     System.out.println("please collect your money in the Despenser");
     System.out.println("Total balance is : " + remain);
      }
      
      
     break;
     
     case 3:
     System.out.print("deposit: ");
	          int deposit = sc.nextInt();
	          int d = deposit + balance;
	          System.out.println("total deposit: "+ d );
	        break;
	         
	         case 4:
	          System.out.println("thank you for using the atm");
	        break;
	         
  
  }
	}
}
