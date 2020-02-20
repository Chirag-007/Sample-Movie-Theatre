import java.io.*;
import java.util.*;
public class Ticket_counter
{ 
    public static void main()
    {
        Scanner ch=new Scanner(System.in);
        System.out.println("                       MAIN MENU ");
        System.out.println("                       Welcome to Royal Cinemas ");
        System.out.println("                       Please choose a movie of your choice ");
        System.out.println(" Now Playing:  ");
        System.out.println(" 1. Kedarnath   ");
        System.out.println(" 2. 2.0  ");
        System.out.println(" 3. Aquaman ");
        System.out.println(" 4. Spiderman:Into the spiderverse ");
        System.out.println(" Enter your choice:   ");
        int choice=ch.nextInt();
        switch(choice)
        {
            case 1:
        {
         System.out.println("        You have chosen to watch Kedarnath ");
         System.out.println("Kedarnath is a potent combination of love and religion, of passion and spirituality");
         System.out.println("It is set on a 14-kilometer pilgrimage from Gauri Kund to Kedarnath - the 2000-year-old holy temple of Lord Shiva."); 
         System.out.println("Mansoor, a reserved and reticent porter, helps pilgrims make an arduous journey to the temple town."); 
         System.out.println("His world turns around when he meets the beautiful and rebellious Mukku, who draws him into a whirlwind of intense love."); 
         System.out.println("Destiny has plans for lovers amidst the uncertainties of life, nature, and broken hearts.");
         System.out.println("This movie stars Sushant Singh Rajput and debutant Sara Ali Khan in lead roles");
         System.out.println("It is a wonderful love-drama combination filled with amazing songs and is a must watch for Bollywood fans");
         System.out.println("Our rating for this movie is a complete 10");
         System.out.println("The show times are as follows");
         System.out.println("1. 2:00 p.m");
         System.out.println("2. 9:00 p.m");
         System.out.println("Which show do you want to watch?");
         System.out.println("Press 1 for 2:00 pm show and any other number for 9:00 pm show");
         int n=ch.nextInt();
         if(n==1)
         {
             int show=2;
               System.out.println("You have chosen 2:00 p.m show");
         
         }
         else
         {
             int show=9;
             System.out.println("You have chosen 9:00 p.m show");
         }
         
         System.out.println("Please choose the number of tickets, Maximum number of tickets = 6");
         System.out.println("Cost of 1 ticket is Rs.200");
         int t=ch.nextInt();
         int ticket=t;
         int bill=ticket*200;
         System.out.println("Do you want a food cart; press Y if so");
         String d=ch.next();
         String s="Y";
         
         if(d.compareTo(s)==0)
         {
             System.out.println("You have chosen to opt for a food court");
             System.out.println("The options are as follows");
             System.out.println("1. Popcorn");
             System.out.println("2. Nachos");
             System.out.println("Note you can only order one of the above");
             System.out.println("Please enter your choice using the numbers alloted to the food items");
             int f=ch.nextInt();
             if(f==1)
             {
                 System.out.println("You have chosen to buy Popcorn");
                 System.out.println("Cost is Rs.100");
                 System.out.println("Enter the number of popcorn buckets you want");
                 int f1=ch.nextInt();
                 int money=100*f1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String f2=ch.next();
                 String s1="Y";
                 if(f2.compareTo(s1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int f3=ch.nextInt();
                    int money2=50*f3;
                    int foodbill=money+money2;
                    int total=foodbill+bill;
                    System.out.println("You have chosen to watch Kedarnath");
                    System.out.println("Number of tickets is "+ticket);
                    System.out.println("Your ticket bill is "+bill);
                    System.out.println("Your food bill is "+foodbill);
                    System.out.println("Your total bill is "+total);
                    System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                    System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                 int foodbill=money;
                 int total=foodbill+bill;
                 System.out.println("You have chosen to watch Kedarnath ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 
             }
                 else if(f==2)
             {
                 System.out.println("You have chosen to buy Nachos");
                 System.out.println("Cost is Rs.90");
                 System.out.println("Enter the number of nachos you want");
                 int n1=ch.nextInt();
                 int mon=90*n1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String n2=ch.next();
                 String S1="Y";
                 if(n2.compareTo(S1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int n3=ch.nextInt();
                    int mon2=50*n3;
                    int foodbill=mon+mon2;
                    int total=foodbill+bill;
                 System.out.println("You have chosen to watch Kedarnath ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                     int foodbill=mon;
                     int total=foodbill+bill;
                 System.out.println("You have chosen to watch Kedarnath ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }

             }
         }
         else 
         {
                int total=bill;
                System.out.println("You have chosen to watch Kedarnath ");
                System.out.println("Number of tickets is "+ticket);
                System.out.println("Your ticket bill is "+bill);
        
                System.out.println("Your total bill is "+total);
         }
        } break;                                                  //End of case 1
        case 2:
        {
         System.out.println("        You have chosen to watch 2.0 ");
         System.out.println("2.0 is a 2018 Indian Tamil-language science fiction action film[3][8] written and directed by S. Shankar.");
         System.out.println("Produced by Subaskaran under the banner of Lyca Productions, the film is a standalone sequel to Enthiran (2010).");
         System.out.println("The film follows the conflict between Chitti, the once dismantled humanoid robot, and Pakshi Rajan, an ornithologist who seeks vengeance on cell phone users to prevent avian population decline."); 
         System.out.println("The soundtrack is composed by A. R. Rahman, with lyrics written by Madhan Karky and Na. Muthukumar.");
         System.out.println("This movie stars Akshay Kumar and Rajnikanth in lead roles");
         System.out.println("Our rating for this movie is 7.5 out of 10");
         System.out.println("The show timing is 7:00 p.m");
         System.out.println("Please choose the number of tickets, Maximum number of tickets = 6");
         System.out.println("Cost of 1 ticket is Rs.180");
         int t=ch.nextInt();
         int ticket=t;
         int bill=ticket*180;
         System.out.println("Do you want a food cart; press Y if so");
         String d=ch.next();
         String s="Y";
         
         if(d.compareTo(s)==0)
         {
             System.out.println("You have chosen to opt for a food court");
             System.out.println("The options are as follows");
             System.out.println("1. Popcorn");
             System.out.println("2. Nachos");
             System.out.println("Note you can only order one of the above");
             System.out.println("Please enter your choice using the numbers alloted to the food items");
             int f=ch.nextInt();
             if(f==1)
             {
                 System.out.println("You have chosen to buy Popcorn");
                 System.out.println("Cost is Rs.100");
                 System.out.println("Enter the number of popcorn buckets you want");
                 int f1=ch.nextInt();
                 int money=100*f1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String f2=ch.next();
                 String s1="Y";
                 if(f2.compareTo(s1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int f3=ch.nextInt();
                    int money2=50*f3;
                    int foodbill=money+money2;
                    int total=foodbill+bill;
                    System.out.println("You have chosen to watch 2.0");
                    System.out.println("Number of tickets is "+ticket);
                    System.out.println("Your ticket bill is "+bill);
                    System.out.println("Your food bill is "+foodbill);
                    System.out.println("Your total bill is "+total);
                    System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                    System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                 int foodbill=money;
                 int total=foodbill+bill;
                 System.out.println("You have chosen to watch 2.0 ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 
             }
                 else if(f==2)
             {
                 System.out.println("You have chosen to buy Nachos");
                 System.out.println("Cost is Rs.90");
                 System.out.println("Enter the number of nachos you want");
                 int n1=ch.nextInt();
                 int mon=90*n1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String n2=ch.next();
                 String S1="Y";
                 if(n2.compareTo(S1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int n3=ch.nextInt();
                    int mon2=50*n3;
                    int foodbill=mon+mon2;
                    int total=foodbill+bill;
                 System.out.println("You have chosen to watch 2.0 ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                     int foodbill=mon;
                     int total=foodbill+bill;
                 System.out.println("You have chosen to watch 2.0");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }

             }
         }
         else 
         {
                int total=bill;
                System.out.println("You have chosen to watch 2.0 ");
                System.out.println("Number of tickets is "+ticket);
                System.out.println("Your ticket bill is "+bill);
        
                System.out.println("Your total bill is "+total);
         }
        } break;                         //End of case 2
        case 3:
        {
         System.out.println("        You have chosen to watch Aquaman ");
         System.out.println("Aquaman is a 2018 American superhero film based on the DC Comics character of the same name, distributed by Warner Bros. Pictures.");
         System.out.println("It is the sixth installment in the DC Extended Universe (DCEU). "); 
         System.out.println(" In Aquaman, Arthur Curry, the heir to the underwater kingdom of Atlantis, must step forward to lead his people against his half-brother Orm "); 
         System.out.println("Orm seeks to unite the seven underwater kingdoms against the surface world."); 
         System.out.println("The movie stars Jason Momoa and Willem Defoe in lead roles. ");
         System.out.println("We give this movie 8 out of 10 ");
         System.out.println("The show timing is 8:30 a.m");
         System.out.println("Cost of 1 ticket is Rs.160");
         int t=ch.nextInt();
         int ticket=t;
         int bill=ticket*160;
         System.out.println("Do you want a food cart; press Y if so");
         String d=ch.next();
         String s="Y";
         
         if(d.compareTo(s)==0)
         {
             System.out.println("You have chosen to opt for a food court");
             System.out.println("The options are as follows");
             System.out.println("1. Popcorn");
             System.out.println("2. Nachos");
             System.out.println("Note you can only order one of the above");
             System.out.println("Please enter your choice using the numbers alloted to the food items");
             int f=ch.nextInt();
             if(f==1)
             {
                 System.out.println("You have chosen to buy Popcorn");
                 System.out.println("Cost is Rs.100");
                 System.out.println("Enter the number of popcorn buckets you want");
                 int f1=ch.nextInt();
                 int money=100*f1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String f2=ch.next();
                 String s1="Y";
                 if(f2.compareTo(s1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int f3=ch.nextInt();
                    int money2=50*f3;
                    int foodbill=money+money2;
                    int total=foodbill+bill;
                    System.out.println("You have chosen to watch Aquaman");
                    System.out.println("Number of tickets is "+ticket);
                    System.out.println("Your ticket bill is "+bill);
                    System.out.println("Your food bill is "+foodbill);
                    System.out.println("Your total bill is "+total);
                    System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                    System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                 int foodbill=money;
                 int total=foodbill+bill;
                 System.out.println("You have chosen to watch Aquaman ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 
             }
                 else if(f==2)
             {
                 System.out.println("You have chosen to buy Nachos");
                 System.out.println("Cost is Rs.90");
                 System.out.println("Enter the number of nachos you want");
                 int n1=ch.nextInt();
                 int mon=90*n1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String n2=ch.next();
                 String S1="Y";
                 if(n2.compareTo(S1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int n3=ch.nextInt();
                    int mon2=50*n3;
                    int foodbill=mon+mon2;
                    int total=foodbill+bill;
                 System.out.println("You have chosen to watch Aquaman ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                     int foodbill=mon;
                     int total=foodbill+bill;
                 System.out.println("You have chosen to watch Kedarnath ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }

             }
         }
         else 
         {
                int total=bill;
                System.out.println("You have chosen to watch Aquaman ");
                System.out.println("Number of tickets is "+ticket);
                System.out.println("Your ticket bill is "+bill);
        
                System.out.println("Your total bill is "+total);
         }
        } break;                                                         //End of case 3
        case 4:
        {
         System.out.println("        You have chosen to watch Spiderman:Into The Spiderverse ");
         System.out.println("  Bitten by a radioactive spider in the subway, Brooklyn teenager Miles Morales suddenly develops mysterious powers that transform him into the one and only Spider-Man. ");
         System.out.println("  When he meets Peter Parker, he soon realizes that there are many others who share his special, high-flying talents. ");
         System.out.println("  Miles must now use his newfound skills to battle the evil Kingpin, a hulking madman who can open portals to other universes and pull different versions of Spider-Man into our world.");
          System.out.println("This movie is voiced by actors like Jake Johnson,Hailee Steinfield and Shameik Moore");
          System.out.println("This movie is a marvel animation and therfore the first of its kind");
          System.out.println("Our rating for this movie is a 9 out of 10");
          System.out.println("The show times are as follows");
         System.out.println("1. 11:00 a.m");
         System.out.println("2. 7:00 p.m");
         System.out.println("Which show do you want to watch?");
         System.out.println("Press 1 for 7:00 pm show and any other number for 11:00 am show");
         int n=ch.nextInt();
         if(n==1)
         {
             int show=7;
               System.out.println("You have chosen 7:00 p.m show");
         
         }
         else
         {
             int show=11;
             System.out.println("You have chosen 11:00 a.m show");
         }
         
         System.out.println("Please choose the number of tickets, Maximum number of tickets = 6");
         System.out.println("Cost of 1 ticket is Rs.190");
         int t=ch.nextInt();
         int ticket=t;
         int bill=ticket*190;
         System.out.println("Do you want a food cart; press Y if so");
         String d=ch.next();
         String s="Y";
         
         if(d.compareTo(s)==0)
         {
             System.out.println("You have chosen to opt for a food court");
             System.out.println("The options are as follows");
             System.out.println("1. Popcorn");
             System.out.println("2. Nachos");
             System.out.println("Note you can only order one of the above");
             System.out.println("Please enter your choice using the numbers alloted to the food items");
             int f=ch.nextInt();
             if(f==1)
             {
                 System.out.println("You have chosen to buy Popcorn");
                 System.out.println("Cost is Rs.100");
                 System.out.println("Enter the number of popcorn buckets you want");
                 int f1=ch.nextInt();
                 int money=100*f1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String f2=ch.next();
                 String s1="Y";
                 if(f2.compareTo(s1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int f3=ch.nextInt();
                    int money2=50*f3;
                    int foodbill=money+money2;
                    int total=foodbill+bill;
                    System.out.println("You have chosen to watch Spiderman");
                    System.out.println("Number of tickets is "+ticket);
                    System.out.println("Your ticket bill is "+bill);
                    System.out.println("Your food bill is "+foodbill);
                    System.out.println("Your total bill is "+total);
                    System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                    System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                 int foodbill=money;
                 int total=foodbill+bill;
                 System.out.println("You have chosen to watch Spiderman ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 
             }
                 else if(f==2)
             {
                 System.out.println("You have chosen to buy Nachos");
                 System.out.println("Cost is Rs.90");
                 System.out.println("Enter the number of nachos you want");
                 int n1=ch.nextInt();
                 int mon=90*n1;
                 System.out.println("Do you want any drinks with that?");
                 System.out.println("If so,press Y");
                 String n2=ch.next();
                 String S1="Y";
                 if(n2.compareTo(S1)==0)
                 {
                    System.out.println("You have chosen to buy drinks");
                    System.out.println("Cost is Rs.50");
                    System.out.println("Enter the number of drinks you want");
                    int n3=ch.nextInt();
                    int mon2=50*n3;
                    int foodbill=mon+mon2;
                    int total=foodbill+bill;
                 System.out.println("You have chosen to watch Spiderman ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }
                 else
                 {
                     int foodbill=mon;
                     int total=foodbill+bill;
                 System.out.println("You have chosen to watch Spiderman ");
                 System.out.println("Number of tickets is "+ticket);
                 System.out.println("Your ticket bill is "+bill);
                 System.out.println("Your food bill is "+foodbill);
                 System.out.println("Your total bill is "+total);
                 System.out.println("Patrons are requested to arrive 30 minutes before showtimes");
                 System.out.println("                              *** Thank you for booking with us ***");
                 }

             }
         }
         else 
         {
                int total=bill;
                System.out.println("You have chosen to watch Spiderman ");
                System.out.println("Number of tickets is "+ticket);
                System.out.println("Your ticket bill is "+bill);
        
                System.out.println("Your total bill is "+total);
         }
        } //End of case 4
        default:
        {
            System.out.println("                     ******** WRONG CHOICE ******* ");
            
            
        }            
    }
  }
