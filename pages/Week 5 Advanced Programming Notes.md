## Notes
	- ### Data Structure
		- A data structure is a collection of data type "Values" which are stored and organised in such a way that it allows for efficient access to modification
		- There are two approaches to create a data structure
			- **Static Data Structures**
				- Structure that does not change in size while the program is running
					- Arrays
						- As once you delare their size, they cannot be changed
						- There are some languages that allow the changing of size of arrays
						- Pros
							- Resources allocated at compile time
							- Easy to use
							- Faster access to elements
						- Cons
							- Estimation of the maximum space is required
							- Waste a lot of resources if overestimating
							- Add, remove or modify elements is not directly possible or impossible
			- **Dynamic Data Structures**
				- Structures that can change size while a program is running
					- ArrayList
						- Pros
							- Ability to efficiently add, remove or modify elements
							- Flexible size
							- Effective use of resources - Resources are allocated at runtime as required
						- Cons
							- A bit more difficult to use
							- Can be slow to access elements
					- LinkedList
	- ### Arrays
		- A data structure that can hold many values
			- All values should be of the same type
		- Each individual value in the array is called **an elemenst**
		- All the values in the array must be of the **same type**
		- Each element is referred to by **an index number**
		- ### Array Examples
			- ```java
			  public class loopingArray {
			  	public static void main(String[] args) {
			  		int[] test = new int[10];
			  		for (int i = 0; i <= 9; i++) {
			  			test[i] = i;
			  		}
			  		
			  		for (int i : test) {
			  			System.out.println(i);
			  		}
			  	}
			  }
			  ```
			- ```java
			  public class Students {
			  	public static void main(String[] args) {
			  		String[] students = {"Jack", "Rachel", "Tim", "Anne", "Sam"};
			  		for (int i = 0; i < students.length; i++) {		
			  			System.out.println(students[i]);		
			  		}
			  		
			  		System.out.println("Number of Students: " + students.length);
			      }
			  }
			  ```
		- ### Declaring Arrays
			- To declare an array
				- Two line statement
					- ```java
					  type[] variable_name;
					  variable_name = new type[:number of elements:];
					  ```
				- One line statement
					- ```java
					  type[] variable_name = new type[:number of elements:];
					  ```
				- **E.g.**
					- ```java
					  String[] StudentNames = new String[10];
					  ```
		- ### Accessing Arrays
			- An individual element of an array can be accessed by it's index
			- To assign a data element into an array
				- ```java
				  StudentNames[0] = "John";
				  ```
			- Use the length property to get the total number of elements in an array
				- ```java
				  StudentNames.length;
				  ```
	- ### Multi-dimensional Array
		- Each element of the multi-dimensional array is an array
			- ```java
			  final int ROWS = 3, COLS = 6;
			  int[][] gamemap = new int[ROWS, COLS];
			  ```
				- Would visually produce a grid with 3 rows and 6 columns
				- {{renderer :tables_66c3bcde-0eae-45c8-a43c-9878382e5c71}}
				  collapsed:: true
					- data
					  collapsed:: true
						- :
						  collapsed:: true
							- 0
							- 1
							- 2
						- 0
						  collapsed:: true
							- -
							- -
							- o
						- 1
						  collapsed:: true
							- -
							- x
							- -
						- 2
						  collapsed:: true
							- x
							- -
							- -
						- 3
						  collapsed:: true
							- -
							- o
							- x
						- 4
						  collapsed:: true
							- -
							- -
							- x
						- 5
						  collapsed:: true
							- -
							- -
							- o
	- ### ArrayList
		- Java has a class called *ArrayList* which is a generic class that can be used to create a group of array objects
		- **Syntax**
			- ```java
			  ```
		- ### ArrayList: Add Method
			- ```java
			  arraylist.add(index, object);
			  ```
			- ```java
			  accounts.add(new BankAccount(123.45));
			  accounts.add(2, 100);
			  ```
		- ### ArrayList: Set Method
		- ### Arraylist: Get Method
			- ```java
			  arraylist.get(index);
			  ```
		- ### ArrayList: Remove Method
			- ```java
			  arraylist.remove(index);
			  ```
		- ### ArrayList: Size Method
			- ```java
			  arraylist.size();
			  ```
		- ### Traversing an ArrayList
			- To iterate through an ArrayList, we can use the same approach as we did with an Array
			- For loop:
				- ```java
				  ```
			- For each loop:
				- ```java
				  for (dataType item : array) {
				    System.out.println(item);
				  }
				  ```
				-