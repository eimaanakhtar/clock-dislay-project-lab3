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
This demonstrates two calls fro each method.
Q29
