## Class Recap
-
- ## Class Notes
	- ### What is OOP:
		- OOP revolves around the concept of objects as the basic elements of your programs
	- ### Popular OPP Languages:
		- Java, Javascript, C++
	- ### Objects in OOP:
		- Objects in the real world can easily be modelled as software objects using the properties as data and the behaviours as methods.
			- {{renderer :tables_66c26c13-65d3-418e-b536-36e18e016adc}}
			  collapsed:: true
				- data
					- Object
						- Car
					- Properties
						- Type of Transmission
						  Manufacturer
						  Color
					- Behavior
						- Turning
						  Braking
						  Accelerating
	- ### Why OOP?:
		- Keep large software projects manageable by human programmers
		- Better modelling of the real world
		- Modularization
		- Usability
		- Abstraction
		- Encapsulation
		- Extendibility-Hierarchy
		- Continuity-maintenance
	- ### What is a class?:
		- A definition of object of a same kind
		- Is a Blueprint/Plan/Template
		- A class is like a cookie cutter and the "cookies" is produces are the objects
			- One cookie cutter, many possible cookies
		- A class is a programmer-defined, reusable software entity
		- A class can be visualized as a box with 3 compartments consisting of:
			- Name/Identifier
			- Data Member/Variables
			- Behaviour - Methods or functions
		- ### Designing a class:
			- Declare Class
			  logseq.order-list-type:: number
			- Define Variables
			  logseq.order-list-type:: number
			- Define Constructor
			  logseq.order-list-type:: number
			- Define Methods
			  logseq.order-list-type:: number
	- ### What is an object?:
		- An object is an instance of a class sometimes called an object instance
		- The property values of an object instance is different from the once of other object instances of a same class
		- A class can be used to create many instances called objects
		- An object exists at run time only
		- An object has attributes that are carried with the object as it is used in a program
		- Each object or instance of a class maintains its own copy of an attribute in memory known as an instance variable
		- Objects of a particular class are created in Java by using the keyword **new**
			- ```java
			  MyClass myObject = new MyClass();
			  ```
	- ### Class Declaration:
		- ```java
		  public class Student() {
		  	// Other code here
		  }
		  ```
		- Public
			- Means that our class is accessible to other classes outside the package
		- Class declaration starts with keyword class
	- ### Constructors:
		- Telling Java the initial value of a variable in a class
		- id:: 66c28f8b-df08-4f43-a803-3a7bd1a6f135
		  ```java
		  public Student(String name, double g) {
		  	this.name = name;
		  	this.grade = g;
		  }
		  ```
	- ### Class Instance Declaration:
		- ```java
		  MyClass myObject = new MyClass();
		  ```
	- ### Methods:
		- A method can require one or more parameters that represent additional information (input) it needs to perform its task
		- Typically, you cannot call a method that belongs to another class until you create an instance of an object from that class
		- The number of arguments in a method call must match the number of parameters in the parameter list of the method's declaration
		- The argument types in the method call must be consistent with the the data types defined within the original method
	- ### Instance Variables:
		- Declare all your instance variables right after class declaration
		- Declare one variable for each line
		- Start variable name with a small letter
		- Use an appropriate data type
	- ### UML Basic Notation
		- {{renderer :tables_66c26e03-7649-4cee-923b-6ba1ee4379d6}}
		  collapsed:: true
			- data
				- Name
				  collapsed:: true
					- + = Public
						- = Private
					- + = Public
						- = Private
				- Student
				  collapsed:: true
					- + name : String
						- roll : int
						- section : String
					- + Display()
						- Add()
						- Edit()
				- Blank
					- Attributes
	- ### Access Modifiers
		- {{renderer :tables_66c26ee8-9972-46cc-84f0-8ce80b2c268b}}
		  collapsed:: true
			- data
			  collapsed:: true
				- Type
				  collapsed:: true
					- Inside Class
					- Same Package Class
					- Same Package Sub-Class
					- Other Package Class
					- Other Package Sub-Class
				- Private
				  collapsed:: true
					- Y
					- N
					- N
					- N
					- N
				- Default/No-Access
				  collapsed:: true
					- Y
					- Y
					- Y
					- N
					- N
				- Protected
				  collapsed:: true
					- Y
					- Y
					- Y
					- N
					- Y
				- Public
				  collapsed:: true
					- Y
					- Y
					- Y
					- Y
					- Y
	- ### Example Public Access Modifier:
		- ```java
		  public class Student {
		  	public String name;
		  
		  	public String getName() {
		  		return name;
		      }
		  
		  }
		  ```
	- ### Example Public Access Modifier:
		- ```java
		  public class Student {
		  
		  	private String name;
		  
		  	private String getName() {
		  		return name;
		  	}
		  
		  }
		  ```
		  
		  
		  
		  <!--EndFragment-->