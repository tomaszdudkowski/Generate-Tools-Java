/**
 * Package name: pl.dudkowski.devTools
 * Date: 29.03.2017
 * Time: 20:40:19
 * Author: tomasz
 */
package pl.dudkowski.devTools;

import java.util.Random;

/**
 * @author tomasz
 *
 */
public class GenerateWord {
	
	private Random rand = new Random();
	
	public char generateLowerCaseLetter() {
		char letter = (char)(rand.nextInt(122-97+1)+97);
		return letter;
	}
	
	public char generateUpperCaseLetter() {
		char letter = (char)(rand.nextInt(90-65+1)+65);
		return letter;
	}
	
	public String generateWord() {
		String word = "";
		for(int i=0; i<5; i++) {
			word += generateLowerCaseLetter();
		}
		return word;
	}
	
	public String generateWord(int range, String option) {
		String word = "";
		if(option == "lower") {
			for(int i=0; i<range; i++) {
				word += generateLowerCaseLetter();
			}
		} else if(option == "upper") {
			for(int i=0; i<range; i++) {
				word += generateUpperCaseLetter();
			}
		} else if(option == "capitalize") {
			word += generateUpperCaseLetter();
			for(int i=0; i<range-1; i++) {
				word += generateLowerCaseLetter();
			}
		}
		return word;
	}
	
}
