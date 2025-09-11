Project: clock-display
Authors: David Barnes and Michael Kölling

This project is part of the material for the book

   Objects First with Java - A Practical Introduction using BlueJ
   Seventh edition
   David J. Barnes and Michael Kölling

It is discussed in chapter 3.

To use this project, create an instance of class ClockDisplay. Then inspect this 
instance and leave the object inspector window open. With the inspector window open, 
call the object's methods, such as timeTick and setTime. Watch the 
"displayString" in the inspector.

The displayString field simulates the actual clock display device. Were this 
program running in a real clock, it would change the real, physical display 
hardware instead of this string. The timeTick method would be triggered once 
every minute by some timer hardware.

Everything else could be pretty much the same.


Note: This project does not implement adequate handling of errors.

Part 2 clock-display

Q21: It starts at 00:00 because the default constructor initializes hours and minutes to 0.
Q22: The inspector shows how method calls update "displaystring" to reflect the new time. For example, it starts at 00:00 and i clicked "timeTick()" two times which led the time to be "00:02".
Q23: Either tick it 60 times, or directly create a new clock at 01:00.
Q24: A variable digit of type NumberDisplay is defined and assigned in the Code Pad as: NumberDisplay digit = new NumberDisplay(10);
Q25: Rectangle window = new Rectangle(20, 30);
Q26: The second constructor lets the user create a ClockDisplay object starting at a chosen hour and minute by assigning those values directly to the NumberDisplay fields.
Q27: Two constructors both create hour and minute NumberDisplay objects, but the first sets the clock to 00:00 while the second one sets it to user-defined values. The second one doesnt really call updateDisplay() because the values are already initialized.
Q28: // Calls to rpint method
    p1.print("document1.pdf", true);
    p1.print("document1.txt", false); 
    // Calls to getStatus method
    p1.getstatus(5);
    p1.getstatus(10);
This demonstrates two calls for each method public void print(String filename, boolean doubleSided)
public int getStatus(int delay).

Q29: The types of objects created by the Picture constructor are 
     - Square objects
     - Triangle objects
     - Circle objects
     - Person objects
These help to create different parts of the picture, such as the roof, walls, sun, and window.
Q30:In the draw method of Picture, the Triangle object called roof has external methods cause like;
                   - moveHorizontal(int distance)
                   - moveVertical(int distance)
                   - changSize(int newHeight, int newWidth)
                   - makeVisible()
                   - makeInvisible()
Q31: There arent any internal methods however it contains external methods such as:   wall.moveVertical(20); wall.changeSize(120); wall.makeVisible();
- window.changeColor("black"); window.moveHorizontal(-120); window.moveVertical(40); window.changeSize(40); window.makeVisible();
- roof.changeSize(60, 180); roof.moveHorizontal(20); roof.moveVertical(-60); roof.makeVisible();
- sun.changeColor("yellow"); sun.moveHorizontal(100); sun.moveVertical(-40); sun.changeSize(80); sun.makeVisible();

Q32: The expression (8 % 3) gives 2. This is because 8 is divided by 3 is 2 remainder 2.
Q33: When using the modulo operator (%) with negative numbers:
- (-8 % 3) gives -2
- (8 % -3) gives 2
- (-8 % -3) gives -2
Sign of the result matches the sign of the dividend (first number).
Q34: The possible results are: 0, 1, 2, 3, 4
Q35: The possible results are: 0, 1, 2, 3, 4 ...., m-1 (remainder always from 0 to one less than the divisor,m.)
Q36: Challenge! To change a 24-hour clock to a 12-hour clock:
- if the internet hours value is 0 (midnight) or 12 (noon), display it as 12
- for hours 13-23, we substract 12 to convert it to PM hours
- minutes stay the same (0-59).

Q37: Two ways to make a 12-hour clock. 
- Option 1: Store hours internally from 1 to 12. The hour number display rolls over from 12 back to 1. Simpler to display, but harder if you need 24-hour internal calculations.

- Option 2: Keep hours internally as 24-hour values, but change the display. Internally, I will stay 0 to 23. Display converts from 0 to 12 AM., 13 to 1 PM, and 23 to 11 PM. Easier for calculations and updating time. Better option for most programs because internal logic remains consistent.
