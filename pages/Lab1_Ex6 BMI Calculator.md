- ```java
  public class BMI {
  	public static void main(String[] args) {
  		// TODO Auto-generated method stub
  		Scanner input = new Scanner(System.in);
  		System.out.println("Please enter your height (in meters):");
  		System.out.print(">>> ");
  
  		double height = input.nextDouble();
  
  		System.out.println("Please enter your weight (in kilograms):");
  		System.out.print(">>> ");
  
  		double weight = input.nextDouble();
  
  		input.close();
  
  		double bmi = weight / (height * height);
  
  		System.out.println(bmi);
  	}
  }
  ```
-