Random-Guess-Game
=================

import java.util.Scanner;


public class Randomif {
	public static void main(String [] args){
		Scanner myScan = new Scanner(System.in);
		int correctAnswer = (int)Math.ceil(Math.random()*10);
		
		int numberOfGuesses = 3;
		int userGuess = 0;
		
	System.out.println("You have Guesses set from 1 to 10");
		
		while(numberOfGuesses > 0) {
			System.out.println("Enter Guess");
			
			userGuess = myScan.nextInt();
			 
			if(userGuess == correctAnswer){
				System.out.println("You Win!!!");
			}else if (numberOfGuesses == 1){
				System.out.println("You Lose!:( The correct answer is" + correctAnswer);
			}else {
				System.out.println("Wrong Anwer! Try again!");
			}
			
			numberOfGuesses--;
		}
	}
}




Number guessing 1-10
