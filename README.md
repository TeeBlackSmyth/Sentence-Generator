# Sentence-Generator
You give the code a series of words and it displays a random sentence. 
import java.util.Scanner;
//imports scanner class 

public class MyLearningProject 
{
	
	public static void main(String args[]) 
	{
		Scanner sc = new Scanner(System.in);
		
		//Creating Arrays for words to go into 
		
		String verb[] = {};
		
		String noun[] = {};
		
		String adj[] = {};
		
		String adv[] = {};
		
		//creating a prompt that asks for a word
		while(true)
		{
		
			System.out.println("Tell me a Word");
		
			String word = sc.nextLine();
		
			System.out.println("what kind of word is this?(Noun, Verb, Adjective, Adverb)");
		
			String definition = sc.nextLine();

		
				if (definition == "verb") 
				{
					word = verb[-1+1];
				}
				if (definition == "noun")
				{
					word = noun[-1+1];
				}
				if (definition == "adjective") 
				{
					word = adj[-1+1];
				}
				if (definition == "adverb")
				{
					word = adv[-1+1];
				}
				
			System.out.println("would you like me to create a sentence with your word? (y/n)");
			
			String res = sc.nextLine();
		
			 if (res == "y")
			 {
				 System.out.println(noun[1] + verb[1] + noun[1]);
			 }
			 if (res == "n") 
			 {
				 System.out.println("sorry.");
			 }
			 
		}

	}
		
}
