Java GUI Calculator - Summary and Documentation

Summary

This Java-based calculator is a simple GUI application that allows users to perform basic arithmetic operations. The calculator interface is built using Swing and AWT components, featuring a grid layout for buttons and a label for the display. It supports addition, subtraction, multiplication, division, percentage calculation, square root, and sign inversion. The program maintains internal states for operand A, operand B, and the selected operator, ensuring correct sequential computations.

Features

Basic Operations: Addition (+), Subtraction (-), Multiplication (×), Division (÷)

Additional Functions: Percentage (%), Square Root (√), Negation (+/-), Clear (AC)

Graphical User Interface: Built using JFrame, JPanel, JLabel, and JButton

Responsive UI: Color-coded buttons for easy differentiation of functions

Code Breakdown

1. GUI Components

JFrame frame: The main window for the calculator.

JLabel displayLabel: Displays the current input and result.

JPanel displayPanel: Contains the displayLabel.

JPanel buttonsPanel: Contains all calculator buttons.

Button Colors:

Numeric buttons: Dark gray

Operators (+, -, ×, ÷, =) : Orange

Special functions (AC, +/- , %) : Light gray

2. Button Functionality

Each button in the calculator is assigned a specific function via an ActionListener:

Number Buttons (0-9, .): Append digits or decimal to the display.

Operator Buttons (+, -, ×, ÷): Store operand A and operator while waiting for operand B.

Equals (=): Computes the result of the stored operation.

Special Buttons:

AC: Clears all stored values and resets the display.

+/-: Toggles the sign of the displayed number.

%: Converts the displayed number to a percentage.

3. Internal Computation

The calculator maintains three key variables:

A: Stores the first operand.

B: Stores the second operand.

operator: Stores the selected arithmetic operator.

When = is pressed, the calculator converts A and B into double values, performs the selected operation, updates the display, and resets values for the next operation.

4. Utility Methods

clearAll(): Resets all stored values.

removeZeroDecimal(double num): Converts results to integer format if they have no decimal values.

Known Issues & Improvements

Comparison Issues: String comparisons use == instead of .equals().

Chained Operations: Currently, only one operation can be performed at a time.

GUI Layout: Can be further refined for better responsiveness.

Conclusion

This Java calculator provides a functional and visually appealing interface for performing basic arithmetic operations. It can be expanded with features like history tracking, scientific functions, and improved error handling.

