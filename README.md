package m7md.java1;

import java.util.Scanner ;

public class M7MDJava1 {

    public static void main(String[] args) {
Scanner n=new Scanner(System.in);
System.out.print("  Enter the number for which you would like to change the unit of measurement = "); 
Double num1=n.nextDouble() ;
 System.out.println("==================================================================================");
   System.out.println("""
                     
    1- Convert from CM to Inche
    2- Convert from Inche to CM
    3- Convert from M to Feet
    4- Convert from Feet to M
    5- Convert from Dunm to Hiktar
    6- Convert from Hiktar to Dunm
    7- Convert from Cels to Fenh
    8- Convert from Fenh to Cels
            """
    );
    System.out.println("==================================================================================");
 
            System.out.print("Select the number corresponding to the transaction you wish to perform = ");

    int num2=n.nextInt() ;  
    
        System.out.println("==================================================================================");
        if ((num1>0) && (num2<=6) && (num2>=1)) {
      
        switch (num2){
        case 1 : System.out.println("Converted from CM to Inche = " + (num1*0.3937));
        break ;
        case 2 :System.out.println("Converted from Inche to CM = " + (num1*2.54));
        break ;
        case 3: System.out.println("Converted from M to Feet = " + (num1*3.28084));
        break ;
        case 4:System.out.println("Converted from Feet to M =  " + (num1/3.28084));
        break;
        case 5:System.out.println("Converted from Dunm to Hiktar = " + (num1*0.1));
        break ;
        case 6:System.out.println("Converted from Hiktar to Dunm = " + (num1/0.1));
        break;
        default :
            System.out.println("error");
        }
        }
        else if ((num2<=8) && (num2>=7)  && ((num1>=-1000)||(num1<=-1000) )){
        switch (num2){
         case 7:System.out.println("Converted from Cels to Fenh = " + ((num1*1.8) + 32));
        break ;
        case 8:System.out.println("Converted from Fenh to Cels = " + ((num1-32)/1.8));
        break ;   
        
        
        } 
}
        else  {
            
            if ((num1<=0)&& ((num2<=6 )&&(num2>=1)))
                System.out.println("Choose a number greater than zero");
            else 
            System.out.println("Choose a number from 1 to 8. ");
        }      
     System.out.println("==================================================================================");
     System.out.println("                                   Good bey                                       ");
    
        
        
        
    
    }
}
