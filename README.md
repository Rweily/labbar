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
        
        
                 
                 
                 
                 
                 
                 
                 
                 
                 
                 
                
% Uppgift1
 r = 4
 A = pi*r^2

%% 
% Uppgift2
 x = 0:0.1:4*pi ;
 f = sin(x)+0.3*sin(5*x) ;
% plot ritar upp grafen för alla angivna x värden.
 plot (x,f)

%%  
% EXEMPEL 3
% Rita graferna av f(x) = sin(x) och g(x) = sin(4x) f¨or 0 ? x ? 2?. 
% S¨att rubrik och text pa axlarna

x = linspace(0 ,2*pi); % linspace gör så att vi får 100 punkter
                       % mellan 0 till 2pi, finare graf.
f = sin(x);
g = sin(4*x);
plot (x,f,'green',x,g,'red') % f(x) görs gröön och g(x) görs röd.
xlabel('x') % namnger x och y lederna.
ylabel('y')
title('sin(x) och sin(4x)') % Anger titeln på grafen.
grid on

%% 
% Uppgift3
s = 0;
for i = 1:5       % Talen 1 till 5.
    s = s+i^2;    % Tar summan av 1^2 plus 2^2 ända till 5^2. 
end 
disp('summan är') % "display" -> visar texten "summan är"
disp(s)           % följt av s som är summan. 

%% 
% Uppgift4
% Skriven i två separata filer. "kladdkaka" oh "nollstallen".

%% 
% Uppgift 5
%% y = linspace(x1,x2, N) osv. 
% Default är 100 punkter.

%% 
% Grafritning
% 




% Nollställen

x = linspace(-2, 2);
y=kladdkaka(x);
plot(x,y)
grid on
%% Nollställe 1

x=fzero(@kladdkaka,1) 
disp('Nollställe ett är')
disp(x)

%% Nollställe 2

x=fzero(@kladdkaka,-1)
disp('Nollställe två är')
disp (x)




% Funktion namn och funktion. 
function y=kladdkaka(x)
y=x.^2-cos(x);


                
