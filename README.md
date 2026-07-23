#waynemashudu
my SequentialDialogs code space

import javax.swing.JOptionPane;

public class Waynegift {

    public static void main(String[] args) {
        
        // Get student name from the first dialog
        String studentName = JOptionPane.showInputDialog(
            null,
            "Enter your student name:",
            "Step 1",
            JOptionPane.QUESTION_MESSAGE
        );

        // Make sure the input isn't empty or canceled
        if (studentName != null && !studentName.trim().isEmpty()) {
            
            // Show welcome message if valid name was entered
            JOptionPane.showMessageDialog(
                null,
                "Welcome to the system, " + studentName.trim() + "!",
                "Step 2",
                JOptionPane.INFORMATION_MESSAGE
            );

        } else {
            
            // Display error message if blank or canceled
            JOptionPane.showMessageDialog(
                null,
                "Error: No name was entered.",
                "Error",
                JOptionPane.ERROR_MESSAGE
            );

        }
    }
}
