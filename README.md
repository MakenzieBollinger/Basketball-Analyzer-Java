# Basketball-Analyzer-Java

import java.util.*;
public class BasketballAnalyzer{
	public static void main(String[] args){
		
		String school;
		int uncWins, n1, n2, total;
		uncWins = 5;
		Scanner keyboard = new Scanner(System.in);
		
		System.out.println("Welcome to the basketball analyzer! Which school do you believe is the greatest at basketball?");
		school = keyboard.nextLine();
		
			if(school.equalsIgnoreCase("unc")){
				System.out.println("How many championships does UNC have?");
				n1 = keyboard.nextInt();
				
				if (n1 < uncWins)
					System.out.println("You are a fake fan!");
				else if (n1 == uncWins)
					System.out.println("Congrats! You are a true fan!");
				else
					System.out.println("Maybe one day...");
			}
		
			else if(school.equalsIgnoreCase("duke")){
				System.out.println("Get out!!");
			}
			
			else {
				System.out.println("How many NCAA Championships do they have?");
				n2 = keyboard.nextInt();
				
				if (n2 < uncWins){
				total = uncWins - n2;
					System.out.println("UNC has " + total + " more championship wins than that!");
				}
				else
					System.out.println("They are okay.");
			}	
			
			System.out.println("Thank you for usng the Basktball Analyzer. Go Heels!");
}
}
