labbar
======
import javax.swing. *;

//Vår klass heter Laboneadham. Public säger att vi kan använda
//vår klass genom hela programmet. 
public class Laboneadham {
    public static void main (String [] arg) {
      while (true) {
          
        int[] months = new int[12];
        months[0] = 31; //Alla månader + dagar
        months[1] = 28; 
        months[2] = 31;
        months[3] = 30;
        months[4] = 31;
        months[5] = 30;       
        months[6] = 31;
        months[7] = 31;
        months[8] = 30;
        months[9] = 31;
        months[10] = 30;
        months[11] = 31;
        
        String s = JOptionPane.showInputDialog ("Skriv in ett årtal") ;
        int year = Integer.parseInt(s); 
        //Integer.parseInt omvandlar (s) till ett numeriskt värde,
        //och tilldelar detta värdet till strängen String. 
           
        //Om året delat med 4 inte lämnar någon rest OCH året
        //delat med 100 lämnar rest, då är det skottår.
        //Även år som delas med 400 och inte ger rest är skottår. 
        if (year % 4 == 0 && year % 100 !=0) {
            JOptionPane.showMessageDialog(null, year + " är ett skottår");
        } else if (year % 400 == 0) {
            JOptionPane.showMessageDialog (null, year + " är ett skottår");
        } else {
            JOptionPane.showMessageDialog (null, year + " är inte ett skottår");
        }
    }

    }
}




















import javax.swing. *;

public class Lab11adham {
    public static void main (String[] arg) {
    
        int[] months = new int[12];
        months[0] = 31; //Alla månader + dagar
        months[1] = 28; 
        months[2] = 31;
        months[3] = 30;
        months[4] = 31;
        months[5] = 30;       
        months[6] = 31;
        months[7] = 31;
        months[8] = 30;
        months[9] = 31;
        months[10] = 30;
        months[11] = 31;
        
        String s = JOptionPane.showInputDialog ("Skriv ett datum: yyyy-mm-dd") ;
        //int datum = Integer.parseInt(s); 
        
        String datum =("yyyy-mm-dd");
        String datum1 = datum.substring(0,4);
        String datum2 = datum.substring(5,7);
        String datum3 = datum.substring(8,10); 
       
        if (datum.length() == 10) {
            JOptionPane.showMessageDialog (null, "Antal dagar är");
        } else 
            JOptionPane.showMessageDialog (null, "Inte ett datum");
        
        
                 
                
