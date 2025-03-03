# Swing-calculator-U23CE1025-

Chinedum Chukwudalu Prosper

U23CE1025

Civil Engineering Department 

ABOUT THE SWING CALCULATOR

This is a well-structured Java program for a simple calculator using the `javax.swing` library. It implements basic arithmetic functions (addition, subtraction, multiplication, division) along with some advanced functions like square, square root, and reciprocal. Additionally, the program includes features such as clearing the display, deleting the last character, and enabling/disabling the calculator using radio buttons.

Here are some key features and components of my code:

1. **Graphical User Interface (GUI):**
   - The main GUI consists of a `JFrame`, `JTextField`, and several `JButton` components for digits (0-9), operations (like +, -, *, /), and other functionalities such as clear (`C`), delete (`DEL`), square (`x²`), square root (`√`), reciprocal (`1/x`), and decimal (`.`).
   - There are also two radio buttons (`on` and `off`) to enable and disable the calculator.

2. **Action Listeners:**
   - The `ActionListener` interface is implemented to handle button clicks. It processes the button presses and performs corresponding operations (e.g., adding numbers, performing calculations).
   
3. **Enabling and Disabling the Calculator:**
   - The calculator can be enabled or disabled based on the state of the `onRadioButton` and `offRadioButton`. When "on" is selected, the calculator is active and the user can perform operations. When "off" is selected, the calculator is disabled, and all buttons are non-interactive.

4. **Mathematical Operations:**
   - It supports basic arithmetic operations (addition, subtraction, multiplication, and division) as well as more advanced operations (square, square root, reciprocal).
   - The `= (equal)` button performs the calculation based on the selected operation.

### Suggestions/Improvements:

1. **Handling Division by Zero:**
   - Currently, division by zero may cause an exception. It's a good idea to handle this case by checking if the denominator is zero and displaying an error message or handling it gracefully.

   Example:
   ```java
   if (Double.parseDouble(textField.getText()) == 0) {
       textField.setText("Error");
   }
   ```

2. **Decimal Input Validation:**
   - When a decimal point (dot) is pressed, it's only allowed if there's no dot already in the input. This is a good practice. However, if the input exceeds a certain length or reaches an unreasonable precision, you might want to consider rounding the result.

3. **Button Styling:**
   - I have used color styling for buttons, which is a great touch for enhancing the UI. However, for readability, consider improving the contrast for the labels or text colors based on the button colors to ensure better accessibility.

4. **Performance:**
   - The current design of the calculator seems to handle small calculations well. If you're planning to add more complex mathematical functions, you might need to consider optimizing the code for larger calculations or introducing additional functionality.

### Conclusion:
This calculator provides a simple yet functional GUI-based experience for performing arithmetic operations, and it includes additional features like square roots, squares, and the reciprocal. The use of colors and layout makes it visually appealing, and overall, it looks like a solid implementation for a desktop-based calculator application.
