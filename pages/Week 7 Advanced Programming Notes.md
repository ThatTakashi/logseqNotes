## Event-driven Programming
	- A programming paradigm in which the flow of the program is determined by event such as user actions
	- Commonly used in graphical user interfaces
	- In an event-driven application, there is generally a main loop that listens for events, then triggers a callback function when one of those events is detected
	- Java can be used to write GUI programs/applications ranging from simple applets which run on a web page to sophisticated programs
- ## Java Swing
	- ### Top level Containers:
		- Contains all of the visual components of a GUI
		- Provides the screen real estate used by the application
		- JFrame, JApplet, JWindow, JDialog
	- ### Intermediate Containers:
		- Used to organise and position GUI components
		- JPanel
	- ### Lightweight Compontents:
		- Present information to or get information from the user
		- Button, Label, Text field, Editor pane, Combo box, Etc
	- ### JFrame
		- Graphical window on the screen
		- Typically holds (hosts) other components
		- Common methods:
			- **JFrame(String title** - Constructor, title optional
			- **setSize(int width, int height)** - Set size of window
			- **add(Component c)** - Add component to window
			- **setVisible(Boolean v)** - Makes the window visible or not
		- ### Example:
			- ```java
			  import javax.swing.JFrame;
			  import javax.swing.JButton;
			  
			  public class FrameDemo {
			    public static void main(String[] args) {
			      JFrame frame = new JFrame("My Frame");
			      frame.setSize(300, 200);
			      frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
			      JButton bOk = new JButton("OK");
			      frame.add(bOk);
			      frame.setVisible(true);
			    }
			  }
			  ```
	- ### JPanel
		- Commonly used as a place for graphics, or to hold a collection of buttons, labels, etc
		- Needs to be added to a window or other container
		- ### Layout
			- Each container has a layout manager
				- Determines the position and size of multiple containers on a panel
			- #### Border Layout
				- Divides the container into five reigns
				- Valid regins
					- NORTH
					- SOUTH
					- EAST
					- WEST
					- CENTER
				- **Border layout constructors**
			- #### Grid Layout
			- #### Flow Layout
				- Positions the components in a left to right and top to bottom manner, starting at the upper-left hand corner
				- **Flow layout constructors**
					- FlowLayout()
					- FlowLayout(int align)
					- FlowLayout(int align, int hgap, int vgap)
				- **Gap**
					- Spacing between the comonents
					- Measured in pixels