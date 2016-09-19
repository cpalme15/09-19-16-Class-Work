# 09-19-16-Class-Work
/* Programmer: Collin Palmer
 * Date: 09/19/16
 * COSC 111- String Methods
 */
import java.util.*;
public class Strings
{

	public static void main(String[] args)
	{

		 Scanner k = new Scanner(System.in);
	
		String address=null,streetname=null;
		String word1= new String("miSSISSIppI");
		String word2= new String("");
		
		
		
		address=new String();
		char firlttr=' ';
		firlttr=word1.toUpperCase().charAt(0);
		word2=firlttr+word1.substring(1).toLowerCase();
		System.out.println("The new word is "+ word2);
		System.out.println(word1.equals(word2));
		System.out.println(word1.equalsIgnoreCase(word2));
		int loadr= 0, streetnum=0;
		
		System.out.print("What is your street address?");//prompt
		
		address= k.nextLine();//input
		
		System.out.println("Your address is "+ address);//echo
		address= address.toUpperCase().trim();
		System.out.println("Your address capitalized is "+ address);
		
		loadr=address.length();
		System.out.println("The length is "+loadr);
		
		streetname=address.substring(address.indexOf(' ')+1 );
		System.out.println("You live on street:"+ streetname);
		
		streetnum=Integer.parseInt(address.substring(0,address.indexOf(' ')));
		System.out.println("The number is:"+ streetnum+".");
		
		}

}
