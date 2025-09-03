# Rock--Paper--Scissors-Game
 a game built using  loops , input and outputs in a efficient manner..
import java.util.*;
public class RockPaperScissors {
public static void main(String[] args){
Scanner obj=new Scanner(System.in);
Random random=new Random();
String[]choices={"rock","paper","scissors"};
String playerchoice;
String computerchoice;
String playagain="yes";
boolean keeprunning=true;
while(keeprunning){
System.out.println("Enter Your Choice::(rock,paper,scissors)");
playerchoice=obj.nextLine().toLowerCase();
if (!playerchoice.equals("rock")&&
    !playerchoice.equals("scissors")&&
    !playerchoice.equals("paper")) {
    System.out.println("invalid choice".toUpperCase());
}
computerchoice=choices[random.nextInt(3)];
System.out.println("Computer choice::"+computerchoice);
if (playerchoice.equals(computerchoice)) {
    System.out.println("its a tie".toLowerCase());
}else if (playerchoice.equals("rock")&&computerchoice.equals("scissors")){
    System.out.println("you win!!!".toLowerCase());
}else if
         (playerchoice.equals("scissors")&&computerchoice.equals("paper")){
            System.out.println("you win!!!".toLowerCase());
}else if
         (playerchoice.equals("paper")&&computerchoice.equals("rock")){
         System.out.println("you win!!!".toLowerCase());
}else{
System.out.println("you lose :(".toLowerCase());
}
System.out.println("playagain:yes/no");
playerchoice=obj.nextLine();
if(!playagain.equals("yes")){
    keeprunning=false;
}

}}}


    

