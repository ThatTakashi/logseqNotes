- ```java
  import java.util.Scanner;
  
  	public class Name2 {
        
  		public static void main(String[] args) {
            	Scanner answer = new Scanner(System.in);
              System.out.println("Enter your name: ");
              System.out.print(">>> ");
            
              String name = answer.nextLine();
              String border = "#";
            
              answer.close();
              System.out.println(border.repeat(name.length() + 8));
              System.out.println("# " + name + " #");
              System.out.println(border.repeat(name.length() + 8));
  		}
        
  	}
  ```
-