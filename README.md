package pontoon;

import java.util.Scanner;

public class pontoon2 {
	
	
	public static void main(String[] args)
	{
		Scanner keyboard = new Scanner(System.in);
		String choice;
		int card1;
		int card2;
		int new_card;
		int total;
		
		card1 = 1 + (int)(Math.random() * 9);
		System.out.println("first card: " + card1);
		
		card2 = 1 + (int)(Math.random() * 9);
		System.out.println("second card: " + card2);
		
	total = card1 + card2;
	System.out.println("your current score is: " + card2);
	System.out.println("would you like to draw another card? (Y/N): ");
	choice = keyboard.next();
	System.out.println("You chose: " + choice);
	
	String anotherString = null;
	while (choice.equalsIgnoreCase(anotherString))
		{
		new_card = 1 + (int)(Math.random() * 9);
		System.out.println("new card: " + new_card);
		total = total + new_card;
		System.out.println("your current score is: " + total);
		System.out.println("draw another card? (Y/N): ");
		choice = keyboard.next();
		System.out.println("You chose: " + choice);
		
		}
	if (choice.equalsIgnoreCase(anotherString))
	{
		if (total > 18 && total < 22)
		{
			System.out.println("House has 18.");
			System.out.println("Player has " + total + "you win");
			keyboard.close();
		}
		if (total > 21 || total < 18)
{
	System.out.println("House has 18.");
	System.out.println("Player has " + total + "you lose");
	keyboard.close();
}
       if (total == 18)
{
	System.out.println("House has 18");
	System.out.println("Player has" + total + "Draw");
	keyboard.close();
}
}
}
		}
	
