## Activity Diagram
	- An Activity Diagram is a work flow chart representing the flow from one activity to another
	- Looks like a flow chart
	- ### Examples
		- {{renderer :mermaid_66ce45fb-0660-4433-bf37-c6efb191325a, 3}}
		  collapsed:: true
			- ```mermaid
			  flowchart TD
			      A[activity1] --> B(activity2)
			      A --> C(activity3)
			      B --> Z{B}
			      Z --> D(activity4)
			      Z --> E(activity5)
			      E --> F{J}
			      D --> F
			      F --> G(activity7)
			      C --> G
			  ```
		- {{renderer :mermaid_66ce4589-0b22-4c2c-b1cd-b7865b7f44e9, 3}}
		  collapsed:: true
			- ```mermaid
			  flowchart TD
			      A[Insert Card] --> B(Enter Pin)
			      B --> C{Pin Accepted?}
			      C -->|Pin Wrong| B
			      C --> D(Select type of transaction)
			      D --> E(Preform the transaction)
			      E --> F{Finished?}
			      F -->|Yes| D
			      F --> G(End the transaction)
			  ```
	- Can also be in the form of a swimming lane diagram
		- Shows each
	- ### How to draw an Activity Diagram
		- Identify the Use case
		- Identify the actors, system and other swim lanes
		- Identify activities that are performed and by whom
		- Identify the decisions that need to be made
		- Identify any activities that can be done in parallel
	- ### Activity Diagram Validation
		- You must ensure that your diagram is correct
			- Needs to be validated by the designer not the developers or programmers
		- An invalid diagram results in invalid system behaviour
		- If something is found to be wrong or missing in the diagram
			- Identify the problem and find a way to fix it. Get someone else to help check
			- Most often you will have misinterpreted the requirements