# BMITable
Produce a BMI measurement table for 5'5" person according to different weights

public class BMITable {

	public static void main(String[] args) {
		int height=65, weight=100, bmi=(weight*703)/(height*height);	
		System.out.println("BMI for a height of " + height/12 + " feet " + height%12 + " inches ");
	
		System.out.println("Weight\tBMI");
		
		for (int x=0; x<15; x++){
			weight +=5;
			bmi = (weight * 703)/ (height * height);
			System.out.println(weight + "\t" + (int) bmi);
		}
		


	}

}
